# PARCIAL---Aprendizaje-Profundo
Este proyecto tiene como objetivo desarrollar un sistema de **clasificación de sonidos urbanos** utilizando técnicas de **Deep Learning**. Se trabaja con el conjunto de datos[UrbanSound8K] , que contiene grabaciones de audio urbano categorizadas en diez clases diferentes, como sirenas, tráfico, construcción, entre otros.
## Contenido del proyecto

El repositorio está organizado de la siguiente manera:

- **notebooks/**: Contiene notebooks con los experimentos realizados, incluyendo modelos densos (fully connected), LSTM y combinaciones CNN + LSTM. Cada notebook incluye análisis de desempeño, métricas y comparaciones entre arquitecturas.
- **deployment/**: Scripts necesarios para el despliegue en **AWS SageMaker**, incluyendo el preprocesamiento de audio, la lógica de predicción y el manejo de casos donde la probabilidad de predicción es baja (`indeterminado`).
- **README.md**: Explicación del proyecto, instrucciones de uso y guía para desplegar en la nube.
- **requirements.txt**: Dependencias necesarias para ejecutar los scripts y notebooks.

## Objetivos y enfoque

1. **Construir un modelo base (baseline)** y mejorar iterativamente según el análisis de sesgo y varianza.
2. **Evaluar distintas arquitecturas** de redes neuronales y comparar su desempeño.
3. **Implementar un modelo final en producción** en AWS SageMaker, con un endpoint que recibe un archivo de audio y devuelve la categoría más probable. Si la probabilidad máxima es menor a 0.6, la categoría se devuelve como "indeterminado".
4. **Documentar todo el proceso**, incluyendo preprocesamiento de audio, entrenamiento, validación y despliegue, para asegurar la reproducibilidad y comprensión completa del proyecto.

## Tecnologías utilizadas

- Python 3.x
- TensorFlow / Keras
- Librosa para procesamiento de audio
- AWS SageMaker para despliegue en la nube
- Git y GitHub para control de versiones

- [Modelo CNN + LSTM](https://colab.research.google.com/drive/10Faw2xwTkcYXryExTWDllBSkfELvEyNU?usp=sharing)
- [Modelo LSTM](https://colab.research.google.com/drive/1FsjaZrDDIMoCVRVn0OieoeqRF-5f6KpN?authuser=1#scrollTo=rK0uJvTSWRPT)
- [Modelo denso](https://colab.research.google.com/drive/1Yae_d_F1w7-i1OOxqCvIh20dSaPTfQKj?usp=sharing)
- [Modelo base (baseline)](https://colab.research.google.com/drive/10Ro3OLeJI7ewu7YJHRQta_Cgl9dY-J2t?usp=sharing)

