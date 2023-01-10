# Elecciones de la Unión Papelera
En este repositorio se encuentran los resultados de las elecciones de la Unión Papelera.

## Verificación
Los resultados de las elecciones son proporcionados sin firmar pero también firmados digitalmente por la Unión Papelera.  
Para verificar la firma digital seguir estos pasos:

1. Necisitas instalar [GnuPG](https://gnupg.org/ "GnuPG")
1. Primero descarga nuestra [clave PGP pública](https://unionpapelera.ml/assets/docs/clave-pgp.txt "Clave PGP pública")
1. Ve al directorio donde la has descargado y abre una terminal
1. Ahora importa nuestra clave pública mediante
```bash
gpg --import clave-pgp.txt
```
5. Comprueba que el fingerprint coincida con el [nuestro](https://unionpapelera.ml/assets/docs/fingerprint-de-la-clave-pgp.txt "Fingerprint") mediante el comando
```bash
gpg --fingerprint gobiernopapelero@mailfence.com
```
6. Descarga el archivo que se encuentra en año/resultados-firmados.md
7. Ve al directorio donde se ha descargado, abre la terminal y ejecuta
```bash
gpg --verify resultados-firmados.md
```
8. Debería decirte "Firma correcta" o "Good signature" aunque saldrá un aviso de PRECAUCIÓN si no has tomado medidas para confiar en el camino a nuestra clave.  
9. Es una buena práctica volver a comprobar que el fingerprint coincida.