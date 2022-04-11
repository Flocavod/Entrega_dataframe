# Análisis de horas del área diseño Q1

## Introducción:

El tiempo dedicado por los empleados al desarrollo de las actividades dentro de la empresa resulta muy valioso para la toma de decisiones. 
Esta información se recaba mediante una aplicación donde cada trabajador debe medir el tiempo que le dedica a sus tareas diarias,
obteniendo mediante este medio los datos necesarios para la toma de decisiones tanto estrátegicas como operativas dentro de la misma. 
Al contar con estos datos surgen varias preguntas, 
desde el lado del servicio que brinda la empresa:Cuales categorías (servicios) captan la mayor cantidad de horas por el área de diseño? 
Mientras que desde una perspectiva del flujo de clientes soportados por el equipo existente dentro de la empresa la pregunta que surge es, 
Cuál es la saturación por empleado que se observa en el primer trimestre del año? 
Están al limite de las horas posibles o queda margen para que la empresa pueda ampliar su cartera de clientes?


## Contexto y Metodología

La empresa a la cual se va a proceder a analizar el dataset se dedica al rubro servicios, especificamente al área del marketing.
En los últimos años la cantidad de información que rodea a las empresas crece a gran nivel dado a las innumerables aplicaciones
y plataformas creadas para el uso diario de las personas y las cuales recolectan datos sobre gustos, preferencias, necesidades, entre otras.
Por estas razones para una empresa poder basar sus decisiones en información real y no basadas en las decisiones de los competidores hoy en día es fundamental
para poder competir en el mercado. 
A su vez debido a la constante actualización de servicios que se requiere en el rubro del marketing para poder ser competitivo es que surge la necesidad
de medir el tiempo dedicado a las tareas diarias del empleado con el fin de mejorar tanto la productividad y eficiencia de los factores productivos
como la calidad del servicio brindado hacia los clientes.

El período de análisis del siguiente informe se basa en los datos extraídos de la aplicación TrackingTime durante el primer trimestre del 2022 del equipo de diseño. 
> Se procede a clasificar las tareas que lleva acabo el área y asi poder definir categorías, estas agrupan dichas tareas para poder facilitar el análisis y lograr
una análisis comparativo de los servicios a los que contribuye el equipo. Las categorías finales se ven reflejadas en el siguiente cuadro de referencia junto 
con los empleados que componen el equipo; mediante esta tabla se va a guiar el análisis.

### Cuadro de referencia del Dataframe

| Designer           | Categories  |
|--------------------|-------------|
| Sofía Pérez (head) | Media       |
| Gonzalo Zamora     | Ads         |
| Jerusa Villalba    | Web         |
| Matias Paoli       | Tradicional |
|                    | Audiovisual |
|                    | Reuniones   |



#### Las columnas finales para el análsis luego de limpiar el dataset se encuentran en la siguiente tabla junto con su clasificación:

| Serie     | Tipo de dato            |
|-----------|-------------------------|
| clientes  | str, categórico nominal |
| tarea     | str, categórico nominal |
| reuniones | str, categórico nominal |
| empleado  | str, categórico nominal |
| fecha     | str, categórico ordinal |
| desde     | str, categórico ordinal |
| hasta     | str, categórico ordinal |
| duración  | str, categórico ordinal |
| horas     | numérico, float         |
| cambios   | str, categórico ordinal |

## Conclusiones


### Categorías:

Dado las categorías definidas anteriormente se puede observar que de las 1056 horas de la muestra,
374 horas el equipo de diseño le dedica al servicio de Social Media, 
mientras que en el servicio de Ads se registran 69 horas, es decir, un 18% de las horas dedicadas a Social Media. 
También se puede observar que la categoría reuniones es la segunda categoría que reporta una elevada cantidad de horas medidas
por el equipo con un total de 294 horas.


### Saturación Empleado:

En este análisis se estima un margen de 1 hr de error diaria por empleado en el total de horas trackeadas debido a varios factores
como el nivel de productividad como tareas que surgen en el momento fuera de la clasificación y que en el futuro hay que ir ajustando.
Por esta razón el total de horas por mes ajustado al margen de error es de:

* Enero: 140 hrs en el mes
* Febrero: 133 hrs en el mes
* Marzo: 154 en el mes

* El total de horas por empleado en el Q1 es de 427. 

Dado lo observado en la muestra se concluye que Sofia se encuentra cerca del nivel de tope de trabajo diario (414,15).Esto tiene sentido dado
que es la head del área y además de las actividades que comprenden diseñar para los clientes,desarrolla actividades de liderazgo 
como distribución de tareas. 
Jerusa (317,8)y Gonzalo (223,35) muestran un margen considerable de tiempo libre para poder realizar actividades que les compete al igual que Matias (100,49),
quien se encuentra muy por debajo de la media de las horas de trabajo (264).
