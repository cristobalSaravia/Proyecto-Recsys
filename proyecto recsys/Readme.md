# Ambiente

Se utilizó google colab con el ambiente gpu t4.

# Code carbon proyecto movie lens

Aquí se encuentra el código de las pruebas sobre el dataset movielens. Se probó con 100k, 1m y 20m, pero finalmente se mantuvo con 1m para todos los experimentos. Se obtienen las emisiones de carbono con CodeCarbon. Los experimentos con ALS se realizan con la librería implicit. Los experimentos para Deepfm y Multivae se realizan con tensorflow y tensorflow recommenders. No todos los gráficos están ejecutados en el código, sin embargo, los datos se encuentran en los archivos csv para cada modelo con terminación _tracker.csv. Para ver los gráficos finales ejecutados en celda se puede revisar el archivo Análisis de métricas que utilizan estos mismo archivos guardados de la experimentación. 

# Proyecto book crossing

En este archivo se hacen experimentos con el dataset book-crossing. Estos experimentos utilizan la intensidad de carbono promedio en vez de CodeTracker para seguir el ejemplo del paper Benchmarking News Recommendation in the Era of Green AI de Qijiong Liu, et. al, ya que así se tenía planeado inicialmente. Para estos experimetnos solo se utilizó ALS, ya que book-crossing es un dataset muy disperso y para los modelos de deep learning, se obtenian resultados nulos. 

# Análisis de métricas

En este archivo se crean los gráficos de los datos para el análisis. Estos incluyen gráficos de métrica de calidad vs co2, correlaciones entre las eficiencias, métricas de calidad y emisiones de co2 y las intersecciones de las mejores eficiencias y la frontera de Pareto. Este archivo utiliza los archivos csv que se encuentran en el repositorio.  