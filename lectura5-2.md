Ideas centrales para el mini resumen
- Se combinan diversos CF algoritmos para poder obtener uno mejor. Se llama ensembled method.
- La mejor combinación dfue de componentes lineales.
- 
Challenges
- 
Puntos interesantes
- Que fueran uno por uno aclarando las caracteristicas del modelo.
- We note here that the individual algorithms in the ensemble were trained on the original training set, i.e. the whole dataset excluding the probe set. However, the training of the blending algorithm was done on the pTrain set, i.e., one half of the probe set.
- Se revisan distintos metodos para encontrar combinaciones de modelos.
- 
Críticas
- 

---

# Combining Predictions for Accurate Recommender Systems

Hoy en día, existe una gran diversidad de algoritmos para entregar recomendaciones a los usuarios en base a información implícita y explícita. Estos algoritmos funcionan bien dependiendo del contexto y la información que se les entrega. Por ejemplo, un collaborative filtering item-item tiene métricas adecuadas cuando existen interacciones entre los usuarios y los items, como ratings. Sin embargo, los resultados pueden ser mejorados cuando se combinan diversos algortimos, lo que se llama _ensembled model_.

En este paper, se combinan diversos algorimos CF para poder obtener uno con métricas superiores. Dentro de los modelos analizados se encuentran KNN item-item, KNN user-user, SVD de factores latentes, AFM (_Asymmetric factor model_), RBM (_Restricted Boltzmann Machine_), GE de factores globales.

En primer lugar, me pareció interesante la metodología para testear los modelos y el consecuente _ensembled model_. En este caso, los modelos individuales son entrenados con el _dataset_ de entrenamiento original, sin considerar la separación para _test_. Sin embargo, el entrenamiento de la combinación se realiza utilizando una partición del _dataset_ del test que se dividió en dos para finalmente realizar el _test_ final con los elementos restantes.

En segundo lugar, el análisis individual de los modelos entrega un entendimiento más completo de los parámetros utilizados y el objetivo inicial de la creación de los modelos. Así, se puede entender la razón de porque SVD y sus especificaciones son las que aportan mayor peso al valor final de la recomendación. Creo que se puede deber al hecho de utilizar factores latentes optimizados para relacionar las características entre los items y los usuarios mejora la recomendación ya que se abstrae el item en particular y se condiciona a la interacción con los demás elementos y usuarios.

Si analizamos el método de combinación de los algoritmos se puede observar que se prioriza el método lineal de ponderación de los distintos modelos. Sin embargo, se explica esto a partir de los resultados obtenidos y se generaliza a partir del caso de estudio. Por esto, cabe recalcar que la metodología de ensable de modelos se tiene que definir luego de iterar sobre varios tipos de combinaciones. En consecuencia, dado un caso en particular se debe entrenar los modelos considerando múltiples metodologías como la lineal, convolucional, no lineal, entre otras.

Además, la selección del modelo lineal se puede deber a que, desde el punto de vista de la economía, la combinación lineal de modelos que pueden disminuir la varianza de su predicción y por ende, mejorar la exactitud en la precisión. Esto se puede relacionar con la rentabilidad esperada dado sus varianzas.

En conclusión, el paper analizado busca encontrar la mejor combinación de modelos de CF para un caso de interacciones con ratings. Así, se explican los diversos modelos utilizados como también la metodología para testear al algoritmo en particular y su _ensembled model_. Además, se observa que se prefirió el método lineal de combinación donde el SVD prioriza en peso de recomendación. Y finalmente, se da un enfoque sobre el por qué el método lineal pudo haber entregado resultados eficientes debido a la combinación lineal de sus elementos y la diminución de la varianza.