---
layout: post
tittle: "Análisis exploratorio"
date: 2021-12-13 15:36:36 +0530
---
Con el análisis exploratorio pudimos responder las siguientes preguntas:

- **Según el tipo de contrato de los profesionales. ¿Quiénes hacen mayor uso del VIAU?**

Lo primero que notamos fue que la mayoría de los profesionales tiene un contrato de tipo *Plazo fijo*, estos tienen el mayor número de consultas como se puede visualizar en el gráfico, no obstante, es de esperarse ya que son los que más tiempo pasan con la plataforma. Por otro lado, podemos notar que los profesionales con contrato de tipo *Reemplazo* tienen el porcentaje más alto de *not_a_user*, esto se puede deber a que no se han podido familiarizar bien con la plataforma en el tiempo que estuvieron como reemplazo. Finalmente, los profesionales con contrato *Indefinido* tienen un uso bastante similar al de los con contrato *Plazo fijo*.

{% include tipo_de_contrato-freq.html %}
{% include tipo_de_contrato.html %}

- **Según el tipo de jornada de los profesionales. ¿Quiénes son los que más visitan el VIAU?**

Al ver el primer gráfico podemos notar que hay una gran diferencia entre el número de consultas de los profesionales con jornada mayor a 40 horas semanales a comparación del resto, no obstante, si uno profundiza en el análisis puede ver que las categorías de las consultas se distribuyen de manera bastante uniforme, es decir, que independiente al tiempo jornada que tengan los profesionales, el uso del VIAU es similar.

{% include jornada_cat-freq.html %}
{% include jornada_cat.html %}

- **Según la profesión. ¿Quiénes usan más el VIAU?**

Analizando los resultados del gráfico podemos ver que los médicos y los(as) matrones(as) tienden a hacer un uso más alto de la plataforma, además tienen un bajo procentaje de *not_a_user*, por lo que se puede inferir que entienden mejor el funcionamiento de la plataforma o sus actividades laborales tienen una mayor dependencia del VIAU.

{% raw %}{% include profesion-freq.html %}{% endraw %}
{% raw %}{% include profesion.html %}{% endraw %}


- **¿Qué género hace mayor uso del VIAU?**

Al comparar el número de consultas entre ambos géneros notamos que las mujeres tienen un número mucho mayor de consultas, pero al comparar con mayor profundidad podemos ver que ambos tienen un uso bastante similar en lo que se refiere al tiempo que la utiliza cada profesional.

{% include sexo-freq.html %}
{% include sexo.html %}

- **¿Qué tipo de establecimiento hace mayor uso del VIAU?**

El consultorio general urbano es el que presenta mayor número de consultas, con mucha diferencia, pero en el segundo gráfico podemos notar que el consultorio general rural tiene un mayor porcentaje de *heavy_user*.

{% include tipo_establecimiento-freq.html %}
{% include tipo_establecimiento.html %}

- **¿Qué grupo etario hace mayor uso del VIAU?**

El grupo etario con mayor volumen de consultas es ***30-40***, no obstante, es el segundo grupo con menor porcentaje de *heavy_user*. Por otro lado, el grupo que tiene mayor porcentaje de *heavy_user* es ***20-30***, esto se puede deber a que el ser más jóvenes entienden mejor el funcionamiento de la plataforma y se familiarizan con ella más rápido.

{% include edad_cat-freq.html %}
{% include edad_cat.html %}
