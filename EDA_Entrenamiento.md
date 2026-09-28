# Analisis de un dataset de ejercicios

## Descripcion 

Este proyecto tiene como objetivo hacer un analisis exploratorio de un conjunto de datos con el objetivo de comprender, identificar patrones y detectar valores atipicos y obtener informacion para tener un mejor conocimiento del analisis

## Objetivos

- Explorar las caracteristicas del dataset
- Analizar la calidad de los datos
- Identificar Valores nulos y atipicos
- Visualizar distribuciones y relaciones entre variables
- Obtener conclusiones apartir de los datos previamente analizados

## Extructura del proyecto

```
Analisis-dataset/
|- build/     # Reportes o resultados generados
|- src/       # Archivo de analisi
|- imagenes   # Graficas y visualizaciones
|-  smart_workout_raw_dataset.csv    # Readme.md
```

## Dataset
Smart_workout_raw_dataset.csv

Este conjunto de datos (dataset) contiene informacion sobre la actividad fisica de los usuarios y atributos relacionados con el entrenamiento. Este dataset esta compuesto por las diferentes tipos de variables como numericas y categoricas las cuales nos van a servir para realizar analisis descriptivos y exploratorios.

## Herramientas utilizadas
- Python
- Pandas
- Numpy
- Matloplib
- Seaborn
- Jupyter Notebook

## Metodologia

### 1. Carga de datos

Se importo las librerias y el conjunto de datos, se reviso su extructura general

### 2. Limpieza de datos

Se verificaron los valores nulos presentes en el dataset 

```python
df.isnull().sum()
```
Se verificaron la exixtencia de valores duplicados 

```python
df.duplicated().sum()
```

### 3. Estadisticas descriptivas

Se obtuvieron las medidas basicas de la variable numericas:

```python
df.describe()
```

### 4. Analisis de la variable objetivo

Se obtuvo la variable objetivo para luego analizarla 

```pthon
df['rating].value_counts()
```

### 5. Visualizacion de datos

Distribucion de la variable ratin:

```python
sns.countplot(x='rating', data=df)
plt.show()
```

### 6. Analizamos las variables categoricas

Se Analizaron las variables categoricas para identificar la frecuencia de las categorias

Para ello se utlizo

```python
value_counts()
```

y ditintos tipos de graficos los cuales permitieron visualizar:

-Categoria mas frecuente
-Categoria menos representante
-Distribucion general de las clases

## Resultados

Se pudo encontrar unos hallazgos como:

-Existencia de valores faltantes.
-Presencia de valores duplicados
-Deteccion de valores atipicos

## Conclusiones

El analisis permitio tener una mejor compresion del dataset, identificar la variable objetivo conocer el comportamiento de las variables numericas y categoricas, la visualizacion ayudaron a encontrar los patrones y posibles anomalias en los datos.

## Aprendizaje 

Este proyecto me hizo fortalecer conocimientos en:

-Manipulacion de datos
-Visualizacion de datos con algunas librerias
-Identificar las variables objetivos

## Autor

Jose Gael Licea Vazquez

Proyecto desarrollado como practica de la materia de analitica de datos de la carrera de inteligencia artificial. Se desarrollo utilizando python y tecnicas de exploracion de datos.
