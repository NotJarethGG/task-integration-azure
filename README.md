<div style="text-align: center;">
  <h1>UNIVERSIDAD NACIONAL</h1>
  <h2>Sede Regional Chorotega</h2>
  <h3>Campus Nicoya</h3>

  <h2>Estándar de Desarrollo</h2>
  
  <h3>LabCibe</h3>
  <h4>2024</h4>
</div>

---

## Índice

1. [Introducción](#introducción)
2. [Principios Clave del Estándar de Desarrollo](#principios-clave-del-estándar-de-desarrollo)  
   1. [Validación antes de marcar tareas como completadas](#validación-antes-de-marcar-tareas-como-completadas)  
   2. [Revisión previa a la implementación en UAT](#revisión-previa-a-la-implementación-en-uat)  
   3. [Estándar para la creación de ramas](#estándar-para-la-creación-de-ramas)  
   4. [Uso consistente de convenciones de código](#uso-consistente-de-convenciones-de-código)  
   5. [Revisión de código colaborativa](#revisión-de-código-colaborativa)  
   6. [Documentación de funciones y módulos](#documentación-de-funciones-y-módulos)  
   7. [Integración continua y despliegue automatizado](#integración-continua-y-despliegue-automatizado)  
   8. [Gestión de dependencias y versiones](#gestión-de-dependencias-y-versiones)  
   9. [Estrategia de manejo de errores y excepciones](#estrategia-de-manejo-de-errores-y-excepciones)  
   10. [Pruebas unitarias obligatorias](#pruebas-unitarias-obligatorias)  

---

## Introducción

En el entorno actual de desarrollo de software, la implementación de estándares es fundamental para garantizar la calidad, consistencia y escalabilidad de los proyectos. Un estándar de desarrollo proporciona un conjunto de directrices y mejores prácticas que guían a los equipos en la creación de soluciones eficientes, seguras y mantenibles. Este documento presenta un estándar de desarrollo diseñado para optimizar los procesos, reducir los riesgos y fomentar una colaboración efectiva entre los desarrolladores, asegurando que el producto final cumpla con las expectativas del cliente y las exigencias del mercado.

En las siguientes secciones, se detallarán los principios clave, las herramientas recomendadas, y las prácticas esenciales que deben seguirse en todas las fases del ciclo de vida del desarrollo, desde la planificación inicial hasta el despliegue y mantenimiento del software. Este estándar no solo sirve como una guía técnica, sino también como un marco que promueve la innovación y la adaptabilidad en un entorno de desarrollo en constante evolución.

---

## Principios Clave del Estándar de Desarrollo

### 1. Validación antes de marcar tareas como completadas
Ninguna tarea puede ser marcada como "Done" sin antes proporcionar pruebas de su correcto funcionamiento. Además, el estado de la tarea no se considerará completado hasta que el pull request asociado haya sido revisado y aceptado en GitHub. Este proceso asegura que cada cambio cumple con los requisitos establecidos y no introduce errores en el código base.

### 2. Revisión previa a la implementación en UAT
Las partes programadas no pueden ser transferidas al entorno de pruebas de aceptación del usuario (UAT) hasta que las pull requests correspondientes hayan sido aceptadas. Esto garantiza que solo el código aprobado y revisado llegue a las pruebas finales, minimizando riesgos de fallos y asegurando que el software cumple con los estándares de calidad antes de ser presentado al cliente o usuario final.

### 3. Estándar para la creación de ramas
Al crear una nueva rama en el repositorio, se debe seguir la siguiente convención de nombres: `task/81-api-registro-reporte`. Este formato ayuda a mantener un orden y claridad en la gestión de las ramas, permitiendo a los miembros del equipo identificar fácilmente el propósito de cada rama y su relación con tareas específicas del proyecto.

### 4. Uso consistente de convenciones de código
Es crucial que todos los desarrolladores sigan un conjunto uniforme de convenciones de codificación. Esto incluye la nomenclatura de variables y funciones, la organización del código y los comentarios. Por ejemplo, las variables deben seguir la convención `camelCase`, las funciones deben nombrarse utilizando verbos que describan su acción, y el código debe ser comentado de manera clara y concisa para facilitar su comprensión por otros miembros del equipo.

### 5. Revisión de código colaborativa
Antes de fusionar cualquier pull request en la rama principal, se requiere una revisión de código por parte de al menos otro miembro del equipo. Esta revisión debe enfocarse en detectar posibles errores, asegurar la adherencia a las convenciones de codificación y verificar que el código cumple con los requisitos funcionales. Las revisiones colaborativas no solo mejoran la calidad del código, sino que también fomentan el aprendizaje y la cohesión del equipo.

### 6. Documentación de funciones y módulos
Cada nueva función o módulo agregado al código debe ir acompañado de una documentación clara que explique su propósito, su uso esperado y cualquier dependencia relevante. Esta documentación debe ser mantenida actualizada conforme el código evoluciona, garantizando que cualquier desarrollador pueda entender y utilizar el código sin necesidad de asistencia adicional.

### 7. Integración continua y despliegue automatizado
Se debe implementar un proceso de integración continua (CI) que ejecute pruebas automatizadas cada vez que se realiza un commit en el repositorio. Esto asegura que cualquier nuevo código introducido no rompa la funcionalidad existente. Además, un despliegue automatizado a entornos de desarrollo o prueba puede ser configurado para facilitar la entrega continua de software.

### 8. Gestión de dependencias y versiones
Es importante que las dependencias del proyecto estén claramente especificadas y que se mantenga un control estricto de las versiones utilizadas. Se recomienda utilizar un archivo de bloqueo (`lock file`) para asegurar que todos los desarrolladores estén utilizando las mismas versiones de las dependencias, evitando conflictos y asegurando la consistencia del entorno de desarrollo.

### 9. Estrategia de manejo de errores y excepciones
El código debe incluir una estrategia clara para manejar errores y excepciones. Esto incluye la captura de excepciones en los lugares apropiados, el registro de errores para análisis posterior, y la provisión de mensajes de error útiles para el usuario final. Un manejo adecuado de errores no solo mejora la experiencia del usuario, sino que también facilita la identificación y solución de problemas durante el desarrollo.

### 10. Pruebas unitarias obligatorias
Cada nuevo código que se añade al repositorio debe estar acompañado de pruebas unitarias que validen su funcionamiento. Las pruebas deben cubrir los casos normales y extremos para asegurar que el código se comporta como se espera en todas las circunstancias. Estas pruebas deben ser revisadas junto con el código durante el proceso de pull request.

---

**NOTA:** Este estándar puede ser modificado en el futuro para adaptarse a nuevas necesidades y desafíos.
