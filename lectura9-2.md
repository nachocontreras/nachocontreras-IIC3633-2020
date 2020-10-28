# Multi-Armed Recommender System Bandit Ensembles

En los últimos años se han realizado varios aportes relacionados al área de los sistemas recomendadores, en específico sobre los ensambles de modelos de recomendación. Esto se ha realizado para poder obtener precisiones y _recalls_ elevados, mientras se mantiene alta la satisfacción del usuario. Sin embargo, para poder entregar recomendaciones basadas en múltiples modelos el ensamble no es la única opción.

En este paper se desarrolla un acercamiento sofisticado en cuanto a la automatización de la optimización de un sistema recomendador basado en múltiples brazos o sub modelos. Esto con el objetivo de maximizar las ganancias del sistema rápidamente, en términos de relevancia para el usuario y su interacción positiva con el sistema (ej. clicks). Esta investigación surge a partir de la idea de que los sistemas recomendadores se evaluan de forma _offline_ y _online_ principalmente, pero cuando es _online_ solo se realiza una iteración sobre las recomendaciones y no se revisa como el sistema recomendador evoluciona frente a las interacciones del usuario. Por ejemplo, en un primer lugar las recomendaciones podrían ser atingentes al usuario pero a medida que puede usar la herramienta o el sistema su enfoque podría modificar y por ende las recomendaciones debiesen seguir ese enfoque.

De esta manera, para poder evaluar esta nueva implementación se propuso la incorporación de un banda de modelos que entregan recomendaciones en un carrusel. Lo importante acá es que los algoritmos utilizados debiesen capturar el desempeño anterior del modelo para poder ir mejorando o prefiriendo otros modelos en la recomendación siguiente. Así, surge el desafío de construir un ensamble de modelos basados en la modificación de la contribución combinada de algoritmos para obtener el desempeño característico de cada uno. 

La información utilizada para desarrollar el algoritmo de desempeños se basa en infromación recolectada a partir de las reacciones de los usuarios a las recomendaciones que reciben. Algunos algoritmos que se presentan son _Thompson sampling_ y _e-greedy_. El primer algoritmo busca maximizar la recompensa generada por la elección de una recomendación frente a las demás basado en que se debe mostrar recomendaciones útiles y populares para el usuario como también explorar más alla. El segundo algoritmo, busca explorar recomendaciones aleatorias durante un tiempo mientras también entrega las recomendaciones más útiles para el usuario.

En conclusión, en este paper se presentan algoritmos y su aplicación para realizar un ensamble de sistemas recomendadores basado en la idea de _multi-armed recommender system_ que muestra varios sistemas recomendadores y el usuario elige cual prefiere. En este caso, se diferencia de propuestas anteriores debido a que considera en tiempo real la interacción con el usuario para siguientes recomendaciones enfocándose en mantener un desempeño actual y futuro adecuado. Así, el sistema recomendador no se queda con solo una iteración de recomendaciones sino que va modificando su actuar y el de los demás modelos en base a las recomendaciones que ya se han entregado, las características del usuario y sus interacciones.

Este sistema permite evaluar modelos de forma conjunta y priorizar aquellos que frente a las elecciones iterativas de los usuarios van siendo los mejores desde el punto de vista de la relevancia, utilidad para el individuo. Este tipo de herramienta, en un caso hipotético, podría ser utilizado en sectores donde las características medioambientales permiten cierto tipo de construcciones y se puede tener varios modelos que a partir de estas características recomienden métodos de construcción y/o materiales para ello. Así, mientras se va utilizando el sistema se va enfocando en un modelo en específico más relacionado con el usuario y así, hacer una construcción para el usuario. Podría ser un punto interesante de investigación relacionada a la construcción o sus derivados.


Ignacio Contreras