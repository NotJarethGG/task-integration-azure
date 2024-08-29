[![Board Status](https://dev.azure.com/prueba-github-integration/5a0b9ee3-f259-4889-b114-e3ecaa426d55/f31fd6cd-5f96-4039-85e2-4d77201d2ba5/_apis/work/boardbadge/e0213df9-bc67-44f6-a26b-82ebd6e9383e)](https://dev.azure.com/prueba-github-integration/5a0b9ee3-f259-4889-b114-e3ecaa426d55/_boards/board/t/f31fd6cd-5f96-4039-85e2-4d77201d2ba5/Backlog%20items/)

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Estándar de desarrollo - Universidad Nacional</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 40px;
            line-height: 1.6;
        }
        h1, h2, h3 {
            text-align: center;
        }
        h1 {
            margin-bottom: 0;
        }
        h2 {
            margin-top: 5px;
        }
        h3 {
            margin-top: 40px;
        }
        p {
            text-align: justify;
        }
        ul {
            margin-left: 20px;
        }
        hr {
            margin: 40px 0;
        }
        .note {
            margin-top: 40px;
            font-style: italic;
        }
    </style>
</head>
<body>

    <h1>UNIVERSIDAD NACIONAL</h1>
    <h2>Sede Regional Chorotega<br>Campus Nicoya</h2>

    <hr>

    <h2>Universidad Nacional</h2>
    <h3>Estándar de desarrollo</h3>
    <h3>LabCibe</h3>
    <h3>2024</h3>

    <hr>

    <h3>INDICE</h3>
    <ul>
        <li><a href="#introduccion">INTRODUCCIÓN</a></li>
        <li><a href="#principios">Principios Clave del Estándar de Desarrollo</a>
            <ul>
                <li><a href="#validacion">Validación antes de marcar tareas como completadas</a></li>
                <li><a href="#revision-uat">Revisión previa a la implementación en UAT</a></li>
                <li><a href="#creacion-ramas">Estándar para la creación de ramas</a></li>
                <li><a href="#convenciones-codigo">Uso consistente de convenciones de código</a></li>
                <li><a href="#revision-colaborativa">Revisión de código colaborativa</a></li>
                <li><a href="#documentacion-funciones">Documentación de funciones y módulos</a></li>
                <li><a href="#integracion-continua">Integración continua y despliegue automatizado</a></li>
                <li><a href="#gestion-dependencias">Gestión de dependencias y versiones</a></li>
                <li><a href="#manejo-errores">Estrategia de manejo de errores y excepciones</a></li>
                <li><a href="#pruebas-unitarias">Pruebas unitarias obligatorias</a></li>
            </ul>
        </li>
    </ul>

    <hr>

    <h3 id="introduccion">INTRODUCCIÓN</h3>
    <p>En el entorno actual de desarrollo de software, la implementación de estándares es fundamental para garantizar la calidad, consistencia y escalabilidad de los proyectos. Un estándar de desarrollo proporciona un conjunto de directrices y mejores prácticas que guían a los equipos en la creación de soluciones eficientes, seguras y mantenibles. Este documento presenta un estándar de desarrollo diseñado para optimizar los procesos, reducir los riesgos y fomentar una colaboración efectiva entre los desarrolladores, asegurando que el producto final cumpla con las expectativas del cliente y las exigencias del mercado.</p>
    <p>En las siguientes secciones, se detallarán los principios clave, las herramientas recomendadas, y las prácticas esenciales que deben seguirse en todas las fases del ciclo de vida del desarrollo, desde la planificación inicial hasta el despliegue y mantenimiento del software. Este estándar no solo sirve como una guía técnica, sino también como un marco que promueve la innovación y la adaptabilidad en un entorno de desarrollo en constante evolución.</p>

    <h3 id="principios">Principios Clave del Estándar de Desarrollo</h3>

    <h4 id="validacion">1. Validación antes de marcar tareas como completadas</h4>
    <p>Ninguna tarea puede ser marcada como "Done" sin antes proporcionar pruebas de su correcto funcionamiento. Además, el estado de la tarea no se considerará completado hasta que el pull request asociado haya sido revisado y aceptado en GitHub. Este proceso asegura que cada cambio cumple con los requisitos establecidos y no introduce errores en el código base.</p>

    <h4 id="revision-uat">2. Revisión previa a la implementación en UAT</h4>
    <p>Las partes programadas no pueden ser transferidas al entorno de pruebas de aceptación del usuario (UAT) hasta que las pull requests correspondientes hayan sido aceptadas. Esto garantiza que solo el código aprobado y revisado llegue a las pruebas finales, minimizando riesgos de fallos y asegurando que el software cumple con los estándares de calidad antes de ser presentado al cliente o usuario final.</p>

    <h4 id="creacion-ramas">3. Estándar para la creación de ramas</h4>
    <p>Al crear una nueva rama en el repositorio, se debe seguir la siguiente convención de nombres: <code>task/81-api-registro-reporte</code>. Este formato ayuda a mantener un orden y claridad en la gestión de las ramas, permitiendo a los miembros del equipo identificar fácilmente el propósito de cada rama y su relación con tareas específicas del proyecto.</p>

    <h4 id="convenciones-codigo">4. Uso consistente de convenciones de código</h4>
    <p>Es crucial que todos los desarrolladores sigan un conjunto uniforme de convenciones de codificación. Esto incluye la nomenclatura de variables y funciones, la organización del código y los comentarios. Por ejemplo, las variables deben seguir la convención <code>camelCase</code>, las funciones deben nombrarse utilizando verbos que describan su acción, y el código debe ser comentado de manera clara y concisa para facilitar su comprensión por otros miembros del equipo.</p>

    <h4 id="revision-colaborativa">5. Revisión de código colaborativa</h4>
    <p>Antes de fusionar cualquier pull request en la rama principal, se requiere una revisión de código por parte de al menos otro miembro del equipo. Esta revisión debe enfocarse en detectar posibles errores, asegurar la adherencia a las convenciones de codificación y verificar que el código cumple con los requisitos funcionales. Las revisiones colaborativas no solo mejoran la calidad del código, sino que también fomentan el aprendizaje y la cohesión del equipo.</p>

    <h4 id="documentacion-funciones">6. Documentación de funciones y módulos</h4>
    <p>Cada nueva función o módulo agregado al código debe ir acompañado de una documentación clara que explique su propósito, su uso esperado y cualquier dependencia relevante. Esta documentación debe ser mantenida actualizada conforme el código evoluciona, garantizando que cualquier desarrollador pueda entender y utilizar el código sin necesidad de asistencia adicional.</p>

    <h4 id="integracion-continua">7. Integración continua y despliegue automatizado</h4>
    <p>Se debe implementar un proceso de integración continua (CI) que ejecute pruebas automatizadas cada vez que se realiza un commit en el repositorio. Esto asegura que cualquier nuevo código introducido no rompa la funcionalidad existente. Además, un despliegue automatizado a entornos de desarrollo o prueba puede ser configurado para facilitar la entrega continua de software.</p>

    <h4 id="gestion-dependencias">8. Gestión de dependencias y versiones</h4>
    <p>Es importante que las dependencias del proyecto estén claramente especificadas y que se mantenga un control estricto de las versiones utilizadas. Se recomienda utilizar un archivo de bloqueo (<code>lock file</code>) para asegurar que todos los desarrolladores estén utilizando las mismas versiones de las dependencias, evitando conflictos y asegurando la consistencia del entorno de desarrollo.</p>

    <h4 id="manejo-errores">9. Estrategia de manejo de errores y excepciones</h4>
    <p>El código debe incluir una estrategia clara para manejar errores y excepciones. Esto incluye la captura de excepciones en los lugares apropiados, el registro de errores para análisis posterior, y la provisión de mensajes de error útiles para el usuario final. Un manejo adecuado de errores no solo mejora la experiencia del usuario, sino que también facilita la identificación y solución de problemas durante el desarrollo.</p>

    <h4 id="pruebas-unitarias">10. Pruebas unitarias obligatorias</h4>
    <p>Cada nuevo código que se añade al repositorio debe estar acompañado de pruebas unitarias que validen su funcionamiento. Las pruebas deben cubrir los casos normales y extremos para asegurar que el código se comporta como se espera en todas las circunstancias. Estas pruebas deben ser revisadas junto con el código durante el proceso de pull request.</p>

    <p class="note">NOTA: Se puede ir modificando a futuro.</p>

</body>
</html>

