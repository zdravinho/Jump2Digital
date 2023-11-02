# Jump2Digital

# Análisis de Componentes Principales en Datos de Alquiler y Ruido
## 1. Introducción
El conjunto de datos analizado proviene de la fusión de dos fuentes principales: datos relacionados con alquileres y datos relacionados con niveles de ruido en distintas áreas. Las variables seleccionadas para el análisis incluyen Codi_Districte, Codi_Barri, Any, Trimestre, y Valor.

## 2. Depuración de datos
### 2.1 Verificación de Valores Nulos
Antes de realizar cualquier análisis, se verificó la presencia de valores nulos en el conjunto de datos. Las decisiones sobre cómo tratar estos valores nulos se basaron en su cantidad y su relevancia para el análisis.

### 2.2 Conversión de Datos
Se identificó que la columna Valor estaba en formato de porcentaje. Por lo tanto, se realizó una conversión para transformar esta columna a formato numérico, facilitando su análisis posterior.

### 2.3 Estandarización
Dado que el Análisis de Componentes Principales es sensible a la escala de las variables, se procedió a estandarizar las variables numéricas para que tuvieran una media de 0 y una desviación estándar de 1.

## 3. Resultados
Tras aplicar el PCA, se identificó que:

El primer componente principal estaba principalmente influenciado por las variables geográficas (Codi_Districte y Codi_Barri).
El segundo componente principal estaba dominado por la variable Valor.
El análisis reveló que con solo los dos primeros componentes se podía explicar el 75% de la varianza en los datos.

## 4. Conclusiones
El PCA reveló que las dimensiones geográficas y el valor son las principales fuentes de variabilidad en el conjunto de datos.
Las técnicas de preprocesamiento, como la estandarización y la conversión de formatos, son esenciales para obtener resultados precisos y significativos con el PCA.
La capacidad de reducir la dimensionalidad del conjunto de datos sin perder mucha información es valiosa, especialmente cuando se trata de visualizaciones o modelos de aprendizaje automático.
