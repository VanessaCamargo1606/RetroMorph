# RetroMorph 🎭

##  Enlace al repositorio

Este proyecto está disponible públicamente en GitHub:

[https://github.com/VanessaCamargo1606/RetroMorph](https://github.com/VanessaCamargo1606/RetroMorph)

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

Abre Anaconda Prompt, CMD o la terminal de VSCode y sigue estos pasos, según cómo obtuviste el proyecto:

**Opción A** – Si clonaste el repositorio con Git:

1. Clona el repositorio:

git clone https://github.com/VanessaCamargo1606/RetroMorph.git
cd RetroMorph

**Opción B** – Si descargaste el proyecto como .zip:

1. Extrae el archivo .zip que descargaste.

2. Navega a la carpeta extraída desde la terminal:
cd RetroMorph-main

**A continuación, realiza los pasos comunes:**

1. Crea y activa un entorno virtual:

conda create -n morph python=3.10
conda activate morph

2. Instala PyTorch con soporte para GPU (recomendado):

Antes de instalar los requerimientos del proyecto, es necesario instalar manualmente PyTorch con soporte CUDA, ya que el archivo `requirements.txt` no incluye `torch` ni `torchvision` para evitar conflictos entre versiones de CPU y GPU.

⚠️ Importante: Si ya tienes instalados torch, torchvision o torchaudio, es necesario desinstalarlos antes de instalar la versión compatible con CUDA.

```bash
pip uninstall torch torchvision torchaudio
```

Si cuentas con una tarjeta NVIDIA, instala la versión de PyTorch compatible con CUDA 11.8 (asegúrate de tener el entorno morph activado):

```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```
3. Instala las dependencias:

pip install -r requirements.txt

4. Ejecuta el archivo principal:

python captura_emocion.py

## Requisitos del sistema

- Python 3.10 (recomendado)
- Windows 10 u 11
- 4 GB de RAM mínimo








