<<<<<<< HEAD
# Análisis de un Dataset de Ejercicios

## Descripción

Este proyecto tiene como objetivo realizar un análisis exploratorio de un conjunto de datos para comprender su estructura, identificar patrones, detectar valores atípicos y obtener información que permita un mejor entendimiento del dataset.

## Objetivos

- Explorar las características del dataset.
- Analizar la calidad de los datos.
- Identificar Valores nulos y atípicos.
- Visualizar distribuciones y relaciones entre variables.
- Obtener conclusiones apartir de los datos previamente analizados.

## Extructura del proyecto

```
Analisis-dataset/
|- build/     # Reportes o resultados generados
|- src/       # Archivo de análisis
|- imagenes   # Graficas y visualizaciones
|-  smart_workout_raw_dataset.csv    # Readme.md
```

## Dataset
Smart_workout_raw_dataset.csv

Este conjunto de datos contiene información sobre la actividad física de los usuarios y atributos relacionados con el entrenamiento. El dataset está compuesto por diferentes tipos de variables, tanto numéricas como categóricas, las cuales sirven para realizar análisis descriptivos y exploratorios.

## Herramientas utilizadas
- Python
- Pandas
- Numpy
- Matloplib
- Seaborn
- Jupyter Notebook

## Metodologia

### 1. Carga de datos

Se importaron las librerías y el conjunto de datos. Posteriormente, se revisó su estructura general.

### 2. Limpieza de datos

Se verificaron los valores nulos presentes en el dataset:

```python
df.isnull().sum()
```
También se verificó la existencia de valores duplicados:

```python
df.duplicated().sum()
```

### 3. Estadisticas descriptivas

Se obtuvieron las medidas estadísticas básicas de las variables numéricas:

```python
df.describe()
```

### 4. Analisis de la variable objetivo

Se identificó la variable objetivo para posteriormente analizar su comportamiento.

```pthon
df['rating].value_counts()
```

### 5. Visualizacion de datos

Distribucion de la variable rating:

```python
sns.countplot(x='rating', data=df)
plt.show()
```

### 6. Analizamos las variables categoricas

Se analizaron las variables categóricas para identificar la frecuencia de cada categoría.

Para ello se utilizó:

```python
value_counts()
```

y distintos tipos de gráficos que permitieron visualizar:

-La categoría más frecuente.
-La categoría menos representada.
-La distribución general de las clases.

## Resultados

Se pudo encontrar unos hallazgos como:

-Existencia de valores faltantes.
-Presencia de valores duplicados.
-Detección de valores atípicos.

## Conclusiones

El análisis permitió obtener una mejor comprensión del dataset, identificar la variable objetivo y conocer el comportamiento de las variables numéricas y categóricas. Las visualizaciones ayudaron a detectar patrones y posibles anomalías en los datos.

## Aprendizaje 

Este proyecto me permitió fortalecer conocimientos en:

-Manipulación de datos.
-Visualización de datos mediante diferentes librerías.
-Identificación de variables objetivo.
-Análisis exploratorio de datos (EDA).

## Autor

José Gael Licea Vázquez

Proyecto desarrollado como práctica de la materia de Analítica de Datos de la carrera de Inteligencia Artificial. Se desarrolló utilizando Python y técnicas de exploración y análisis de datos.
=======
# Análisis de un Dataset de Ejercicios

## Descripción

Este proyecto tiene como objetivo realizar un análisis exploratorio de un conjunto de datos para comprender su estructura, identificar patrones, detectar valores atípicos y obtener información que permita un mejor entendimiento del dataset.

## Objetivos

- Explorar las características del dataset.
- Analizar la calidad de los datos.
- Identificar Valores nulos y atípicos.
- Visualizar distribuciones y relaciones entre variables.
- Obtener conclusiones apartir de los datos previamente analizados.

## Extructura del proyecto

```
Analisis-dataset/
|- build/     # Reportes o resultados generados
|- src/       # Archivo de análisis
|- imagenes   # Graficas y visualizaciones
|-  smart_workout_raw_dataset.csv    # Readme.md
```

## Dataset
Smart_workout_raw_dataset.csv

Este conjunto de datos contiene información sobre la actividad física de los usuarios y atributos relacionados con el entrenamiento. El dataset está compuesto por diferentes tipos de variables, tanto numéricas como categóricas, las cuales sirven para realizar análisis descriptivos y exploratorios.

## Herramientas utilizadas
- Python
- Pandas
- Numpy
- Matloplib
- Seaborn
- Jupyter Notebook

## Metodologia

### 1. Carga de datos

Se importaron las librerías y el conjunto de datos. Posteriormente, se revisó su estructura general.

### 2. Limpieza de datos

Se verificaron los valores nulos presentes en el dataset:

```python
df.isnull().sum()
```
También se verificó la existencia de valores duplicados:

```python
df.duplicated().sum()
```

### 3. Estadisticas descriptivas

Se obtuvieron las medidas estadísticas básicas de las variables numéricas:

```python
df.describe()
```

### 4. Analisis de la variable objetivo

Se identificó la variable objetivo para posteriormente analizar su comportamiento.

```pthon
df['rating].value_counts()
```

### 5. Visualizacion de datos

Distribucion de la variable rating:

```python
sns.countplot(x='rating', data=df)
plt.show()
```

### 6. Analizamos las variables categoricas

Se analizaron las variables categóricas para identificar la frecuencia de cada categoría.

Para ello se utilizó:

```python
value_counts()
```

y distintos tipos de gráficos que permitieron visualizar:

-La categoría más frecuente.
-La categoría menos representada.
-La distribución general de las clases.

## Resultados

Se pudo encontrar unos hallazgos como:

-Existencia de valores faltantes.
-Presencia de valores duplicados.
-Detección de valores atípicos.

## Conclusiones

El análisis permitió obtener una mejor comprensión del dataset, identificar la variable objetivo y conocer el comportamiento de las variables numéricas y categóricas. Las visualizaciones ayudaron a detectar patrones y posibles anomalías en los datos.

## Aprendizaje 

Este proyecto me permitió fortalecer conocimientos en:

-Manipulación de datos.
-Visualización de datos mediante diferentes librerías.
-Identificación de variables objetivo.
-Análisis exploratorio de datos (EDA).

## Autor

José Gael Licea Vázquez

Proyecto desarrollado como práctica de la materia de Analítica de Datos de la carrera de Inteligencia Artificial. Se desarrolló utilizando Python y técnicas de exploración y análisis de datos.
>>>>>>> 3a7861b (Analisis de dataset modificado)
