# 🧠 Redes Neuronales

> 📘 **Repositorio del taller:** *Introducción básica a Redes Neuronales Convolucionales en R*
> 
> 👩🏻‍💻 **Autor:** Jessica Daniela Ocaña Falcón
> 
> 📅 **Fecha de realización:** Marzo 2026

---

---

# 📑 Tabla de contenidos

* 🔹 **1. Introducción**

* 🔹 **2. Software**

* 🔹 **3. Descripción de los frameworks**

  * ▪️ **3.1 TensorFlow**
  * ▪️ **3.2 Keras**
  * ▪️ **3.3 ggplot2**
  * ▪️ **3.4 MNIST**

* 🔹 **4. Tipos de redes neuronales**

  * ▪️ **4.1 Red neuronal profunda (DNN)**
  * ▪️ **4.2 Red neuronal convolucional (CNN)**
  * ▪️ **4.3 Red neuronal recurrente (RNN)**

* 🔹 **5. Diseño de la aplicación**

* 🔹 **6. Descripción del modelo**

* 🔹 **7. Implementación**

  * ▪️ **7.1 Red neuronal profunda (DNN)**

    * ▫️ **7.1.1 Búsqueda y experimentos de parámetros**
    * ▫️ **7.1.2 Descripción del algoritmo**
  * ▪️ **7.2 Red neuronal convolucional (CNN)**

    * ▫️ **7.2.1 Búsqueda y experimentos de parámetros**
    * ▫️ **7.2.2 Descripción del algoritmo**

* 🔹 **8. Ejecución de la aplicación**

* 🔹 **9. Bibliografía**

---

---

# 1️⃣ Introducción

Este repositorio tiene como objetivo introducir los fundamentos de las **redes neuronales**, con énfasis en las **Redes Neuronales Convolucionales (CNN)** utilizando el lenguaje **R**.

El taller aborda:

* ✔ Conceptos básicos de aprendizaje profundo
* ✔ Flujo general de construcción de modelos
* ✔ Implementación práctica en R
* ✔ Clasificación de imágenes mediante CNN

---

# 2️⃣ Software

## 🧰 Software utilizado

* **R (versión reciente)**
* **RStudio**
* **TensorFlow (backend)**
* **Keras para R**
* **ggplot2 (visualización)**

---

# 3️⃣ Descripción de los frameworks

---

## 🔹 3.1 TensorFlow

**TensorFlow** es una biblioteca de código abierto para aprendizaje automático y aprendizaje profundo.
En este proyecto funciona como **backend** para el entrenamiento y optimización de modelos.

---

## 🔹 3.2 Keras

**Keras** es una API de alto nivel que permite construir y entrenar redes neuronales de forma sencilla.
En este taller se utiliza su **interfaz en R**.

---

## 🔹 3.3 ggplot2

**ggplot2** es una biblioteca de visualización en R basada en la gramática de los gráficos.
Se utiliza para representar métricas del modelo y resultados del entrenamiento.

---

## 🔹 3.4 MNIST

**MNIST** es un conjunto de datos que contiene imágenes de dígitos escritos a mano (0–9).

Se utiliza porque:

* ✔ Es un dataset clásico para introducción a CNN
* ✔ Es ligero
* ✔ Permite visualizar fácilmente el desempeño del modelo

---

# 4️⃣ Tipos de redes neuronales

---

## 🔹 4.1 Red neuronal profunda (DNN)

Las **Deep Neural Networks (DNN)** están compuestas por múltiples capas densas (*fully connected*).

Se utilizan en tareas de:

* Clasificación
* Regresión
* Problemas tabulares

---

## 🔹 4.2 Red neuronal convolucional (CNN)

Las **Convolutional Neural Networks (CNN)** están diseñadas para procesar datos con estructura espacial, como imágenes.

Características principales:

* 🔎 Uso de filtros (kernels)
* 🧩 Extracción automática de características
* 📉 Reducción dimensional mediante *pooling*

---

## 🔹 4.3 Red neuronal recurrente (RNN)

Las **Recurrent Neural Networks (RNN)** están diseñadas para trabajar con datos secuenciales, como:

* Texto
* Series temporales
* Señales

---

# 5️⃣ Diseño de la aplicación

La aplicación sigue el siguiente flujo:

1. 📥 Carga y preprocesamiento de datos
2. 🧠 Definición del modelo
3. ⚙️ Compilación
4. 🚀 Entrenamiento
5. 📊 Evaluación
6. 📈 Visualización de resultados

---

# 6️⃣ Descripción del modelo

La CNN implementada está compuesta por:

* 🟢 Capa convolucional
* 🔵 Capa de max pooling
* 🟡 Capa flatten
* 🟣 Capas densas
* 🔴 Capa de salida con activación **softmax**

Objetivo:
Clasificar imágenes del dataset MNIST.

---

# 7️⃣ Implementación

---

## 🔹 7.1 Red neuronal profunda (DNN)

Se implementa una red con capas densas para comparar su desempeño con la CNN.

### ▫️ 7.1.1 Búsqueda y experimentos de parámetros

Se realizan pruebas variando:

* Número de capas
* Número de neuronas
* Funciones de activación
* Optimizadores
* Número de épocas

### ▫️ 7.1.2 Descripción del algoritmo

1. Inicialización de pesos
2. Propagación hacia adelante
3. Cálculo de la pérdida
4. Retropropagación
5. Actualización de pesos

---

## 🔹 7.2 Red neuronal convolucional (CNN)

Implementación orientada a clasificación de imágenes.

### ▫️ 7.2.1 Búsqueda y experimentos de parámetros

Se evalúan variaciones en:

* Número de filtros
* Tamaño del kernel
* Número de capas
* Número de épocas

### ▫️ 7.2.2 Descripción del algoritmo

1. Aplicación de filtros (convolución)
2. Extracción de características
3. Reducción dimensional (pooling)
4. Clasificación final

---

# 8️⃣ Ejecución de la aplicación

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

Posteriormente ejecutar los scripts en el orden indicado en el repositorio.

---

# 9️⃣ Bibliografía

* Documentación oficial de TensorFlow
* Documentación oficial de Keras
* Material introductorio de aprendizaje profundo
* Dataset MNIST

---
