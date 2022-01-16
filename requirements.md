## DESCRIPCIÓN

Para esta prueba se requiere que se integre el API pública  (https://postcodes.io/) que tiene únicamente la información detallada de los códigos postales de UK. 

1. Crear un endpoint que reciba el archivo poscodes_geo.csv que contiene coordenadas cercanas a algunos códigos postales, se desea leer el archivo y hacer uso del API para obtener la información detallada del código postal más cercano a las coordenadas de cada fila. Esta información debe ser almacenada en una base de datos de libre elección.
2. En el README.md realiza una breve explicación y un diagrama de la arquitectura definida que nos explique claramente tu solución propuesta. Además debes agregar el paso para hacerlo funcionar y alguna otra recomendación que creas relevante.



## RESTRICCIONES

- Debes resolver el reto individualmente.
- Crear 2 microservicios:
  - Para recibir el archivo y almacenarlo. 
  - Para consumir el API (postcodes), procesar la data del punto anterior y enviar los códigos postales de nuevo al servicio que tiene la base de datos para completar la información.
- Estos deben ser escritos en cualquiera de los siguientes lenguajes:
  - Javascript/Typescript
  - Python
- Al comunicar los 2 microservicios debes garantizar que todas las coordenadas tienen un código postal.
- El usuario debe enterarse si hay errores en el archivo csv
- Controla las peticiones del API (postcodes) son limitadas
- Los servicios deben levantarse fácilmente a través del uso de Docker Compose o una herramienta similar.
- Debes escribir tests unitarios para todas las funcionalidades de tu código.

## TIPS

- La escalabilidad y la eficiencia son muy importantes.
- Podrás usar cualquier librería o framework para el desarrollo.
- Procura crear cambios pequeños que reflejen el desarrollo de la prueba basado en el historial del repositorio. Puedes utilizar Git Flow o cualquier otro flujo para el manejo del repositorio. Deja escrito en el README.md qué flujo seguiste.

## PUNTOS A EVALUAR

En caso de no terminar la prueba, existen otros factores importantes que evaluaremos para poder hacernos una mejor idea de tu experiencia

- El uso y balance correcto de patrones de diseño, además de mvc o mvm del framework que utilices
- Patrones de integración para la comunicación entre servicios
- Buenas prácticas en el código
- Un mínimo de pruebas unitarias 
- El uso de capas para separar las responsabilidades dentro de los servicios


## ENTREGABLE

Sube a un repositorio en GitHub la solución del reto propuesto.
