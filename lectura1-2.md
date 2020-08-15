FunkSVD
===

Desde el 2007 al 2009 se realizó el *Netflix price*, una competencia en la que se buscaba encontrar el mejor sistema recomendador para predecir cuál será el rating que realizará un usuario específico para cierta película en el futuro. Esta predicción debe lograrse a partir de 100 millones de datos de la forma (user, movie, rating, timestamp) que muestran el rating entregado por 500K usuarios a 17k películas.

De esta manera, Funk explica como a lo largo de ese tiempo desarrolló, junto a su equipo, un sistema recomendador capaz de llegar al tercer lugar en el concurso.

En el blog se explica las etapas por la que pasó el desarrollo para poder obtener el sistema recomendador que se acercaba mucho al ganador pero no generaba mayor diferencia. Así, se comenzó utilizando SVD (_Singular Value Descomposition_) en la que se disminuye la cantidad de variables a utilizar, a partir de los pesos que se le asignan a las variables, como las características de las películas o de los usuarios, a otras de mayor utilidad, como errores cuadráticos medios, promedios de _ratings_, entre otras variables. Esto se realiza debido a la enorme cantidad de 8.500 millones de entradas en una matriz de ratings, que en la mayoría son nulos.

Dentro de las cosas que me parecieron interesantes es que el _averageRating_ utilizado para realizar la predicción no era una media normal sino que dependía de la cantidad de _ratings_ realizados para esa película. Por ejemplo, una película con 1 solo rating no tiene su promedio igual al _rating_, lo que favorece la implementación y no segmenta los datos o los inclina a los extremos (_BetterMean_).

Un inconveniente que vi es que si un usuario no posee una gran cantidad de ratings entonces sus apreciaciones sobre los 40 factores de las películas podría no ser el adecuado y afectar considerablemente los pesos y el rating esperado para una película en particular. Pero, por otro lado, si hay ratings para el usuario, se puede extraer sus "gustos" y mejorar la predicción.

Ignacio Contreras