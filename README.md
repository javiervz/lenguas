# Mapas de lenguas del mundo :)

Un vistazo a los contenidos!

  * [Nuestra idea!](#nuestra-idea)
  * [Datos y datos!](#datos-y-datos)
  * [Mapas y mapas!](#mapas-y-mapas)
  * [Algunas figuras!](#algunas-figuras)

## Nuestra idea!
Nos proponemos describir las relaciones entre **complejidad morfológica** y **vitalidad** en lenguas del mundo. Para aproximarnos a diferencias en las maneras de codificar la morfología, usamos la [entropía](http://www.christianbentz.de/Papers/Bentz%20et%20al.%20(2017)%20The%20entropy%20of%20words.pdf): valores extremos de esta medida, suponen una gran variedad de palabras distintas (resultado de procesos morfológicos); valores mínimos de entropía supone la existencia de menos palabras distintas. Por otro lado, la vitalidad lingüística es entendida según la escala **AES** (Agglomerated Endangerment Status [detalles](https://glottolog.org/glottolog/glottologinformation)), que define 6 niveles de obsolescencia creciente. Planteamos entonces la siguiente hipótesis:

* **Hipótesis (H).** A **mayor obsolescencia** en la escala AES, observaremos **menor entropía**. 

La justificación es al parecer bastante plausible: las lenguas obsolescentes evidencian procesos de pérdida de complejidad morfológica. Por ejemplo,(aunque es otro contexto) existe una disminución de entropía si comparamos el Latín con lenguas romances modernas [link a más información sobre casos y Latín](https://www.aclweb.org/anthology/W16-4125.pdf). 

## Datos y datos!

Utilizamos diversas fuentes de datos:

* **Datos de entropía para 1259 lenguas** calculados por [paper interesante](http://www.christianbentz.de/Papers/Bentz%20et%20al.%20(2017)%20The%20entropy%20of%20words.pdf). Estos datos son abiertos y pueden obtenerse de [datos entropía](http://www.christianbentz.de/publications.html).
* **Datos sobre obsolescencia:** usamos la información proporcionada por [Glottolog](https://glottolog.org/meta/downloads). 
* **WALS:** para acceder a los rasgos de esta base de datos, utilizamos [lingtypology](https://github.com/OneAdder/lingtypology)

## Mapas y mapas!

En esta sección, usamos la famosa librería [lingtypology](https://github.com/OneAdder/lingtypology) para mostrar resultados a través de mapas. 

* [Entropía](./map_entropy.html). En este mapa, dividimos los valores de entropía en 3: **high**, **middle**, **low**. El nivel **middle** se define como los valores que se encuentran a 1 desviación estándar (o menos) del promedio. 

* [Número de casos](./map_entropy.html) (rasgo 49A de [WALS](https://wals.info/))

* [Vitalidad](./map_glottolog.html) de todas las lenguas de [Glottolog](https://glottolog.org/)

* [Vitalidad](./map_entropy_glottolog.html)

## Algunas figuras!

* Número de lenguas según grado de vitalidad :)
![Número de lenguas](https://github.com/javiervz/lenguas/blob/master/vitality.jpg?raw=true)
