# Detector de Emociones y Reconocimiento Facial

Este proyecto implementa una aplicación en Python para detectar rostros en imágenes o vídeo y clasificar el estado de ánimo (feliz, triste, enojado, etc.) de cada rostro encontrado. Utiliza la biblioteca **OpenCV** para el preprocesamiento y detección facial, y la biblioteca **DeepFace** para el reconocimiento de emociones mediante modelos preentrenados de Deep Learning.

## Características

- Detección de rostros en tiempo real desde la cámara web o desde imágenes y vídeos.
- Clasificación de emociones faciales (feliz, triste, enojado, sorprendido, neutral, etc.) para cada rostro detectado.
- Visualización en directo con recuadros alrededor de las caras y etiquetas con la emoción dominante.
- Código modular y fácil de entender, ideal para fines educativos y como demostración de portafolio.

## Requisitos

Antes de ejecutar la aplicación, asegúrate de tener instalado:

- Python 3.8 o superior
- [OpenCV](https://pypi.org/project/opencv-python/)
- [DeepFace](https://github.com/serengil/deepface) y sus dependencias (TensorFlow, Keras, numpy, etc.)

Estas dependencias se gestionan automáticamente a través de `requirements.txt`.

## Instalación

Clona este repositorio y navega al directorio del proyecto:

```bash
git clone https://github.com/Dvstrada/detector-emociones-rostros.git
cd detector-emociones-rostros
```

Crea un entorno virtual (opcional pero recomendado) e instala las dependencias:

```bash
python -m venv venv
source venv/bin/activate   # En Windows usa: venv\Scripts\activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Uso

Para ejecutar la aplicación y empezar a detectar emociones desde la cámara web, ejecuta:

```bash
python app.py
```

Una ventana mostrará el vídeo de tu webcam con un recuadro alrededor de cada rostro detectado y una etiqueta con la emoción dominante. Presiona **q** para detener la aplicación.

Si quieres analizar una imagen o un vídeo en lugar de la cámara, puedes modificar el código de `app.py` para cargar un archivo y pasar el frame al análisis de DeepFace.

## Estructura

- `app.py` – script principal que captura vídeo, detecta rostros y clasifica emociones.
- `requirements.txt` – lista de dependencias del proyecto.
- `.gitignore` – configurado para proyectos Python.
- `LICENSE` – licencia MIT para el código de este repositorio.
- `README.md` – documentación del proyecto.

## Notas

- La primera vez que ejecutes la aplicación, DeepFace descargará los modelos preentrenados necesarios para la detección y reconocimiento de emociones; esto puede tardar varios segundos.
- Este proyecto se realiza con fines educativos y de demostración. La precisión del reconocimiento depende del modelo utilizado.

## Licencia

Este proyecto está licenciado bajo los términos de la licencia MIT. Consulta el archivo `LICENSE` para más información.
