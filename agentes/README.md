# Agentes del proyecto

Esta carpeta contiene protocolos operativos reutilizables de Informática Aplicada 2026.

## `entrega_informe`

Archivo: `agentes/entrega_informe.md`

Disparador: `entrega_informe`

Función: preparar la identificación, nomenclatura, estructura y contenido validado de un informe de entrega en TXT y, cuando se solicite, en PDF.

Al iniciar un informe, el agente debe obtener explícitamente para la interacción actual: nombre completo del alumno, tema, asignatura, carrera, sección, nombre del docente, universidad y facultad. No debe inferir ni reutilizar los datos institucionales o académicos desde conversaciones anteriores, GitHub, otros informes u otro contexto.

La nomenclatura utiliza `YYYYMMDD<letra>_nombre_del_alumno_tema`, con letras secuenciales por día (`a`, `b`, `c`, ...). El TXT y el PDF del mismo informe conservan la misma letra.

El agente debe conservar fielmente el texto del alumno: salvo solicitud explícita, solo puede aplicar correcciones ortográficas, de forma de palabra conforme al diccionario y gramaticales que no alteren el significado.

## `vocabulario feliz`

Archivo: `agentes/vocabulario_feliz.md`

Disparador: `vocabulario feliz`

Misión asociada: `misiones/20260814a_formacion_de_vocabulario.md`.

Función: identificar **vocabulario técnico directamente relacionado con la unidad de estudio y con el programa oficial**.

El agente usa el planeamiento para identificar la clase y la bibliografía, y el programa de estudios para verificar que los términos pertenezcan realmente al contenido técnico de la unidad. La presentación, el planeamiento y el programa no se utilizan como fuentes directas de vocabulario.

Se excluyen del vocabulario de estudio términos académicos generales o de presentación de la asignatura como `competencia`, `mérito académico` y `medición diagnóstica`. El alumno puede preguntar por ellos de forma independiente, pero no se incorporan automáticamente al vocabulario técnico de la unidad.

El agente debe identificar la bibliografía relacionada y presentarla en APA 7 cuando existan datos suficientes. Si la bibliografía necesaria no está disponible entre las fuentes, debe pedir al alumno que la agregue y detenerse hasta recibir aviso. No puede inventar ni sustituir automáticamente la fuente ausente.

Solo después de disponer de la obra bibliográfica debe localizar capítulos o secciones pertinentes, extraer términos técnicos, indicar su procedencia y justificar por qué conviene estudiarlos.

Los agentes deben respetar la metodología de **construcción de clases** y las reglas permanentes del proyecto.
