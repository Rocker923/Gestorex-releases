# Gestorex, instaladores

Este repositorio solo publica los instaladores de la aplicación de escritorio Gestorex.
**No contiene código fuente** y no debe contenerlo: es público para que el actualizador
de la aplicación pueda descargar las versiones nuevas sin credenciales.

## Cómo se publica una versión

1. Compilar el instalador con `python Build_Instalador.py` en el repositorio del proyecto.
2. Crear aquí una release con la etiqueta `vX.Y.Z` (con la **v**) y adjuntar el archivo
   `Installer_Gestorex_vX.Y.Z.exe` con ese nombre exacto. Publicarla, no dejarla en borrador.
3. Solo después, desplegar el backend con `CURRENT_VERSION = "X.Y.Z"`. En cuanto el backend
   anuncia la versión, las aplicaciones instaladas la ofrecen y la descargan de aquí.

Los instaladores no llevan ninguna credencial: solo la dirección del servidor.
