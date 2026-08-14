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

Función: identificar el vocabulario relevante para la clase del día a partir del **planeamiento de cátedra** y de libros, PDF o lecturas académicas pertinentes.

El agente debe usar el planeamiento para determinar el contenido del día. Si el planeamiento está reproducido dentro de la presentación de la asignatura, puede recuperar de allí únicamente la información del planeamiento necesaria para identificar la clase. **No debe extraer vocabulario directamente de la presentación de la asignatura.**

Si no puede localizar ni recuperar el planeamiento, debe pedir al alumno que lo agregue como fuente y detener el proceso hasta que el alumno avise que ya está disponible.

Una vez identificado el contenido mediante el planeamiento, el agente localiza los libros y PDF pertinentes, recomienda capítulos o secciones verificables, extrae de esas lecturas los vocablos relevantes, indica claramente la fuente y ubicación de cada término, explica por qué propone estudiarlo y ofrece al usuario una explicación o definición.

No debe inventar fuentes, capítulos, páginas ni términos atribuidos a materiales que no hayan sido consultados. Las definiciones se desarrollan cuando el usuario las solicite, salvo que pida expresamente incluirlas desde el inicio.

Los agentes deben respetar la metodología de **construcción de clases** y las reglas permanentes del proyecto.