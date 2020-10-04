Ideas centrales para el mini resumen
- Usuarios quieren inspeccionar y controlar cómo sus relaciones sociales influyen las recomendaciones que reciben, ya que se basan en amigos más que en vecinos desconocidos.
- El razonamiento y visión en el proceso de un recsys expuesto por una interaz aumenta la capacidad of being inspected or publicly observed.
- step beyond existing work on social recommenders by explicitly testing the effect of leveraging users’ knowledge about their friends to improve inspectability and control. By allowing a user to inspect and control los elementos de control en los que se basan las recomendaciones.
- Se utiliza el sistema TasteWeights con algunas modificaciones que recomienda nuevos artistas y bandas basados en los likes de música del usuario y de sus amigos de Facebook.
- Se modifican los pesos propios o la similitud con los amigos. (control).
Challenges
- 
Puntos interesantes
- Se utiliza un recomendador de Facebook que entrega a los usuarios control sobre sus recomendaciones.
- Los pesos del modelo son calculados usando User KNN con Pearson correlation coefficient.
- Se le asigna el peso a todas las bandas/artistas que no ha escuchado el usuario. (Novedad)
- Both inspectability and control have a positive effect on the user experience, primarily because an inspectable and controllable recommender system is easier to understand. 
- In effect, the recommendation graph increases the understandability, perceived control, perceived recommendation quality, and system satisfaction.
Críticas
- Inspección y control aumenta la calidad de las clasificaciones (rating) y la satisfacción frente al sistema.
- Se consideran pesos positivos y probablemente, hubiese sido bueno evaluar la ponderación o peso negativo de los usuarios ya que inclina hacia otras recomendaciones más que aumentar levemente el peso de un item que el usuario no ha visto.

---

# Inspectability and Control in Social Recommenders

Hoy en día, las recomendaciones buscan tener un componente de explicabilidad y transparencia, debido a que saber de donde provienen las recomendaciones y cómo se relacionan con sus características o conocidos les permiten mejorar su toma de decisiones. De esta manera, en este paper se trabaja sobre la idea de que los usuarios quieren inspeccionar y controlar cómo sus relaciones sociales influyen las recomendaciones que reciben, ya que se basan en amigos más que en vecinos desconocidos.

Para esta investigación se utiliza un recomendador de Facebook, _TasteWeights_, que entrega a los usuarios control sobre sus recomendaciones. Este sistema entrega recomendaciones de música, artistas y bandas en relación al usuario y a sus conocidos. Además, se busca realizar un paso más en el trabajo existente sobre recomendadores sociales gracias al testeo explícito del efecto de saber que le gusta a tus amigos para mejorar la inspección y control del usuario. Esto se puede lograr gracias a la inspección y control de los elementos en que se basan las recomendaciones, como el peso del aporte de los usuarios y el peso de los items.

De esta manera, se presenta un modelo User KNN donde se modifica el peso de cada item, que afecta a la similitud con los otros items y también se modifica el peso de cada usuario, esto con el objetivo de hacer que usuarios aporten más en la recomendación que otros. Entonces, durante la investigación, se presenta la posibilidad de no hacer ningún cambio, de modificar los pesos propios o el de los amigos. Estas modificaciones se enfocan en el control del usuario. Las recomendaciones se presentan en forma de grafo o en lista.

Sin embargo, el coeficiente utilizado para obtener la similitud de los usuario se base en _Pearson Correlative Coefficient_. Yo creo que la utilización de pesos positivos, derivados de este coeficiente podría mejorarse si se evalúa utilizando también números negativos en la similitud. Esto debido a que la ponderación o peso negativo de los usuarios podría inclinar hacia otras recomendaciones más que aumentar levemente el peso de un item que el usuario no ha visto. Así, si dos usuarios son opuestos, sus gustos modificaría aún más la recomendación más que no aportan tanto en ellas (debido a que en Pearson sería casi 0), mientras que negativo podría ser, por ejemplo, -2. 

En conclusión, las recomendaciones buscan tener un componente de explicabilidad y transparencia. En este paper, se propone un sistema _TasteWeights_, que difiere de experimentos anteriores ya que ahora permite realizar modificaciones a los pesos de los items y de los usuarios. Se observa que el razonamiento y visión en el proceso de un sistema recomendador expuesto por una interaz aumenta la capacidad de inspección del usuario. Además, las recomendaciones en grafo aumentan el entendimiento, control percibido, calidad de las recomendaciones percibidas y la satisfacción del sistema. Esta idea surge a partir de las técnicas SVD utilizadas por Wei Xu, Xin Liu, y Yihong Gong en 2003.

Por otro lado, podría existir la posibilidad de utilizar similitudes negativas como un efecto que disminuye la valoración de un item. Esto debido a que los items musicales no solo se componen de atributos positivos sino que podrían entregar atributos negativos que mejoren la explicación de la recomendación.

Ignacio Contreras


Referencias

Wei Xu, Xin Liu, and Yihong Gong. 2003. Document clustering based on non-negative matrix factorization. In Proceedings of the 26th annual international ACM SIGIR conference on Research and development in informaion retrieval (SIGIR '03). Association for Computing Machinery, New York, NY, USA, 267–273. DOI:https://doi.org/10.1145/860435.860485