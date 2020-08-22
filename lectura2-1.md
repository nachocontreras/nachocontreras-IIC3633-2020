Collaborative Filtering for Implicit Feedback Datasets
===

En este paper se busca analiza un sistema recomendador basado en información implícita del comportamiento de los usuarios en base a programas de televisión. En este caso, se proponen las características fundamentales de los *datasets* de *feedback* implícito. En particular, este tipo de *datasets* no contiene información negativa de los items en base a los usuarios, sino que representan positividad al ser utilizados, vistos, adquiridos los items y los no usados pueden ser o neutros o negativos, por lo que para su recomendación no se consideran.

Para el modelo a utilizar se considera $r_{ui}$ como la variable de confianza que determina si un item tiene prioridad para un usuario $u$. Además, se considera en la implementación un factor $c_{ui}$ que incrementa la importancia o interés por los items separando aquellos que son utilizados en menor medida. Y por último, se utiliza un modelo de factores latentes para representar la interacción entre usuario e item basados en la similaridad entre los items.

Podría ser interesante evaluar la implementación de este modelo en los cursos online ya que de la misma forma que se extrae la información de cuánto se ha visto un programa de tv se puede obtener cuánto es el interés de las personas por diversas clases. Además, utilizando factores de latencia y un *content-based approach* se podría recomendar con *feedback* implícito las mejores clases para que un usuario activo pueda seguir estudiando. Hasta, en base a los cursos que ya ha visto, se podrían recomendar tutoriales o profundización para seguir mejorando.

Además, considerando la forma en que se obtiene el peso $r_{ui}$ para los programa de TV, demás que podría considerarse un factor de normalización que aumente el tiempo de visualización de un programa largo vs un programa corto. Porque no es lo mismo ver 5 min de una serie de 20min que 5 min de una película. Yo creo que eso podría haberse mejorado para evitar una tendencia a los programar más cortos.

Ignacio Contreras.

