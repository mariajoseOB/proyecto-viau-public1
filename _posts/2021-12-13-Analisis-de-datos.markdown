---
layout: post
tittle: "Análisis de datos"
date: 2021-12-13 15:34:36 +0530
---

Luego de realizar el análisis exploratorio decidimos añadir métodos de clustering para nuestra investigación, no obstante, tuvimos algunos inconvenientes, ya que la mayoría de nuestros datos eran de tipo categórico, por lo que no podíamos hacer uso de **K-Means**, así que siguiendo los consejos de nuestra profesora e investigando sobre K-Modes logramos realizar el análisis con clustering, para poder analizar correctamente los resultados decidimos usar gráficos de barras con las distintas variables. Para una explicación sencilla y paso a paso de este algoritmo, consultar [aquí](https://www.analyticsvidhya.com/blog/2021/06/kmodes-clustering-algorithm-for-categorical-data/)

{% include clusters_consultas_cat.html %}

Para empezar, notamos que el mayor porcentaje de **heavy_user** estaba presente en el cluster 1, además de ser este último el que menor porcentaje de **not_a_user** tenía, esto lo hace un cluster muy interesante para centrar nuestra investigación. Para empezar nuestro análisis de cluster, vimos cómo era la distribución de los géneros en cada cluster. Los cluster 0, 1 y 3 presentaban una distribución bastante similar, sin embargo, el cluster 2 tenía un porcentaje mucho mayor de hombres que de mujeres, curiosamente también es uno de los que presenta mayor pocertaje de **not_a_user**. Otro dato interesante fue que el cluster 1 contenía 1/5 de las mujeres totales, mientras que el cluster 2 contenía el 32% de los hombres.

{% include sexo_cluster.html %}

A continuación, quisimos ver la relevancia que tenía el tipo de contrato en cada cluster, pero no hayamos nada relevante para nuestro estudio.

{% include tipo_de_contrato_cluster.html %}

 Analizando los clusters por profesión, dimos con que el cluster 1 estaba mayormente compuesto por enfermero(a)s y matrone(a)s, el cluster 2 tenía mayor porcentaje de TENS y Kinesiólogo(a)s. Además, el cluster 2 contenía al 89% de los médicos, siendo este grupo de profesionales uno bastante numeroso.

{% include profesion_cluster.html %}

 Por otro lado, quisismos analizar que profesión le aportaba mayor cantidad de **heavy_user** a cada cluster y con esto conseguimos ver que en el cluster 0 la mayoría de **heavy_user** está constituido por médicos con un 63,1%, por el contrario, al cluster 1, que sus **heavy_user** están mayormente compuestos por enfermero(a)s y matrone(a)s. En el resto de cluster no se pueden sacar muchas conclusiones, porque son un grupo muy pequeño de **heavy_user**.

{% include profesion-heavy.html %}

Depués, nos pareció interesante ver qué rango etario componía mayormente el clluster 1, el gráfico nos reveló que el 56% de los profesionales que pertenecen al cluster 1 tienen un rango de edad entre 40-50 años. Pero también notamos que el 35% de las personas pertenecientes al rango 40-50 están en el cluster 0, siendo este último uno con buen uso de la plataforma, por lo que se podría deducir que las personas entre 40 y 50 años hacen un buen uso del VIAU.

{% include edad_cat_cluster.html %}

Finalmente, la última variable consideramos de importancia fue la comuna en la que trabajan los profesionales, lo cual nos reveló que el cluster 1 estaba compuesto mayoritariamente por gente de La Pintana, otra cosa interesante fue que los profesionales de La Pintana se repartían entre el cluster 0 y 1, siendo estos los que más usan la plataforma.

{% include nombre_comuna.html %}

Sin embargo, en el cluster 0 la mayor cantidad de **heavy_user** pertenece a La Florida.

{% include nombre_comuna-heavy.html %}
