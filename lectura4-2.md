Ideas centrales para el mini resumen
- propose a novel document clustering method based on the non-negative factorization of the termdocument matrix of the given document corpus.
- With a good document clustering method, computers can automatically organize a document corpus into a meaningful cluster hierarchy, which enables an efficient browsing and navigation of the document corpus.
- Topic Detection Tracking (TDT)
Challenges
- 
Puntos interesantes
- Recent jobs, (clustering) these methods model the given document set using a undirected graph in which each node represents a document, and each edge (i, j) is assigned a weight wij to reflect the similarity between documents i and j.
- Se hace una proyección a K topicos para representar el documento.
- Diferencia NMF vs SVD
    - SVD toma negativos y el otro no, haciendo como suma de topicos y no restas, es mas entendible
    -  
Críticas
- Probablemente remover los documentos con varios labels haga que si se quiere revisar el cluster de un documento variado se obtengan resultados sesgados hacia un tipo de topico. Los documentos tienen muchos tópicos y como se ve en el dataset de TDT2, casi 56000 documentos no fueron utilizados debido a esto.


---
# Document Clustering Based On Non-negative Matrix Factorization
