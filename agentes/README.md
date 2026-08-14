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

Función: identificar el vocabulario relevante para la clase del día utilizando el **planeamiento de cátedra para determinar el contenido y localizar la bibliografía correspondiente**, y utilizando después la obra bibliográfica realmente disponible para extraer vocablos.

El agente **no propone el planeamiento como fuente de lectura para formar vocabulario**. Debe identificar en el planeamiento la bibliografía asociada a la clase y presentarla en formato APA 7 cuando existan datos suficientes, sin inventar información faltante.

Si el planeamiento no está disponible, debe pedir al alumno que lo agregue y detener el proceso hasta recibir aviso. Si la bibliografía indicada en el planeamiento no está disponible entre las fuentes del cuaderno, debe pedir al alumno que agregue esa obra bibliográfica y detenerse hasta que el alumno avise que ya está disponible.

Solo después de disponer de la obra bibliográfica debe localizar capítulos, secciones o páginas pertinentes, extraer vocablos, indicar su procedencia y explicar por qué propone estudiarlos. La presentación de la asignatura no se utiliza como fuente directa de vocabulario.

No debe inventar fuentes, referencias APA, capítulos, páginas ni términos atribuidos a materiales que no hayan sido consultados. Las definiciones se desarrollan cuando el usuario las solicite, salvo que pida expresamente incluirlas desde el inicio.

Los agentes deben respetar la metodología de **construcción de clases** y las reglas permanentes del proyecto.