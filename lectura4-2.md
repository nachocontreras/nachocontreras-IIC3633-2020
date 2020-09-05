# Document Clustering Based On Non-negative Matrix Factorization

En este paper se propone una nueva metodología para realizar clasificación de documentos (items con texto) basados en la factorización no negativa de los términos en forma de matriz, asemejando a una ponderación de tópicos que crean el documento en vez de sma y resta de pesos como lo hace SVD. Además, con una buen algoritmo de clasificación de documentos, los computadores puede organizar un documento como una ordenamiento jerárquico de los tópicos en él, permitiendo una eficiente bpusqueda y entendimiento de los tópicos que componen al item.

Durante la lectura pude notar algunos hechos interesantes. En primer lugar, investigaciones recientes han mostrado que la clasificación utilizando grafos no dirigidos, como forma de relacionar a los items, ha permitido realizar comparaciones entre los items de forma eficiente. 

En segundo lugar, la nueva metodología propone la factorización para cada documento de forma de obtener las proyecciones para cada tópico a evaluar. Así, luego se proyecta hacia los K tópicos de mayor importancia, obteniendo la representación del documento. Esto en particular es una gran diferencia con SVD que puede tener proyecciones negativas y no *human readable*, permitiendo entender y analizar de mejor manera la configuración y representación de los documentos.

Algo que me llamó la atención, en el contexto del entrenamiento para encontrar los mejores parámetros para clasificar los documentos, es el hecho de que, probablemente, remover los documentos con varios labels haga que si se quiere revisar el cluster de un documento variado se obtengan resultados sesgados hacia un tipo de tópico. Los documentos tienen muchos tópicos y como se ve en el dataset de TDT2, casi 56000 documentos no fueron utilizados debido a esto.

En conclusión, se propone una nueva metodología de factorización no negativa para poder clasificar documentos en base a su tópico. Además, en comparación con los algoritmos actuales como SVD, se evita tener representaciones latentes de los factores y se genera un entendimiento *human readable* sobre la representación de los items y su contenido.

Ignacio Contreras

