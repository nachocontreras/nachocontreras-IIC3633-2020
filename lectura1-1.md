Item-Based Collaborative Filtering Recommendation Algorithms
===

En el contexto de los sitios web y la gran demanda que estos poseen, surge la necesidad de generar recomendaciones de calidad a millones de usuarios por sobre muchos items. De esto, los sistemas recomendadores basados en los items más que los usuarios pueden lograr separar las características de los usuarios y enfocarse más en que relaciona a los objetos. Así, en este _paper_ se habla sobre diversas técnicas para obtener estas similaridades y para recomendar.

A diferencia del filtrado colaborativo basado en usuarios o _user-based collaborative filtering_, algoritmo muy usado pero que trae problemas de escalabilidad, _scalability_, y calidad, _sparcity_, de las recomendaciones, los algoritmos basados en items no tienen que buscar dentro de los millones de usuarios sino que dentro de los miles de items. Haciendo más eficiente su cálculo.

Se presentan diversas maneras para calcular la similitud entre los items, tales como _cosine-based_, _correlation-based_ y _adjusted-cosine_. De estas se despeja el _weigthed sum_, que a propósito podría ser más clara la forma en que eligen que es un elemento similiar ya que se podría dar a entender que son _K_ elementos pero al no mostrarlo podrían ser también todos aquellos que tengan algún rating del usuario _u<sub>a</sub>_.

Me pareció interesante que además de considerar los ratings y las similitudes entre los items (que se pueden calcular de varias formas), consideraran la cantidad de vecinos a revisar pero de forma predefinida, debido a que uno podría pensar que a mayor cantidad de items a comparar se pueden obtener los mejores resultados pero tal como se señala en la figura 6, el menor MAE se desprende de un bajo número de vecinos.

Para trabajo futuro se podría realizar el mismo análisis pero sobre una base de datos que tenga un pequeño _sparcity level_, esto con el objetivo de saber si solo para aquellos casos donde el tamaño de la matriz es significativamente más grande que la cantidad de ratings el _item-based_ forma mejores recomendaciones que _user-based_.

Ignacio Contreras
