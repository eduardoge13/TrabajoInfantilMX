# TrabajoInfantil MX
En este repositorio se realiza un análisis de la Encuesta Nacional de Trabajo Infantil en México 2019, se hacen esfuerzos econométricos para determinar las causas de las condiciones de ocupacion infantil segun las definiciones del INEGI.

# Resumen
En el presente documento se aspira realizar una investigación sobre el trabajo infantil en México, tomando en cuenta algunas variables analizadas para la población de 5 a 17 años obtenidas de los microdatos de la Encuesta Nacional de Trabajo Infantil (ENTI 2019) del INEGI. Por lo que para analizar la base filtraremos de la base original variables de corte socioeconómico e intrafamiliar determinantes para la condición de trabajo infantil CTI como variable dependiente, así como, las omisiones, datos nulos, cuestionarios incompletos y categorías no especificadas, hasta conformar una submuestra.
Segundo, se realizará una descripción estadística de la base de datos y también de la submuestra, asi como un análisis de la muestra para que podamos observar la estructura y distribución de los datos y a que nivel representativo llegamos. Posteriormente, integramos un modelo logit multinomial con las variables seleccionadas, donde se analice la condición de ocupación de los infantes y con regresores socioeconómicos e intrafamiliares que consideramos tienen un mayor impacto en la determinación de su condición de ocupación, ya sea no permitida, peligrosa o no permitida y permitida. Finalmente se concluye con algunos resultados y reflexiones sobre el trabajo infantil en México en 2019, los retos y propuestas a implementar.
# Datos

Para la reproducibilidad del modelo deben usarse los microdatos de la Encuesta Nacional de Trabajo Infantil 2019 realizada por el INEGI:
https://www.inegi.org.mx/programas/enti/2019/#Microdatos

# Resultados 
![Trabajo Infantil en México; Horas en quehaceres domesticos](https://raw.githubusercontent.com/eduardoge13/TrabajoInfantilMX/main/images/Trabajo%20Infantil%20en%20México%3B%20Horas%20en%20quehaceres%20domesticos.png)

Vemos que, de los datos proporcionados por el INEGI (sin filtrar), en 2019 la cantidad de infantes que trabajaban al menos 14 horas era de 58,158 y más preocupante es que existan aún las 2602 observaciones que están trabajando de entre 14 y 28 horas.

![Trabajo Infantil en México; Condicion de quehaceres domesticos](https://raw.githubusercontent.com/eduardoge13/TrabajoInfantilMX/main/images/Trabajo%20Infantil%20en%20México%3B%20Condicion%20de%20quehaceres%20domesticos.png)

En la segunda gráfica podemos ver más claramente como en la condición de quehaceres domésticos tanto hombres como mujeres se encuentran en quehaceres domésticos con condiciones adecuadas, sin embargo es preocupante observar que aun más de 500 infantes de la submuestra se encuentran en horarios prolongados o condiciones peligrosas. Finalmente podemos ver que las mujeres son menos propensas a estar exentas de trabajo domestico.

![Trabajo Infantil en México; Edades de niños ocupados, por sexo](https://raw.githubusercontent.com/eduardoge13/TrabajoInfantilMX/main/images/Trabajo%20Infantil%20en%20México%3B%20%20Edades%20de%20niños%20ocupados.png)
La tercera gráfica nos demuestra la relación de la edad de los infantes con su condición de ocupación. Entre mayor edad, existe una mayor cantidad de niños ocupados, es decir que la economía requiere de fuerza de trabajo infantil y cada que se acercan a su edad propia para trabajar como adultos, se demanda mayor cantidad del mismo, aun en condiciones impropias.

## Efectos Marginales del modelo logistico multinomial
-   Si la edad crece hay 2.10 veces más probabilidad que el infante este en ocupación no permitida y quehaceres domésticos en condiciones no adecuadas, pero incrementa 29933 veces la probabilidad de que estén fuera del trabajo infantil, esto remarca el hecho de la demanda por trabajo infantil en México aun es amplia y abarca los años de edad más cercanos a cuando los infantes van a cumplir la mayoría de edad.

-   A su vez es 1.75 veces más probable que siendo hombre se este en condición de trabajo infantil.

-   La asistencia escolar presenta un efecto marginal fuerte ya que decimos que la asistencia a la escuela aumenta en 2.16 la probabilidad de que el infante este en condiciones de ocupación no permitida y quehaceres domésticos, sin embargo, si la asistencia crece solo incrementa en 0.42 veces la probabilidad de estar fuera de trabajo infantil.

-   La condición de ocupación solo afecta de manera muy reducida en la probabilidad que no este en CTI.

-   El nivel de escolaridad causa que los infantes tengan 1.3 veces más probabilidad de que estén en ocupaciones no permitidas y quehaceres domésticos, mientras que también aumenta en 0.72 veces la probabilidad de que los encuestados estén fuera del trabajo infantil. Los resultados son opuestos sin embargo esto podría apuntar a la tesis de que existen infantes que trabajan y estudian, y sus condiciones son riesgosas.

-   La probabilidad aumenta 1.95 veces de estar en CTI cuando también se realizan quehaceres domésticos, y aumenta en menor medida la probabilidad de estar fuera de la condición.

-   Como es lógico el nivel de ingreso responde de manera positiva al trabajo, aumentando la probabilidad de estar en condiciones de empleo malas, pues se puede inferir que los infantes necesitan estos trabajos por sus necesidades socioeconomicas. Sin embargo, también afecta de manera positiva en estar fuera del trabajo infantil, lo que podría indicar que muchos infantes trabajan y luego dejan de hacerlo o están en edades muy grandes.

-   El hecho de que el infante este bajo la contratación de una persona, aumenta sus probabilidades en 1.27 veces más de que sus condiciones de trabajo no sean aptas, pero, también aumenta en 1.60 a que estén fuera de estas condiciones, esto de manera significativa estadísticamente.

-   Finalmente el hecho de que un infante tenga un tipo de apoyo, hace probable en 1.0 veces que se encuentre fuera de trabajo infantil, por lo que se encontraría en condiciones mejores ya que no necesita recibir el ingreso y puede obtener empleos con mejores condiciones. Asimismo, se dice que el hecho que reciba algún apoyo implica que su probabilidad es 0.829 veces más que este en condiciones no aptas.

-   Los efectos marginales muestran los resultados finales del modelo. La edad demuestra ser de gran relevancia para estar fuera del trabajo infantil (4); a su vez es 1.75 veces más probable que siendo hombre este en CTI, es 2.16 veces más probable que los infantes que cumplan con la condición CTI tengan la necesidad de asistir a la escuela y es mucho menor la probabilidad de estar en CTI si se asiste a la escuela. Finalmente el nivel de escolaridad incrementa en 1.3 veces la necesidad de estar en CTI y asistir a la escuela, de nuevo apuntando a la tesis de que la escolaridad esta relacionada con el trabajo infantil, probablemente estas condiciones se deban a que el infante necesita financiamiento para sus estudios, así mismo, un nivel de escolaridad mayor aumenta en 0.72 veces la probabilidad de estar fuera de CTI.

## Conclusiones finales

Basado en el trabajo aquí escrito, tenemos suficiente evidencia para rechazar la hipótesis nula y por tanto los determinantes o regresores tienen, ciertamente, algún efecto en la variable dependiente CTI,  dento del modelo la mayor parte de las variables son significativas a un grado alto, la mayoría del modelo muestra un buen ajuste y su predicción es buena aunque mayores investigaciones son necesarias para analizar el nivel de efecto que tiene el orden de los hijos entre otras nuevas construcciones que han demostrado ser determinantes de igual forma.

Basado en el estudio de la ENTI, podemos rescatar que, aun existen una gran cantidad de infantes que tienen condiciones laborales que moralmente y jurídicamente deben desaparecer, por ello se propone mayores refuerzos especialmente para políticas publicas enfocadas a las familias numerosas en cuanto a asistencia económico-social, pues como se ha visto estos factores son los mayores determinantes a la hora de que los niños se encuentren en un ambiente pleno o se inserten al estudio, y si llegaran a estar en una ocupación, que esta fuera digna y sin condiciones de peligro.

Otra propuesta es la de el fomento a la educación básica, pues como ya se ha dicho la variable de la asistencia escolar esta relacionada tambien con la condicion de trabajo infantil nula, asi como concentrarnos en la educación media superior pues la mayor parte de los infantes que laboran están en un nivel educativo de secundaria o secundaria incompleta. De igual manera se recomienda el fomento a la educación por medio de becas y otros apoyos, con sepecial enfasis en promover politicas publicas para el incremento en el salario a nivel nacional en especifico para personas con familias numerosas, pues como ya se ha dicho esta variable también es importante a la hora de determinar si algun infante se encuentra en una condicion de trabajo infantil y dedicar mayor trabajo a disminuir la deserción y mejorar la educación media superior pues la mayor parte de los infantes que laboran están en un nivel educativo de secundaria o secundaria incompleta.
