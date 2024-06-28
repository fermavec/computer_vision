# Proyecto: Asistente Inteligente de Navegación para Personas con Discapacidad Visual

## Descripción del Proyecto
El proyecto consiste en desarrollar un asistente inteligente de navegación para personas con discapacidad visual. Este asistente utilizará técnicas de machine learning para identificar y clasificar objetos en tiempo real a través de una cámara portátil y proporcionar retroalimentación auditiva sobre el entorno del usuario. El asistente también podrá reconocer texto y señales, ayudando al usuario a moverse de manera más segura y eficiente en su vida diaria.

## Objetivos del Proyecto
1. **Desarrollar un modelo de machine learning** para la detección y clasificación de objetos.
2. **Implementar una solución de reconocimiento de texto** para leer señales y otros textos relevantes en el entorno.
3. **Proporcionar retroalimentación auditiva en tiempo real** basada en la detección y clasificación de objetos y textos.

## Datasets Recomendados
1. **COCO Dataset**: Un gran conjunto de datos que contiene imágenes de objetos comunes en sus contextos naturales. [COCO Dataset](https://cocodataset.org/#home)
2. **Open Images Dataset**: Un conjunto de datos con millones de anotaciones para detección de objetos. [Open Images Dataset](https://storage.googleapis.com/openimages/web/index.html)
3. **ICDAR 2013**: Un conjunto de datos para el reconocimiento de texto en escenas naturales. [ICDAR 2013](http://rrc.cvc.uab.es/?ch=2&com=downloads)

## Temario

### Semana 1: Fundamentos de Machine Learning Aplicados al Proyecto

**Día 1: Introducción a Machine Learning y al Proyecto**
- **Teoría:** Definición de Machine Learning, tipos de aprendizaje (supervisado, no supervisado, por refuerzo), aplicaciones.
- **Práctica Proyecto:** Instalación de Python y bibliotecas (numpy, pandas, scikit-learn, matplotlib). Configuración del entorno de desarrollo. Descripción del proyecto y objetivos.

**Día 2: Preprocesamiento de Datos**
- **Teoría:** Importancia del preprocesamiento, técnicas (limpieza de datos, normalización, manejo de valores faltantes).
- **Práctica Proyecto:** Recolección y preparación de un conjunto de datos inicial de imágenes. Ejercicios de limpieza y preprocesamiento con estas imágenes.

**Día 3: Conjuntos de Datos y Visualización**
- **Teoría:** Tipos de conjuntos de datos, división en entrenamiento y prueba, visualización de datos.
- **Práctica Proyecto:** Uso de pandas y matplotlib para explorar y visualizar el conjunto de datos de imágenes.

**Día 4: Modelos de Aprendizaje Supervisado**
- **Teoría:** Introducción a regresión lineal y logística.
- **Práctica Proyecto:** Implementación de un modelo de clasificación simple (e.g., regresión logística) para clasificar imágenes en categorías básicas (e.g., objetos vs. no objetos).

**Día 5: Evaluación de Modelos**
- **Teoría:** Métricas de evaluación (precisión, recall, F1-score, matriz de confusión).
- **Práctica Proyecto:** Evaluación del modelo de clasificación utilizando scikit-learn. Ajuste del modelo basado en los resultados de la evaluación.

**Día 6: Algoritmos de Clasificación**
- **Teoría:** K-Nearest Neighbors (KNN), Support Vector Machines (SVM).
- **Práctica Proyecto:** Implementación y comparación de KNN y SVM en el conjunto de datos del proyecto. Selección del mejor modelo basado en el desempeño.

**Día 7: Trabajo en el Proyecto**
- **Práctica Proyecto:** Refinamiento del modelo seleccionado. Ampliación del conjunto de datos de imágenes si es necesario. Pruebas adicionales y ajustes.

### Semana 2: Aplicaciones Avanzadas de Machine Learning

**Día 8: Árboles de Decisión y Random Forest**
- **Teoría:** Fundamentos de árboles de decisión y Random Forest.
- **Práctica Proyecto:** Implementación de Random Forest en el conjunto de datos del proyecto. Comparación de resultados con modelos anteriores.

**Día 9: Reducción de Dimensionalidad**
- **Teoría:** Introducción a PCA (Principal Component Analysis).
- **Práctica Proyecto:** Aplicación de PCA para la reducción de dimensionalidad en el conjunto de datos de imágenes. Evaluación del impacto en el desempeño del modelo.

**Día 10: Clustering**
- **Teoría:** K-means, clustering jerárquico.
- **Práctica Proyecto:** Implementación de algoritmos de clustering para identificar patrones no etiquetados en el conjunto de datos. Exploración de posibles aplicaciones en el proyecto.

**Día 11: Implementación de Modelos en el Proyecto**
- **Práctica Proyecto:** Entrenamiento de un modelo de clasificación de objetos utilizando el conjunto de datos refinado. Preparación del sistema para la integración de OCR.

**Día 12: Reconocimiento de Texto**
- **Teoría:** Introducción a OCR (Optical Character Recognition).
- **Práctica Proyecto:** Implementación de OCR utilizando Tesseract para reconocer texto en imágenes del proyecto. Integración del reconocimiento de texto con el sistema de clasificación de objetos.

**Día 13: Integración del Proyecto**
- **Práctica Proyecto:** Integración del modelo de clasificación de objetos y OCR en una aplicación que proporciona retroalimentación auditiva. Desarrollo de la interfaz de usuario.

**Día 14: Pruebas y Evaluación del Proyecto**
- **Práctica Proyecto:** Pruebas de la aplicación en escenarios reales. Evaluación de su desempeño. Ajustes y mejoras basados en los resultados de las pruebas.

### Resultados Esperados
Al final de las dos semanas, habrás aprendido los conceptos clave de machine learning mientras desarrollas un asistente inteligente de navegación para personas con discapacidad visual. El prototipo funcional podrá clasificar objetos y reconocer texto en tiempo real, proporcionando retroalimentación auditiva al usuario.
