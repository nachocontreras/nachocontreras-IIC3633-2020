Ideas centrales para el mini resumen
- However, selecting the most relevant items (albums, artists, playlists...) to display in these carousels is a challenging task, as items are numerous and as users have different preferences.
- In this paper, we model carousel personalization as a contextual multi-armed bandit problem with multiple plays, cascade-based updates and delayed batch feedback
- our proposed framework,
- Throughout this paper, the K arms will correspond to a list of K cards/items, such as a catalog of albums or playlists in a music streaming app.
- Cada vez que se revisa o clickea una tarjeta dentro de las L que se pueden ver se le asigna un valor 1 con una probabilidad p. Esto hace referencia a las tarjetas que el usuario tiene interés. El usuario no puede ver todas las tarjetas y tampoco se sabe exactamente cuales se ven. Entonces se puede considerar que las tarjetas presentadas no son de interés del usuario pero si pide más significa que vió hasta el máximo de tarjetas entregadas.
- Se realizó un experimento offline luego un online A/B test para validar los resultados del experimento offline.
- El offline, SVD KNN.
- superiority of the proposed multi-armed bandit framework for personalization
Challenges
- 
Puntos interesantes
- user feedback to adaptively improve the recommended content via online learning strategies.
- Semi-Personalization via User Clustering: app, users from a same group would have homogeneous musical tastes. Aunque sea más rápido depende de la calidad del los clusters.
- Contextual Multi-Armed Bandits: Semejante al SVD con factores latentes. vectors aim at summarizing user preferences on the platform, e.g. their musical tastes
- algoritmo ts-seg-pessimistic. method manages to effectively exploit information and to quickly rank playlists,
Críticas
- 
---

# Carousel Personalization in Music Streaming Apps with Contextual Bandits