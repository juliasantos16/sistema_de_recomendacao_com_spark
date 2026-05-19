# Sistema de recomendação com Spark

Nesse projeto, desenvolvi um sistema de recomendação de músicas usando Spark, unindo análise de dados, machine learning e integração com a API do Spotify. A ideia era criar algo parecido com os sistemas de recomendação das plataformas de streaming, capaz de encontrar músicas semelhantes com base nas características sonoras de cada faixa.

No início do projeto, utilizei o PCA para reduzir os dados para apenas duas componentes principais. O objetivo dessa etapa era principalmente visual.
Mas, como a escolha da quantidade de componentes influencia diretamente na qualidade da clusterização e das recomendações, não mantive apenas duas dimensões no modelo final. 
Depois dessa análise inicial, utilizei PCA para identificar a quantidade ideal de componentes que preservasse o máximo possível das informações importantes das músicas.

Essa etapa foi essencial para reduzir a complexidade dos dados sem perder qualidade, deixando o algoritmo K-Means mais eficiente e melhorando significativamente a precisão das recomendações geradas pelo sistema.


###  Algoritmos e Técnicas:
Standard Scaler: Aplicado no pipeline para padronizar os dados e garantir que todas as features musicais ficassem na mesma escala  

PCA (Principal Component Analysis): Utilizado para a redução de dimensionalidade dos dados.  

K-Means: Algoritmo de clusterização onde foi criado os agrupamentos de músicas baseados em suas características  

Distância Euclidiana: Técnica matemática implementada para calcular a distância entre a música de referência do usuário e as demais faixas do mesmo cluster, permitindo retornar o top 10 de músicas mais próximas

link para obter a API do spotify: https://developer.spotify.com/dashboard/login
