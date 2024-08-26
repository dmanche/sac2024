# Síntesis de una base de datos y clasificación del movimiento humano basado en IMU mediante redes neuronales para la rehabilitación asistida con exoesqueleto

## Requisitos 
- Modelo SMPL. Es necesario disponer de la libreria [SMPL](https://smpl.is.tue.mpg.de/index.html), la cual contiene código necesario, así como los modelos SMPL utilizados.
- Librería [Aitviewer](https://github.com/eth-ait/aitviewer/tree/main/aitviewer).
- Librería [smpl](https://github.com/vchoutas/smplx/tree/main/smplx).
- Datos [AMASS](https://amass.is.tue.mpg.de/). En caso de que se requiera la base de datos con movimientos ya etiquetados, por favor contáctenme.

## Smplx

## Aitviewer
La carpeta aitviewer contiene la configuración usada durante el uso de la librería. Además contiene el archivo [smpl.py](./aitviewer/smpl.py), un archivo modificado proveniente de aitviewer/renderables/smpl.py. En caso de querer utilizarse, sustituir ambos archivos de la librería aitviewer previamente descargada por los archivos que se encuentran en [aitviewer](./aitviewer).

## Síntesis
El archivo [aux_and_synthesis.ipynb](./aux_and_synthesis.ipynb) contiene codigo auxiliar (leer y cargar datos en formato .pkl, representar modelos SMPL, pasar de .npz a .pkl...) y el código utilizado para realizar la síntesis de datos.


