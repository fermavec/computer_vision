# Computer Vision
## First Steps
1. Install all the dependencies:
```sh
pip install -r requirements.txt
```

## Structure
```
main/
├── README.md
├── .gitignore
├── requirements.txt
└── 01_ML-CV
    ├── 01_ML-CV.md
└── Intro-to-ML/
    └── data/
        ├── diabetes.csv
    ├── 01_reto-procesando-un-dataset.ipynb
```

# Notas y Apuntes
# Introducción a Machine Learning con Enfoque en Diabetes y Discapacidad Visual

## 1. Definición de Machine Learning

**Machine Learning (ML)** es una rama de la inteligencia artificial (IA) que se centra en el desarrollo de algoritmos y modelos que permiten a las computadoras aprender y hacer predicciones o decisiones basadas en datos. En lugar de ser explícitamente programadas para realizar una tarea específica, las máquinas aprenden de ejemplos y experiencias.

## 2. Tipos de Aprendizaje en Machine Learning

### a. Aprendizaje Supervisado

**Definición**: En el aprendizaje supervisado, el algoritmo de ML se entrena usando un conjunto de datos etiquetados. Cada ejemplo en el conjunto de datos tiene una entrada y una salida correspondiente. El objetivo es aprender una función que mapee entradas a salidas.

**Ejemplos**:
- **Clasificación**: Predecir la presencia de retinopatía diabética en imágenes de retina.
- **Regresión**: Predecir los niveles de glucosa en sangre basados en datos de sensores continuos.

**Aplicaciones**:
- **Diagnóstico de Retinopatía Diabética**: Utilizando imágenes de retina para detectar signos de retinopatía diabética.
- **Predicción de Niveles de Glucosa**: Modelos que predicen los niveles futuros de glucosa en sangre basados en mediciones pasadas y otros factores como la dieta y la actividad física.
- **Detección de Neuropatía Diabética**: Clasificación de pacientes en riesgo de desarrollar neuropatía diabética basada en historial médico y datos de sensores.

### b. Aprendizaje No Supervisado

**Definición**: En el aprendizaje no supervisado, el algoritmo de ML se entrena usando un conjunto de datos que no están etiquetados. El objetivo es encontrar patrones o estructuras en los datos.

**Ejemplos**:
- **Clustering**: Agrupar pacientes diabéticos en diferentes clusters basados en sus perfiles de glucosa y estilos de vida.
- **Asociación**: Encontrar patrones en los hábitos alimenticios que afectan los niveles de glucosa en sangre.

**Aplicaciones**:
- **Segmentación de Pacientes**: Identificar subgrupos de pacientes diabéticos con características y necesidades similares para personalizar tratamientos.
- **Análisis de Comportamiento**: Detección de patrones en los datos de actividad física y dieta que podrían estar correlacionados con cambios en los niveles de glucosa.

### c. Aprendizaje por Refuerzo

**Definición**: En el aprendizaje por refuerzo, un agente aprende a tomar decisiones interactuando con un entorno. Recibe recompensas o penalizaciones según las acciones que toma y ajusta su estrategia para maximizar la recompensa total.

**Ejemplos**:
- **Optimización de Dosis de Insulina**: Un agente que ajusta la dosis de insulina en tiempo real para mantener los niveles de glucosa dentro de un rango óptimo.
- **Asistencia para la Movilidad de Personas con Discapacidad Visual**: Un agente que aprende a guiar a una persona ciega a través de diferentes entornos usando retroalimentación en tiempo real.

**Aplicaciones**:
- **Sistemas de Administración de Insulina**: Algoritmos que optimizan la administración de insulina basándose en lecturas continuas de glucosa y otros datos.
- **Lazarillos Digitales**: Dispositivos que ayudan a personas con discapacidad visual a moverse de manera segura aprendiendo de sus interacciones con el entorno.

## 3. Aplicaciones de Machine Learning en Diabetes y Discapacidad Visual

### Diabetes
- **Predicción de Niveles de Glucosa**: Utilizando sensores continuos de glucosa y datos de actividad para predecir niveles futuros y alertar a los pacientes.
- **Diagnóstico de Complicaciones**: Detección temprana de complicaciones relacionadas con la diabetes como la retinopatía diabética, neuropatía y nefropatía mediante análisis de imágenes y otros datos médicos.
- **Gestión Personalizada de la Diabetes**: Aplicaciones que proporcionan recomendaciones personalizadas de dieta y ejercicio basadas en datos del usuario.

### Discapacidad Visual
- **Lectores de Pantalla Mejorados por IA**: Utilizando procesamiento de lenguaje natural y visión por computadora para leer texto en voz alta y describir imágenes a usuarios ciegos o con discapacidad visual.
- **Sistemas de Navegación**: Dispositivos portátiles o aplicaciones móviles que utilizan visión por computadora y aprendizaje por refuerzo para ayudar a personas con discapacidad visual a navegar en entornos complejos.
- **Reconocimiento de Objetos y Personas**: Aplicaciones que identifican y describen objetos y personas en tiempo real, proporcionando una mayor independencia a los usuarios con discapacidad visual.

Machine Learning está proporcionando herramientas innovadoras para mejorar la vida de personas con diabetes y discapacidad visual, permitiendo diagnósticos más precisos, gestión personalizada y asistencia en tiempo real.

# Importancia del Preprocesamiento en Machine Learning

El preprocesamiento de datos es una etapa crítica en el desarrollo de modelos de Machine Learning. Esta etapa implica preparar y transformar los datos en un formato adecuado para que los algoritmos de Machine Learning puedan utilizarlos eficazmente. La calidad de los datos y cómo se preparan pueden tener un impacto significativo en el rendimiento y la precisión de los modelos.

## ¿Por qué es importante el preprocesamiento?

1. **Mejora la Calidad de los Datos**: Datos ruidosos, inconsistentes o incompletos pueden afectar negativamente el rendimiento del modelo. El preprocesamiento ayuda a limpiar y preparar los datos, mejorando su calidad.
2. **Reducción de Sesgos**: Eliminar o corregir datos sesgados es crucial para evitar que el modelo aprenda patrones incorrectos.
3. **Optimización del Rendimiento del Modelo**: Transformar los datos a una escala común y eliminar características irrelevantes puede mejorar significativamente la eficiencia y la precisión del modelo.
4. **Manejo de Valores Faltantes**: Los valores faltantes pueden llevar a resultados incorrectos si no se manejan adecuadamente. El preprocesamiento permite abordar este problema de manera sistemática.

## Técnicas de Preprocesamiento

### 1. Limpieza de Datos

**Objetivo**: Eliminar o corregir datos que son incorrectos, incompletos, duplicados o irrelevantes.

**Pasos Comunes**:
- **Eliminación de Duplicados**: Remover registros duplicados del conjunto de datos.
- **Corrección de Inconsistencias**: Uniformizar formatos y correcciones ortográficas en los datos.
- **Filtrado de Datos Irrelevantes**: Eliminar características o registros que no aportan información útil para el modelo.

### 2. Normalización

**Objetivo**: Escalar las características numéricas para que tengan una escala común. Esto es importante para algoritmos que son sensibles a la escala de los datos, como la regresión logística y las redes neuronales.

**Técnicas Comunes**:
- **Min-Max Scaling**: Escala los datos para que estén dentro de un rango específico (normalmente 0 a 1).
- **Z-Score Normalization**: Transforma los datos para que tengan media 0 y desviación estándar 1.

### 3. Manejo de Valores Faltantes

**Objetivo**: Abordar los valores faltantes en los datos de manera que no afecten negativamente el rendimiento del modelo.

**Técnicas Comunes**:
- **Eliminación de Registros/Filas**: Si el porcentaje de valores faltantes es pequeño, se pueden eliminar los registros con valores faltantes.
- **Imputación de Valores**: Reemplazar valores faltantes con valores estimados, como la media, la mediana o el valor más frecuente.
- **Imputación Avanzada**: Utilizar técnicas más sofisticadas como la imputación mediante KNN (K-Nearest Neighbors) o modelos predictivos.

## Resumen

El preprocesamiento de datos es una etapa esencial en el pipeline de Machine Learning que asegura la calidad y la integridad de los datos utilizados para entrenar modelos. Las técnicas de limpieza de datos, normalización y manejo de valores faltantes son fundamentales para preparar los datos de manera adecuada y optimizar el rendimiento de los algoritmos de Machine Learning.

Al seguir estos pasos y aplicar estas técnicas, se puede garantizar que los datos estén en una forma óptima para el modelado, lo que lleva a modelos más precisos y robustos.

