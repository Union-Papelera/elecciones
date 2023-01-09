# Elecciones de la Unión Papelera
En este repositorio se encuentran los resultados de las elecciones de la Unión Papelera.

## Verificación
Los resultados de las elecciones son proporcionados sin firmar pero también firmados digitalmente por la Unión Papelera.  
Para verificar la firma digital seguir estos pasos:

1. Necisitas instalar [GnuPG](https://gnupg.org/ "GnuPG")
1. Primero descarga nuestra [Clave Pública](https://unionpapelera.ml/assets/docs/clave-pgp.txt)
1. Ve al directorio donde la has descargado y abre una terminal
1. Ahora importa nuestra clave pública mediante
```bash
gpg --import clave-pgp.txt
```
2. Descarga el archivo que se encuentra en año/resultados-firmados.md
3. Ve al directorio donde se ha descargado, abre la terminal y ejecuta
```bash
gpg --verify resultados-firmados.md
```
4. Debería decirte "Firma correcta" o "Good signature"