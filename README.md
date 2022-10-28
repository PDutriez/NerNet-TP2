# Redes Neuronales - Trabajo Practico N°2 - Rossman Store Sales

En este práctico se trabajará con el dataset de Rossmann. Rossmann es una cadena de drugstores con más de 3000 tiendas en 7 países de Europa. La tarea que se intentará resolver con este dataset es el de predicción de las ventas totales de cada tienda que tendrán lugar en un intervalo de 6 semanas. Se uso como referencia para el preprocesamiento de datos y definir la red neuronal el siguiente repositorio: https://github.com/deeplearning-itba/kaggle-rossmann

El repositorio esta estructurado de la siguiente forma:
 - **dataset**: Set de información utilizado para el entrenamiento de redes.
 - **model_data**: Distintos datos de los modelos entrenados.
 - **notebooks**: Notebooks de datos utilizados para el trabajo práctico.
 - **procesed_data**: Recopilación de los datos procesados para el entrenamiento de las neuronas.
 - **submision_data**: Son los resultados obtenidos por distintas redes entrenadas, adentro esta el archivo pdutriez_submisions_data.csv que recopila toda la información de la redes y los resultados obtenidos en Kaggle.


## Mejor Score obtenido:

![](pdutriez_bestscore.jpeg)

## Preguntas teóricas del Trabajo Práctico

- **¿Qué son los Entity Embeddings y cómo se relacionan con las variables categóricas?** 

Los Entity Embeddings son parámetros para representar la relación que tienen distintas variables para ser procesados de una manera más ordenada y fácil. Un problema en las redes neuronales es la forma en que un objeto es analizado por sus parámetros y luego como los relaciona entre sí, dado que todas las caracteristicas propias del objeto son discretas existe un problema de discontinuidad en los datos. Por eso los Entity Embeddings resuelven este problema creando una continuidad intrínseca entre los datos para que la red neuronal pueda obtener mejores resultados.

- **Explicación la métrica utilizada en la competencia.**

La métrica utilizada en la competencia es la Root Mean Square Percentage Error (RMSPE). Esta métrica a diferencia de la RMSE para el contexto del trabajo, nos permite independizar de la cantidad de ventas de cada local al ser un error porcentual y no absoluto. Entonces se pondera de igual forma las ventas de todos los lugares sin importart la cantidad de ventas.
