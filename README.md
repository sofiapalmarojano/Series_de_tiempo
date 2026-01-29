# Series_de_tiempo
# 📈 Series de Tiempo (Time Series Analysis)

Este repositorio contiene una introducción teórica y práctica al **análisis de series de tiempo**, cubriendo modelos clásicos y modernos utilizados en economía, finanzas y ciencia de datos.

---

## 1️⃣ Introducción a las Series de Tiempo

Una **serie de tiempo** es una secuencia de observaciones ordenadas cronológicamente. Su principal característica es que los datos **no son independientes**, ya que el pasado influye en el futuro.

### Componentes de una serie de tiempo

* **Tendencia (Trend):** comportamiento de largo plazo
* **Estacionalidad (Seasonality):** patrones que se repiten en intervalos regulares
* **Ciclo:** fluctuaciones no necesariamente periódicas
* **Ruido (Error):** variación aleatoria no explicada

### Ejemplos comunes

* Precios de acciones
* Tipo de cambio
* Inflación mensual
* Ventas por periodo
* Demanda energética

---

## 2️⃣ Modelos ARMA y SARIMA

### 🔹 Modelo ARMA (p, d, q)

Combina:

* **AR (AutoRegressive):** dependencia de valores pasados
* **MA (Moving Average):** dependencia de errores pasados

Forma general:
[
ARMA(p, q)
]

> ⚠️ Requiere que la serie sea **estacionaria**.

---

### 🔹 Modelo SARIMA (p, d, q)(P, D, Q)ₛ

Extiende ARIMA incorporando **estacionalidad**.

* (p, d, q): parte no estacional
* (P, D, Q): parte estacional
* s: periodo estacional (ej. s = 12 para datos mensuales)

Muy utilizado en:

* Series económicas
* Ventas con estacionalidad
* Pronósticos de demanda

---

## 3️⃣ Funciones de Autocorrelación

### 🔸 ACF (Autocorrelation Function)

Mide la correlación de la serie consigo misma en distintos rezagos.

* Útil para identificar el orden **q** del modelo MA

### 🔸 PACF (Partial Autocorrelation Function)

Mide la correlación directa entre observaciones separadas por k rezagos.

* Útil para identificar el orden **p** del modelo AR

---

## 4️⃣ Criterios de Selección de Modelos

### 🔹 Log-verosimilitud

Mide qué tan bien el modelo explica los datos observados.

> A mayor valor, mejor ajuste.

### 🔹 Criterio de Información de Akaike (AIC)

[
AIC = -2 \ln(L) + 2k
]

Penaliza la complejidad del modelo.

### 🔹 Criterio de Información Bayesiano (BIC)

[
BIC = -2 \ln(L) + k \ln(n)
]

Penaliza más fuertemente modelos complejos.

---

## 5️⃣ Modelos de Volatilidad

### 🔹 GARCH (Generalized ARCH)

Modela la **volatilidad condicional** de una serie.

Aplicaciones:

* Finanzas
* Riesgo
* Rendimientos bursátiles

Captura el fenómeno de **volatility clustering**.

---

### 🔹 EGARCH (Exponential GARCH)

Extensión del modelo GARCH que:

* Permite efectos asimétricos
* No requiere restricciones de positividad

Muy usado para analizar:

* Impactos negativos vs positivos en volatilidad
* Mercados financieros

---

## 📌 Objetivo del repositorio

* Entender la teoría detrás de los modelos
* Aplicarlos a datos reales
* Comparar desempeño entre modelos
* Facilitar el aprendizaje de series de tiempo

---

## 🧠 Requisitos

* Conocimientos básicos de estadística
* Álgebra lineal
* Programación (Python / R recomendado)

---

## 🚀 Autor

Repositorio creado con fines académicos y de aprendizaje en análisis de series de tiempo.
