# Clasificación y diagnóstico de imágenes médicas por medio de algoritmos de Machine Learning y Deep Learning

Este repositorio contiene el material asociado al Trabajo Final de Máster (TFM) titulado **"Clasificación y diagnóstico de imágenes médicas por medio de algoritmos de Machine Learning y Deep Learning"**, realizado por **Lucía Salmerón Gallar** en el marco del **Máster Universitario en Ingeniería Biomédica y Salud Digital** (Universidad de Sevilla, junio 2025).

El codigo ha sido desarrollando utilizando la plataforma Google Collab. Este repositorio contiene tanto los Notebooks relacionados con el desarrollo, como los enlaces para acceder a Google Collab y ejecutarlos.

## Abstract

El melanoma, una de las formas más agresivas de cáncer de piel, ha experimentado un aumento constante en su incidencia global, haciendo que la detección temprana sea crucial para mejorar el pronóstico. Este proyecto explora la aplicación de algoritmos de Machine Learning (ML) y Deep Learning (DL) para la clasificación y diagnóstico automatizado de imágenes médicas de lesiones cutáneas. La finalidad de este estudio es optimizar los procesos de diagnóstico y reducir la variabilidad humana.

Se realizó un análisis comparativo de diversas arquitecturas de redes neuronales convolucionales (CNN) preentrenadas, como **VGG16**, **ResNet50**, **Xception**, **MobileNetV2**, **InceptionV3** y **EfficientNetV2**, utilizando un conjunto de datos desequilibrado del repositorio **ISIC Archive** (más de 50,000 imágenes de melanomas malignos y lesiones benignas). Las pruebas iniciales con datos desequilibrados mostraron una alta precisión pero una sensibilidad clínicamente inaceptable (63.31 %), con una elevada tasa de falsos negativos.

Para mitigar este desequilibrio, se implementaron técnicas de **balanceo de clases** (submuestreo, sobremuestreo y generación de datos sintéticos), así como estrategias de **fine-tuning** (descongelación progresiva de capas) y **aumento de datos avanzado** con la librería **Albumentations**. Estos esfuerzos mejoraron significativamente el rendimiento, especialmente la sensibilidad.

Los resultados finales tras el fine-tuning y el uso de Albumentations destacaron a **ResNet50** como la arquitectura más robusta, alcanzando una *accuracy* del **92.81 %**, un *AUC* del **93.94 %** y un *recall* del **76.86 %**. Esta mejora en la sensibilidad es fundamental para la detección temprana de melanomas. Aunque se observó un ligero aumento en los falsos positivos, la reducción de los falsos negativos es clínicamente más crítica.

El estudio concluye que la combinación de arquitecturas robustas con una estrategia de entrenamiento cuidadosa, incluyendo balanceo de clases y aumento de datos avanzado, es fundamental para el desarrollo de modelos de IA clínicamente útiles en dermatología. Se reconoce que, si bien los resultados son prometedores en un entorno controlado, se necesitan validaciones adicionales en escenarios clínicos reales y una integración con sistemas de soporte a la decisión médica para su aplicación práctica.

## Codigos

#### [Evaluacion_de_modelos_basico.ipynb:](https://github.com/luciasalmeron/TFM_Ingenieria_Biomedica_y_Salud_Digital/blob/main/Evaluacion_de_modelos_basico.ipynb)

Este codigo es...


#### [Evaluacion_de_modelos_balanceo_de_clases.ipynb:](https://github.com/luciasalmeron/TFM_Ingenieria_Biomedica_y_Salud_Digital/blob/main/Evaluacion_de_modelos_balanceo_de_clases.ipynb)

Este otro codigo es...

#### [Evaluacion_de_modelos_fine_tuning.ipynb](https://github.com/luciasalmeron/TFM_Ingenieria_Biomedica_y_Salud_Digital/blob/main/Evaluacion_de_modelos_fine_tuning.ipynb)

Este otro codigo es...


#### [ResNet50_con_Albumentations.ipynb:](https://github.com/luciasalmeron/TFM_Ingenieria_Biomedica_y_Salud_Digital/blob/main/ResNet50_con_Albumentations.ipynb)

Este otro codigo es...
