# Clasificación de imágenes con y sin filtro Sobel

Este proyecto compara el rendimiento de un modelo de clasificación de imágenes (CNN) utilizando la base de datos CIFAR-10 en dos versiones:

1. Imágenes originales.
2. Imágenes procesadas con el filtro Sobel.

# Objetivo

Evaluar si la aplicación del filtro **Sobel**, que resalta los bordes y contornos de las imágenes, mejora el rendimiento de un modelo de clasificación al facilitar la extracción de características importantes.

# Justificación del filtro Sobel

El **filtro Sobel** es un operador de detección de bordes que calcula la derivada de la intensidad de una imagen. Al aplicar este filtro:

- Se enfatizan los contornos y cambios abruptos de intensidad.
- Se pueden resaltar estructuras y formas clave en las imágenes.
- Se reduce el "ruido" visual al eliminar información redundante de color o textura que no es relevante para la clasificación.

Este filtro es especialmente útil en modelos que podrían beneficiarse de una entrada más simplificada y estructurada.

# Modelo utilizado

Se usó una red neuronal convolucional (CNN) sencilla con dos capas convolucionales y dos capas completamente conectadas. El objetivo fue enfocarse en la comparación del efecto del filtro Sobel, no en maximizar la precisión absoluta.

# Resultados esperados

Al final del entrenamiento, el programa imprime las precisiones del modelo entrenado:

- Sin filtro Sobel.
- Con filtro Sobel.

Con esto se evalúa si el preprocesamiento con Sobel mejora o no el rendimiento.



