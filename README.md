# Trabajo Final Vision por computadora 2

Alumnos:

- Julian Ferreira
- Amilcar Rincon Charris
- Paola Cartala
  
### Detección de objetos y anomalías en imágenes mediante YOLOv11

Este proyecto implementa un sistema de detección automática de objetos utilizando la arquitectura **YOLOv11**, aplicado a un conjunto de datos de **imágenes de rayos X**.  

El trabajo forma parte del curso **Visión por Computadora 2** y tiene como objetivo evaluar el rendimiento de modelos de detección en escenarios con objetos pequeños, variaciones de color y diferentes niveles de 

brillo.

---
## Contenido del repositorio

Trabajo-Final-VPC2

- dataset/ # Conjunto de datos de entrenamiento y validación

- runs/ # Resultados de entrenamiento generados por YOLOv11

- notebook.ipynb # Notebook principal (entrenamiento y análisis)

- requirements.txt # Librerías necesarias

- README.md # Este archivo

## Descripción del flujo de trabajo

### Descarga y preparación del dataset
Se descarga automáticamente desde Kaggle (por ejemplo, X-ray Baggage Anomaly Detection).
Las etiquetas y rutas se definen en el archivo data.yaml.

### Entrenamiento del modelo YOLOv11
Entrenamiento con 150 épocas, tamaño de imagen de 960–1152 px y técnicas de data augmentation (mosaic, mixup, HSV).

### Validación y métricas
Se evalúa el modelo en el conjunto de validación, obteniendo métricas de precisión, recall y mAP (50–95).

### Análisis cromático por clase
Se realiza un estudio del espacio de color RGB/HSV para verificar si el modelo aprende por forma o por color, calculando:

### Histogramas por canal

## Fisher Score por canal

## Clasificador logístico HSV

## Visualización de nubes H–S

## Generación de evidencia de funcionamiento
Se produce un demo_evidencia.zip con:

Métricas de validación

Imágenes anotadas

Curvas de entrenamiento

Matriz de confusión y PR curve

Rendimiento (FPS/latencia)
