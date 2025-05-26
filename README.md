# RetroMorph 🎭

##  Enlace al repositorio

Este proyecto está disponible públicamente en GitHub:

➡️ [https://github.com/VanessaCamargo1606/RetroMorph](https://github.com/VanessaCamargo1606/RetroMorph)

##  Descarga directa del proyecto (.zip)

Si desea descargar todo el código directamente:

   [Descargar ZIP](https://github.com/VanessaCamargo1606/RetroMorph/archive/refs/heads/main.zip)

**RetroMorph** es una aplicación de escritorio desarrollada en Python con Tkinter que detecta la emoción de una persona a partir de una imagen, realiza un Face Swap con un personaje cinematográfico y permite aplicar un estilo artístico a la imagen final mediante técnicas de Neural Style Transfer (NST).

-  Detección de emociones con **EfficientNet**
-  Intercambio facial con **InsightFace** (`inswapper_128.onnx`)
-  Interfaz gráfica con **Tkinter**
-  Preparada para aplicar técnicas de estilizado artístico en etapas posteriores

Debido a las restricciones de tamaño en GitHub, el modelo inswapper_128.onnx no está incluido en este repositorio.
Puedes descargarlo manualmente desde el siguiente enlace de Google Drive:

🔗 [Descargar inswapper_128.onnx](https://drive.google.com/file/d/1krOLgjW2tAPaqV-Bw4YALz0xT5zlb5HF/view)

Una vez descargado, colócalo en la raíz del proyecto (junto a captura_emocion.py).

## Instalación 

Antes de continuar, asegúrate de tener Anaconda instalado.
Puedes descargarlo desde su página oficial:
🔗 https://www.anaconda.com/products/distribution

Abre **Anaconda Prompt**, CMD o la terminal de VSCode y sigue estos pasos:

1. Clona el repositorio:

git clone https://github.com/TU_USUARIO/RetroMorph.git
cd RetroMorph

2. Crea y activa un entorno virtual:

conda create -n morph python=3.10
conda activate morph

3. Instala las dependencias:

pip install -r requirements.txt

El modelo `inswapper_128.onnx` ya viene incluido en el repositorio dentro de la carpeta `models/`, por lo que no es necesario descargarlo manualmente.

4. Ejecuta el archivo principal:

python captura_emocion.py


## Si estás usando Visual Studio Code:

- Abre la carpeta del proyecto RetroMorph desde VSCode.
- Abre la terminal integrada con `Ctrl + ñ` o desde el menú "Terminal > Nueva terminal".
- Asegúrate de que el entorno `morph` esté activado. Si no lo está, actívalo con:
  
  conda activate morph

- Luego ejecuta el archivo principal con:

  python captura_emocion.py


## Requisitos del sistema

- Python 3.10 (recomendado)
- Windows 10 u 11
- 4 GB de RAM mínimo








