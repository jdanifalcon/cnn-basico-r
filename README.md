# Redes neuronales ✨

**Autor:** Jessica Daniela Ocaña Falcón
**Repositorio creado para el taller:** *Introducción básica a Redes Neuronales Convolucionales en R*
**Fecha de realización:** Marzo 2026

---

## 📑 Tabla de contenidos

1. Introducción
2. Hardware y software
3. Descripción de los frameworks
   3.1 TensorFlow
   3.2 Keras
   3.3 ggplot2
   3.4 MNIST
4. Tipos de redes neuronales
   4.1 Red neuronal profunda (DNN)
   4.2 Red neuronal convolucional (CNN)
   4.3 Red neuronal recurrente (RNN)
5. Diseño de la aplicación
6. Descripción del modelo
7. Implementación
   7.1 Red neuronal profunda (DNN)
   7.1.1 Búsqueda y experimentos de parámetros
   7.1.2 Descripción del algoritmo
   7.2 Red neuronal convolucional (CNN)
   7.2.1 Búsqueda y experimentos de parámetros
   7.2.2 Descripción del algoritmo
8. Ejecución de la aplicación
9. Bibliografía

---

## 1. Introducción

Este repositorio tiene como objetivo introducir los fundamentos de las redes neuronales, con énfasis en las Redes Neuronales Convolucionales (CNN) utilizando el lenguaje R.

El taller aborda los conceptos básicos del aprendizaje profundo, el flujo general de construcción de modelos y una implementación práctica orientada a la clasificación de imágenes.

---

## 2. Hardware y software

**Hardware recomendado:**

* Procesador multinúcleo
* 8 GB de RAM (mínimo recomendado)
* GPU opcional

**Software utilizado:**

* R (versión reciente)
* RStudio
* TensorFlow (backend)
* Keras para R
* ggplot2 (visualización)

---

## 3. Descripción de los frameworks

### 3.1 TensorFlow

TensorFlow es una biblioteca de código abierto para aprendizaje automático y aprendizaje profundo. En este proyecto funciona como backend para el entrenamiento y optimización de modelos.

---

### 3.2 Keras

Keras es una API de alto nivel que permite construir y entrenar redes neuronales de forma sencilla. En este taller se utiliza su interfaz en R.

---

### 3.3 ggplot2

ggplot2 es una biblioteca de visualización en R basada en la gramática de los gráficos, utilizada para representar resultados y métricas del modelo.

---

### 3.4 MNIST

MNIST es un conjunto de datos que contiene imágenes de dígitos escritos a mano (0–9). Es ampliamente utilizado para introducir modelos de clasificación con redes neuronales.

---

## 4. Tipos de redes neuronales

### 4.1 Red neuronal profunda (DNN)

Las Redes Neuronales Profundas (Deep Neural Networks) están compuestas por múltiples capas densas (fully connected). Se utilizan en tareas de clasificación y regresión cuando los datos no requieren estructura espacial explícita.

---

### 4.2 Red neuronal convolucional (CNN)

Las Redes Neuronales Convolucionales (Convolutional Neural Networks) están diseñadas para procesar datos con estructura espacial, como imágenes. Utilizan filtros (kernels), capas convolucionales y capas de pooling para extraer características automáticamente.

---

### 4.3 Red neuronal recurrente (RNN)

Las Redes Neuronales Recurrentes (Recurrent Neural Networks) están diseñadas para trabajar con datos secuenciales, como texto o series temporales, manteniendo memoria de estados anteriores.

---

## 5. Diseño de la aplicación

La aplicación sigue el siguiente flujo de trabajo:

1. Carga y preprocesamiento de datos
2. Definición del modelo
3. Compilación del modelo
4. Entrenamiento
5. Evaluación
6. Visualización de resultados

---

## 6. Descripción del modelo

El modelo implementado en este taller corresponde a una CNN básica compuesta por:

* Capa convolucional
* Capa de max pooling
* Capa flatten
* Capas densas
* Capa de salida con función de activación softmax

El objetivo es clasificar imágenes del conjunto de datos MNIST.

---

## 7. Implementación

### 7.1 Red neuronal profunda (DNN)

Se implementa una red neuronal con capas densas para comparar su desempeño frente a una CNN.

#### 7.1.1 Búsqueda y experimentos de parámetros

Se realizan pruebas variando:

* Número de capas
* Número de neuronas
* Funciones de activación
* Optimizadores
* Número de épocas

#### 7.1.2 Descripción del algoritmo

1. Inicialización de pesos
2. Propagación hacia adelante
3. Cálculo de la función de pérdida
4. Retropropagación
5. Actualización de pesos

---

### 7.2 Red neuronal convolucional (CNN)

Se implementa una CNN básica orientada a clasificación de imágenes.

#### 7.2.1 Búsqueda y experimentos de parámetros

Se evalúan variaciones en:

* Número de filtros
* Tamaño del kernel
* Número de capas
* Número de épocas

#### 7.2.2 Descripción del algoritmo

1. Aplicación de filtros (convolución)
2. Extracción automática de características
3. Reducción dimensional mediante pooling
4. Clasificación final mediante capas densas

---

## 8. Ejecución de la aplicación

Instalar dependencias:

```r
install.packages("keras")
install.packages("tensorflow")
install.packages("ggplot2")

library(keras)
library(tensorflow)
library(ggplot2)

install_keras()
```

Posteriormente ejecutar los scripts en el orden establecido en el repositorio.

---

## 9. Bibliografía

* Documentación oficial de TensorFlow
* Documentación oficial de Keras
* Material introductorio de aprendizaje profundo
* Dataset MNIST

---

Si quieres, puedo ahora ayudarte a que el README se vea todavía más profesional con:

* Badges de GitHub
* Sección de instalación más detallada
* GIF del modelo entrenando
* Enlace a diapositivas del taller

Tú dime el nivel de formalidad que quieres proyectar 👀✨
