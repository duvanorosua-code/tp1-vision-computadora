# TP1 — Visión por Computadora

Notebook académico adaptado para ejecutarse localmente desde esta carpeta. Conserva los algoritmos, explicaciones, resultados y visualizaciones del notebook original; los cambios se limitan a la carga de datos y las rutas.

## Estructura

- datasets/white_patch/: ocho imágenes usadas por White-Patch.
- datasets/: img1_tp.png e img2_tp.png, usados en la Parte 2.
- outputs/white_patch/: imágenes corregidas generadas por el notebook.
- outputs/histogramas/: carpeta de resultados de histogramas.
- while_patch/, img1_tp.png, img2_tp.png y segmentacion.png: originales conservados en su ubicación.

segmentacion.png es un archivo adicional que no se utiliza en el TP.

## Ejecución

Abra TP1_Vision_Computadora.ipynb con el directorio de trabajo configurado en esta carpeta y ejecute todas las celdas. El notebook lee las diez imágenes de datasets/ mediante pathlib y crea las carpetas de outputs/ automáticamente.

Dependencias: Python, Jupyter, OpenCV (opencv-python), NumPy, Matplotlib y pandas.


## Entorno reproducible

El proyecto utiliza Python 3.12 y uv. Desde la raíz de TP1, sincroniza las dependencias con:

    uv sync

VS Code usa .venv/Scripts/python.exe como intérprete predeterminado. El notebook se asocia al kernel del proyecto Python 3.12 - TP1 Vision por Computadora.

Si reconstruyes .venv, regístralo de nuevo como kernel local del entorno con:

    uv run python -m ipykernel install --prefix .venv --name tp1-vision-computadora --display-name "Python 3.12 - TP1 Vision por Computadora"
