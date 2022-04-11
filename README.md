## Introducción:
El tiempo dedicado por los empleados al desarrollo de las actividades dentro de la empresa resulta muy valioso para la toma de decisiones. Esta información se recaba mediante una 
aplicación donde cada trabajador debe medir el tiempo que le dedica a sus tareas diarias, por este medio se recaba la información la cual resulta muy útil ante la toma de decisiones tanto 
estrátegicas como operativas dentro de la misma. El período de análisis del siguiente informe es del primer trimestre del 2022. Al contar con estos datos surgen varias preguntan a contesta como, 
desde el lado del servicio que se brinda por la empresa *Cuales categorías (servicios) captan la mayor cantidad de horas por el área de diseño? 
Mientras que para poder tomar decisiones acerca de la cantidad de clientes que soporta el equipo existente dentro de la empresa la pregunta es: 
Cuál es la saturación por empleado que se observa en el primer trimestre del año?


## Contexto y Metodología

La empresa a la cual se va a proceder a analizar el dataset se dedica al rubro servicios, especificamente al área del marketing. En los últimos años la cantidad de información que rodea a las empresas crece a gran nivel dado a las innumerables aplicaciones y plataformas creadas para el uso diario de las personas y las cuales recolectan datos sobre gustos, preferencias, necesidades, entre otras. Por lo que para una empresa poder basar sus decisiones en información real y no sobre tendencia hoy en día es fundamental para poder competir en el mercado. 
Debido a la constante actualización de servicios que se requiere por parte del marketing para poder ser competitivo es que se comienza a medir el tiempo dedicado a las tareas diarias del empleado con el fin de mejorar la productividad, eficiencia y calidad del servicio brindado por parte de la misma.

Se procede a clasificar los servicios de un área de gran importancia como es la de diseño, la misma se ve reflejada en el siguiente cuadro de referencia junto con los empleados que componen el equipo; mediante esta tabla se va a guiar el análisis.

### Cuadro de referencia del Dataframe

| Designer           | Categories  |
|--------------------|-------------|
| Sofía Pérez (head) | Media       |
| Gonzalo Zamora     | Ads         |
| Jerusa Villalba    | Web         |
| Matias Paoli       | Tradicional |
|                    | Audiovisual |
|                    | Reuniones   |



#### Las columnas finales para el análsis luego de limpiar el dataset se encuentran en la siguiente tabla junto con su clasificación

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

#### Categorías:

De las 1056 horas de la muestra se observa que 374 horas el equipo de diseño le dedica al servicio de Social Media mientras que en el servicio de Ads
se registran 69 horas. También se observa que la categoría reuniones es la segunda con mayor cantidad de horas dedicadas por el equipo con un total de 294 horas.


### Saturación Empleado

* Enero: 140 hrs en el mes
* Febrero: 133 hrs en el mes
* Marzo: 154 en el mes

* Total de horas por empleado en Q1: 427 con un margen de error de una hora por día. 

Se concluye que Sofia se encuentra cerca del nivel de tope de trabajo diario, tiene sentido dado que es la head del área y además de diseñar desarrolla actividades de liderazgo en el área. 
Jerusa y Gonzalo muestran un margen considerable de tiempo libre para poder realizar actividades que les compete al igual que Matias, quien se encuentra muy por debajo de la media de las horas de trabajo.
