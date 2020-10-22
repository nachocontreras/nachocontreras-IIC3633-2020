Ideas centrales para el mini resumen
- This article aims to provide a comprehensive review of recent research eorts on deep learning based recommender systems. More concretely, we provide and devise a taxonomy of deep learning based recommendation models, along with providing a comprehensive
summary of the state-of-the-art.
- However, there is a lack of extensive review on deep learning based recommender system. The goal of this survey is to thoroughly review literature on the advances of deep learning based recommender system
- Neural architectures have demonstrated tremendous success in both supervised and unsupervised learning tasks. Dentro de estas se mencionan algunas con su explicación.
- recapitulate, we summarize the strengths of deep learning based recommendation models that readers might bear in mind when try to employ them for practice use (ver ejemplos de esa frase)
- Limitaciones (ver ejemplos)
Puntos interesantes
- In recent years, deep learning has garnered considerable interest in many research elds such as computer vision and natural language processing, owing not only to stellar performance but also the aractive property of learning feature representations from scratch.
- Deep learning is able to eectively capture the non-linear and non-trivial user-item relationships, and enable the codification of more complex abstractions as data representations in the higher layers
- of the most atractive properties of neural architectures is that they are (1) end-to-end dierentiable and (2) provide suitable inductive biases catered to the input data type.
- Tipos de deep leraning, con bloques neuronales e híbrido
- Tambien estan los multilayer perceptron, recomendaciones basadas en eso.
- there exist two general ways of applying autoencoder to recommender system: (1) using autoencoder to learn lower-dimensional feature representations at the boleneck layer; or (2) lling the blanks of the interaction matrix directly in the reconstruction layer
- Convolution Neural Networks are powerful in processing unstructured multimedia data with convolution and pool operations. Most of the CNNs based recommendation models utilize CNNs for feature extraction.

--- 
# Deep Learning based Recommender System: A Survey and New Perspectives

Durante las últimas décadas se han realizado grandes esfuerzos e investigaciones en el área de los sistemas de recomendación. Sin embargo, no hace mucho tiempo, los sistemas basados en aprendizaje profundo fueron tomando importancia debido a la habilidad o oportunidad que entregan estos mecanismos para encontrar características y patrones en los datos entregados. 

Este paper tiene como objetivo proveer un análisis detallado de la investigación reciente entorno a los sistemas recomendadores basados en deep learnig, para abreviar _RecSysDL_. Así se presentan durante el desarrollo del artículo características de estos sistemas y herramientas como algortimos en el estado del arte.

Tal como se señaló anteriomente, las redes neuronales, componente fundamental del aprendizaje profundo, puede capturar caractarísticas no lineales ni triviales sobre las relaciones entre la información, por ejmplo, relaciones usuario-items. Este es un beneficio considerable ya que permite abstraer la representación de la información a capas más altas de procesamiento. Lo que además, permite enfocarse en la utilidad y objetivo del modelo entrenado más que en como la información se interrelaciona.

De esta manera, vemos que las redes neuronales comprenden dos tipos: con bloques neuronales o híbridos. El primero, corresponde a redes donde sus componentes llamados "bloques" tienen funciones que extraen infromación y relaciónes en la data y que son utilzadas para agrupar ponderaciones y/o asignar pesos a las conexiones entre los mismos bloques. Por ejemplo, los AutoEncoder tienen componentes característicos que permiten, asociar un origen con el destino de a través de un intermediario y los CNN, permiten extraer múltiples capas de _data_ basados en la información original.
Por otro lado, las redes híbridas tienen el objetivo o la característica de utilizar varias redes neuronales de forma conjunta para complementarse y así generar un modelo con mejores métricas.

También, durante el paper se señalan diversos ejemplos sobre el uso de estos sistemas en la vida diara. Por ejemplo, . En este caso, vemos como el RecSysDL permite 

Sin embargo, las redes neuronales tienen limitaciones que pueden afectar su desempeño y utilidad en la recomendación.

En conclusión, el aprendizaje profundo es una zona nueva de investigación que tiene una gran utilidad en diversas áreas, como salud, transporte, educación y en este caso, para la recomendación. Así, en este paper se presentan características de las redes neuronales como los diferentes tipos que existen, sus componentes, sus limitaciones y ejemplos de uso. Gracias al trabajo de estos investigadores se pueden resumir y agrupar varias investigaciones dentro de estas divisiones, permitiendo un mayor entendimiento de las redes neuronales y de su prometedor futuro como base para los sistemas de recomendación.

Ignacio Contreras