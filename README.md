# Synthesis And Classification (SAC): Síntesis de una base de datos y clasificación del movimiento humano basado en IMU mediante redes neuronales para la rehabilitación asistida con exoesqueleto

## Requisitos 
- Modelo SMPL. Es necesario disponer de la libreria [SMPL](https://smpl.is.tue.mpg.de/index.html), la cual contiene código necesario, así como los modelos SMPL utilizados.
- Librería [Aitviewer](https://github.com/eth-ait/aitviewer/tree/main/aitviewer).
- Librería [SMPLX](https://github.com/vchoutas/smplx/tree/main/smplx).
- Datos [AMASS](https://amass.is.tue.mpg.de/). En caso de que se requiera la base de datos con movimientos ya etiquetados, por favor contáctenme.
- La versión utilizada para python es la 3.8.0, versiones superiores pueden dar lugar a problemas con el uso de tensorflow.
- La versión utilizada para tensorflow es la 2.10.0. En caso de querer realizar la instalación, recomiendo el siguiente [tutorial](https://youtu.be/hHWkvEcDBO0?si=l2H_PB0Oysy1_lH3).

## Smplx
La carpeta contiene el archivo [body_models.py](./smplx/body_models.py). En caso de querer utilizarse, sustituirlo por el archivo del mismo nombre contenido en la librería SMPLX.

## Aitviewer
La carpeta aitviewer contiene la configuración usada durante el uso de la librería. Además contiene el archivo [smpl.py](./aitviewer/smpl.py), un archivo modificado proveniente de aitviewer/renderables/smpl.py. En caso de querer utilizarse, sustituir ambos archivos de la librería aitviewer previamente descargada por los archivos que se encuentran en [aitviewer](./aitviewer).

## Síntesis
El archivo [aux_and_synthesis.ipynb](./aux_and_synthesis.ipynb) contiene codigo auxiliar (leer y cargar datos en formato .pkl, representar modelos SMPL, pasar de .npz a .pkl...) y el código utilizado para realizar la síntesis de datos.

## Red

### Preprocesado
El archivo [preprocesado.ipynb](./preprocesado.ipynb) contiene el código relativo a la carga de datos y preprocesado realizado antes de introducir los datos en la red. También contiene el código de la evaluación.

### Redes
El archivo [Redes.ipynb](./Redes.ipynb) contiene las distintas redes usadas en el desarrollo del TFG.

## Datos
La carpeta con los datos ya sintetizados y clasificados se encuentra subida en [drive](https://drive.google.com/drive/folders/1n18zbdNR3EYaqvdYyHdoP9ouTpQiHxRh?usp=sharing).


