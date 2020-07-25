# Entropía, obsolescencia y mapas de lenguas del mundo :)

Un vistazo a los contenidos!

  * [Nuestra idea!](#nuestra-idea)
  * [Datos y datos!](#datos-y-datos)
  * [Mapas y mapas!](#mapas-y-mapas)
  * [Resultados en forma de figura!](#resultados-en-forma-de-figura)

## Nuestra idea!
Nos proponemos describir las relaciones entre **complejidad morfológica** y **vitalidad** en lenguas del mundo. Para aproximarnos a diferencias en las maneras de codificar la morfología, usamos la [entropía](http://www.christianbentz.de/Papers/Bentz%20et%20al.%20(2017)%20The%20entropy%20of%20words.pdf): valores extremos de esta medida, suponen una gran variedad de palabras distintas (resultado de procesos morfológicos); valores mínimos de entropía supone la existencia de menos palabras distintas. Por otro lado, la vitalidad lingüística es entendida según la escala **AES** (Agglomerated Endangerment Status [detalles](https://glottolog.org/glottolog/glottologinformation)), que define 6 niveles de obsolescencia creciente. Planteamos entonces la siguiente hipótesis:

* **Hipótesis (H).** A **mayor obsolescencia** en la escala AES, observaremos **menor entropía**. 

La justificación es al parecer bastante plausible: las lenguas obsolescentes evidencian procesos de pérdida de complejidad morfológica. Por ejemplo,(aunque es otro contexto) existe una disminución de entropía si comparamos el Latín con lenguas romances modernas [link a más información sobre casos y Latín](https://www.aclweb.org/anthology/W16-4125.pdf). 

## Datos y datos!

Utilizamos diversas fuentes de datos:

* **Datos de entropía para 1259 lenguas** calculados por [paper interesante](http://www.christianbentz.de/Papers/Bentz%20et%20al.%20(2017)%20The%20entropy%20of%20words.pdf). Estos datos son abiertos y pueden obtenerse de [datos entropía](http://www.christianbentz.de/publications.html).
* **Datos sobre obsolescencia:** usamos la información proporcionada por [Glottolog](https://glottolog.org/meta/downloads). 
* **WALS:** para acceder a los rasgos de esta base de datos, utilizamos [lingtypology](https://github.com/OneAdder/lingtypology). En general esta base de datos es __sparse__, por lo que posee una gran cantidad de rasgos para los cuales no hay información. 

## Mapas y mapas!

En esta sección, usamos la famosa librería [lingtypology](https://github.com/OneAdder/lingtypology) para mostrar resultados a través de mapas. 

* [Entropía](./map_entropy.html). En este mapa, dividimos los valores de entropía en 3: **high**, **middle**, **low**. La muestra incluye datos para **1245 lenguas**. El nivel **middle** se define como los valores que se encuentran a 1 desviación estándar (o menos) del promedio. Es interesante notar, por ejemplo, la **alta entropía de lenguas andinas**. 

* [Número de casos](./map_entropy.html) (rasgo 49A de [WALS](https://wals.info/)). El **rasgo 49A de WALS** cuenta el número de casos. ¿Existe una relación entre número de casos y entropía? 

* [Vitalidad para todas las lenguas en Glottolog](./map_glottolog.html). En este mapa, se incluyen todas las lenguas de [Glottolog](https://glottolog.org), para las que existe información sobre la escala **AES**: 7831 lenguas :)

* [Vitalidad para las lenguas donde tenemos información de entropía](./map_entropy_glottolog.html). Aquí, fundimos los datos sobre **entropía** y la escala **AES**. Presentamos entonces la **vitalidad** para 1245 lenguas.  

## Resultados en forma de figura!

1. **Número de lenguas según grado de vitalidad.** Para la muestra de **7831 lenguas**, el eje **vitality** indica un grado creciente de obsolescencia, desde **safe** hasta **extinct**. El eje **percentage of languages** indica la proporción de lenguas que se encuentra es un estado específico de vitalidad. Desde [Glottolog](https://glottolog.org]) extraemos la información de **macroareas lingüísticas.** 
![Número de lenguas vs vitalidad](https://github.com/javiervz/lenguas/blob/master/vitality.jpg?raw=true)

2. **Número de lenguas según grado de vitalidad (conjunto restringido de lenguas).** Para la muestra de **1245 lenguas** (para las que tenemos valores de **entropía**), mostramos la relación entre **vitality** y **percentage of languages**. Notemos la disminución (con respecto a la figura anterior) del número de lenguas en estado **extinct**, y al mismo tiempo el aumento de lenguas en estado **vulnerable** y **definitely endangered.**
![Número de lenguas vs vitalidad](https://github.com/javiervz/lenguas/blob/master/vitality_entropy.jpg?raw=true)

3. **Entropía versus vitalidad (conjunto restringido de lenguas).** xxx
![Entropía vs vitalidad](https://github.com/javiervz/lenguas/blob/master/vitalityvsentropy.jpg?raw=true)
