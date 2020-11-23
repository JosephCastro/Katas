# Calculadora sobre microservicios

Queremos hacer un servicio que se encargue de calcular ejercicios matematicas simples (sin paréntesis) , donde
tenemos el siguiente input y esperamos el siguiente output (uno por linea):

INPUT
    3 x 4 + 4 - 1
    1 + 2 + 3 + 4
    3 / 3 + 3 - 3

OUTPUT
    3 x 4 + 4 - 1 = 15
    1 + 2 + 3 + 4 = 10
    3 / 3 + 3 - 3 = 1
   
Para ello cada una de las operaciones básicas son un microservicio, en concreto (como mínimo):

- Microservicio para sumar (+)
- Microservicio para restar (-)
- Microservicio para multiplicar (*)
- Microservicio para dividir (/)

#### Nota: Debes considerar que tienes que tener un servicio u api para que poder obtener la respuesta.

Para resolver este ejercicio buscamos que cumplas las siguientes reglas:
- Ocupar buenas prácticas de desarrollo
- Ocupar patrones de integración de servicios y patrones de software
- Utilización de git comprensiva (queremos ir viendo como desarrollaste la solucion, por lo tanto debes incluir commits descriptivos).

 
Formato de entrega:
- Debes subir tu código, a un github/bitbucket/gitlab con un README de como usarlo.
- Debes ocupar docker y tener un docker-compose para levantar todos los servicios.
- Debes agregar diagramas que expliquen tu solución (los que estimes convenientes).

Evaluaremos
- Diseño de la solución, buscamos que pueda ser escalable y maneje concurrencia
- Calidad de la solución, mientras mas simple mejor, siempre cuidando las formas de desarrollo
- Desarrollo de la solución, como se implemento
- Buenas practicas de desarrollo, minimo tests de integracion en adelante
- Funcionamiento de la solución, que responda como debe responder
- Infraestructura + herramientas/tecnologia utilizada (REST, QUEUE, Mensajeria, etc)
