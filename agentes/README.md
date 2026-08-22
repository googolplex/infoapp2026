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

Función: aplicar un **método transversal para formar vocabulario por unidad de estudio**, reutilizable en distintas asignaturas sin incorporar ejemplos, términos ni bibliografías específicas de una disciplina en el protocolo permanente.

El agente identifica la unidad desde el planeamiento, programa o documento equivalente; localiza la bibliografía relacionada; verifica que la obra esté disponible; determina qué capítulo, sección o páginas conviene leer; y extrae vocablos directamente relacionados con la unidad.

La salida normal se organiza en **tandas de alrededor de 40 vocablos**. La primera presentación de cada tanda contiene solo los términos, sin definiciones ni desarrollos automáticos. Si la fuente inspeccionada no permite sostener aproximadamente 40 vocablos pertinentes, se presentan únicamente los disponibles en vez de completar la cantidad con términos dudosos.

Cuando el usuario solicita otra lista, otros 40 o una petición equivalente, el agente genera una nueva tanda sin repetir los vocablos de las tandas anteriores de esa misma unidad que estén verificablemente disponibles en el contexto de la interacción.

Las definiciones, explicaciones y ejemplos se desarrollan únicamente cuando el usuario pregunta por uno o varios términos o solicita expresamente su desarrollo.

Si no puede identificar la unidad o si la bibliografía necesaria no está disponible, debe pedir al usuario que agregue la fuente correspondiente y detenerse hasta recibir aviso. No debe inventar ni sustituir automáticamente la fuente ausente.

Los vocablos deben provenir de obras realmente inspeccionadas y mantener trazabilidad con la unidad correspondiente.

## `vocabulario técnico — Informática Aplicada`

Archivo: `agentes/vocabulario_tecnico_informatica_aplicada.md`

Disparador: `formación de vocabulario para la clase` o una instrucción equivalente.

Función: identificar, organizar y desarrollar el vocabulario técnico que los estudiantes necesitan para comprender una **clase, sesión o bloque didáctico concreto de Informática Aplicada**.

El agente trabaja exclusivamente con los materiales proporcionados o autorizados para la clase. No genera un vocabulario genérico de toda la asignatura y no asume bibliografía, software, versión, plataforma o sistema operativo no proporcionados o autorizados.

Entrega **como máximo 40 vocablos por bloque**. Prioriza los términos más necesarios para comprender los conceptos centrales, herramientas, interfaces, procedimientos, comandos, funciones, estructuras, resultados, prácticas y lecturas de la clase. Si existen más términos relevantes, el usuario puede pedir `siguiente` para obtener otro bloque sin repeticiones.

La lista inicial utiliza definiciones mínimas orientadas a la clase; el desarrollo detallado se realiza solamente para los términos seleccionados por el usuario. Cada término debe mantener trazabilidad con al menos uno de los materiales utilizados.

Antes de cada tanda, el agente identifica la **bibliografía realmente utilizada** y presenta las referencias en **formato APA 7** cuando existan datos suficientes y verificables. No debe inventar autores, fechas, títulos, ediciones, editoriales, DOI, URL, capítulos ni páginas para completar referencias. Cuando corresponda, también conserva la ubicación concreta de la lectura y puede emplear cita abreviada autor-fecha al desarrollar términos seleccionados.

Los agentes deben respetar la metodología de **construcción de clases** y las reglas permanentes del proyecto.