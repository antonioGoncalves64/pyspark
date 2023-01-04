<img src="spark.png" alt="drawing" width="300"/>

## Análise de Rating de filmes


<a target="_blank" href="https://colab.research.google.com/github/antonioGoncalves64/pyspark/blob/main/LabPySpark-ratings-counter.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>



Pretendemos obter um resumo das classificações de filmes a partir do ficheiro (ratings.csv) que contem milhares de dados de classificações de filmes.  O ficheiro **ratings.csv**  está disponível para consulta em [movielens](https://grouplens.org/datasets/movielens/) e é composto por um conjunto de dados e que contém a  25 milhões de classificações realizadas a 62.000 filmes por 162.000 utilizadores. Onde cada linha representa o números de filmes que forma classificados com um dado valor.

## Formatação e Codificação


O ficheiro do conjunto de dados é escrito como um ficheiro de valores separados por vírgulas com uma única linha de cabeçalho. Estes ficheiros são codificados como UTF-8. Se os caracteres acentuados em títulos de filmes  (por exemplo, Misérables, Les (1995)) forem apresentados incorrectamente, certifique-se de que qualquer programa que leia os dados, como um editor de texto, terminal, ou script, está configurado para UTF-8.

* **Ids do utilizador.** Os utilizadores de MovieLens foram seleccionados ao acaso para inclusão. Os seus identificadores foram anonimizados. 

* **Ids de filmes.** Só estão incluídos no conjunto de dados filmes com pelo menos uma classificação ou etiqueta. Estes ids de filmes são consistentes com os utilizados no sítio web do MovieLens (por exemplo, id 1 corresponde ao URL https://movielens.org/movies/1).

* **Classificações dos filmes.** Todas as classificações estão contidas no ficheiro **ratings.csv**. Este ficheiro possui uma linha de cabeçalho seguido de vários registo de  rating dispostos em linha. Cada registo  tem o seguinte formato: **id do utilizador, id de filme, classificações (rating), carimbos temporais (timestamp).** As classificações (rating)  são feitas numa escala de 5 estrelas, com incrementos de meia estrela (0,5 estrelas - 5,0 estrelas). Os carimbos temporais representam segundos desde a meia-noite do Tempo Universal Coordenado (UTC) de 1 de Janeiro de 1970.


## Trabalho a ser realizado

A partir dos registo de votações contidas no ficheiro **ratings.csv** pretendemos no final obter um histograma, também conhecido como distribuição de frequências, dos ratings totais. Em seguida é apresentado um exemplo.

* 0.5, 18408
* 1.0, 40233
* 1.5, 21566
* 2.0, 85616
* 2.5, 65307
* 3.0, 256838
* 3.5, 164152
* 4.0, 349862
* 4.5, 113879
* 5.0, 556793




 


   
   