# Revisión contable · releases

Paquetes de actualización de la aplicación de escritorio **Revisión contable** (desarrollo: [MEREBA](https://mereba.com)).

Este repositorio solo contiene **binarios firmados**, sin código fuente. Cada release publica un paquete de actualización:

- `actualizacion.json`: manifiesto (versión, notas y SHA-256 de cada instalador);
- `actualizacion.firma`: firma Ed25519 del manifiesto;
- el instalador de Windows (firmado con Authenticode) y la AppImage de Linux con `instalar-linux.sh`.

Las instalaciones comprueban la firma con una clave pública incrustada en la aplicación y solo aceptan versiones más nuevas que la instalada. Un paquete modificado o no firmado por MEREBA se rechaza, venga de donde venga.

No descargue ni ejecute estos ficheros a mano: la aplicación los descarga, los verifica y los instala desde *Administración → Actualizaciones*.
