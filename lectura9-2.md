Ideas centrales para el mini resumen
- Sophisticated approaches have been developed to automatically optimize the ensembles’ configura-tion to maximize their performance gains.
- evolve, the performance of previ-ously well-behaved algorithms may degrade and hamper the en-semble effectiveness –or weaknesses may simply surface that had gone unnoticed in the selection phase
- https://www.offerzen.com/blog/how-to-build-a-product-recommender-using-multi-armed-bandit-algorithms
- Thompson sampling: action that maximizes the expected reward with respect to a randomly drawn belief.
- e-greedy: The reasoning behind this approach is that for a portion of the time the algorithm randomly explores the available actions, but it still exploits the best action the majority of the time
- multi-armed bandit techniques: 
    - They can recommend products with the highest expected value while still exploring other products.
    - They do not suffer from the cold-start problem and therefore don’t require customer preferences or information about products.
- algorithms based on their previous performance. If one recommendation algorithm is clearly less effective than the oth-ers, the bandit ensemble will progressively reduce the traffic it is assigned.
- We have explored the incorporation of multi-armed bandit techniques to the design of dynamic recommender ensembles that select the best among several algorithms based on the previous performance of each candidate.
Challenges
- building ensembles lies in properly tuning the contribution of the combined algorithms to the aggre-gated output.
Puntos interesantes
- large part of the system’s input is collected from the reaction of users to the recommendations they are delivered.
Críticas
- In our experiments, we will select target users in a loop over all users, and update the arms after each such round.
- that each recommender system has its own training, test and exclusion sets, since they are built from the user feedback to their own specific recommendations 
---

# Multi-Armed Recommender System Bandit Ensembles
