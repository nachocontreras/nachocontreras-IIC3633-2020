# Performance of Recommender Algorithms of Top-N Recommendation Tasks

En este paper se propone una nueva metodología para encontrar y mejorar los resultados obtenidos para la recomendación de Top-N.
El top-N es, como hace referencia su nombre, los mejores N items que son recomendados para un usuario. De esta manera, y a partir de la idea de que no se muestra el rating predicho a los usuarios se puede derivar un nuevo método.

Esta investigación nace luego de que se observe que reslutados que mejoran el RMSE no necesariamente se traducen en mejoras en la exactitud de la predicción. Por ende, se piensan en diversas formas para progresar en la recomendación de los Top-N. Así, se propone que el test para probar los resultados se defina cautelosamente en vía de evitar sesgo debido a las generalidades de los usuario e items como el Most Popular por ejemplo.

Esta nueva metodología consiste en utilizar como test solo items con ratings de 5 estrellas. Esto con el objetivo de mostrar si la recomendación entregada para un usuario u es realmente basada en la personalización de u o si está influenciada por las generalidades. De esta manera, para cada predicción que obtenga 5 de rating se extraen 1000 items no recomendados para el usuario y se ranquean los 1001 elementos. Si es que el item original está dentro de los N mejores entoces se obtuvo un hit. Si no, se obtuvo un miss.

Sin embargo, al parecer no se señala de donde se obtienen estos 1000 elementos. Esto surge un problema si es que los 1000 elementos tienen al menos N ratings 5. Si es que hay N items que cumplen con este criterio entonces existe la probabilidad de que el item no esté dentro del Top-N, obteniendo un miss. Probablemente estos 1000 elementos se tengan que extraer de un subconjunto de items que no tengan evaluación existente de 5. Si es que estos items adquieren una evaluación de 5 es que el sistema no está recomendando como debería.

En conlusión, el sistema propuesto modifica la métrica y la forma de obtener el dataset para testear, con el objetivo de mejorar los resultados obtenidos por la recomendación del Top-N.