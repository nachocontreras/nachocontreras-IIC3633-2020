Ideas centrales para el mini resumen
- This article aims to provide a comprehensive review of recent research eorts on deep learning based recommender systems. More concretely, we provide and devise a taxonomy of deep learning based recommendation models, along with providing a comprehensive
summary of the state-of-the-art.
- However, there is a lack of extensive review on deep learning based recommender system. The goal of this survey is to thoroughly review literature on the advances of deep learning based recommender system

- RNNs are extremely suitable for sequential data processing. As such, it becomes a natural choice for dealing with the temporal dynamics of interactions and sequential paerns of user behaviours, as well as side information with sequential signals, such as texts, audio, etc. Como GRU4REC . indicated that simple neighbourhood approach could achieve same accuracy results as GRU4Rec.

- Restricted Boltzmann Machine based Recommendation

- Neural Attention based Recommendation: illtering out the uninformative features from raw inputs and reduce the side eects of noisy data.

- Neural AutoRegressive based Recommendation: tractable distribution estimator which provides a desirable alternative to RBM. Ideally, the order of movies should follow the time-stamps of ratings.

- Deep Reinforcement Learning for Recommendation
Most recommendation models consider the recommendation process as a static process, which makes it dicult to capture user’s temporal intentions and to respond in a timely manner.(1) dynamic changes of news content and user preference; (2) incorporating return paerns (to the service) of users; (3) increase diversity of recommendations.

- Adversarial Network based Recommendation: process between documents and queries, and retrieval tasks can be achieved by generating relevant document d given a query q. Se hace un mix max entre documentos relevantes y no relevantes.

- Deep Hybrid Models: Mezcla

Trabajo futuro:
- Explainable Recommendatio. e rst, is to make explainable predictions to users, allowing them to understand the factors behind the network’s recommendationsn
- Hay mas

conclusion:
this article, we provided an extensive review of the most notable works to date on deep learning based
recommender systems. We proposed a classication scheme for organizing and clustering existing publications,
and highlighted a bunch of inuential research prototypes. We also discussed the advantages/disadvantages of
using deep learning techniques for recommendation tasks

Critica:
 veo que siempre se busca "Making accurate recommendations requires deep understanding of item characteristics and user’s actual demands
and preferences".

Puntos interesantes
- In recent years, deep learning has garnered considerable interest in many research elds such as computer vision and natural language processing, owing not only to stellar performance but also the aractive property of learning feature representations from scratch.
- Deep learning is able to eectively capture the non-linear and non-trivial user-item relationships, and enable the codification of more complex abstractions as data representations in the higher layers

--- 
# Deep Learning based Recommender System: A Survey and New Perspectives