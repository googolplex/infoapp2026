# Misión 20260813a — Generación de informes para entregas

**Estado:** aprobada por el usuario el 13/08/2026.  
**Agente operativo:** `agentes/entrega_informe.md`.

Objetivo: definir un estándar verificable para informes académicos de entrega, coherente con la metodología de construcción de clases, las reglas de evaluación vigentes y `quality control protocol`.

La misión debe producir y mantener sincronizados requisitos generales, una estructura base, una plantilla reutilizable, una lista de cotejo y el agente operativo, distinguiendo requisitos confirmados de requisitos particulares de cada actividad.

## Regla 1 confirmada — nombre del PDF y del TXT

Todo informe presentado en formato PDF debe utilizar:

`YYYYMMDD<letra>_nombre_del_alumno_tema.pdf`

La versión textual aprobada previa al PDF debe utilizar:

`YYYYMMDD<letra>_nombre_del_alumno_tema.txt`

Cada palabra del nombre del alumno y cada palabra del tema debe separarse mediante `_`, sin espacios.

### Secuencia diaria de la letra

La letra que sigue a `YYYYMMDD` identifica el orden de los informes generados en una misma fecha.

- El primer informe generado en el día utiliza `a`.
- El segundo informe generado en el mismo día utiliza `b`.
- El tercero utiliza `c`.
- Los informes posteriores continúan con la secuencia alfabética correspondiente.
- Al cambiar la fecha, la secuencia vuelve a comenzar en `a`.

El agente debe utilizar la siguiente letra disponible cuando pueda comprobar que ya se generó otro informe en la misma fecha dentro del contexto, archivos o sesión disponibles. No debe reutilizar deliberadamente una letra ya asignada a otro informe del mismo día cuando esa información sea verificable.

Si no existe evidencia disponible de un informe anterior en esa fecha, se utiliza `a`. La letra debe mantenerse igual entre el TXT aprobado y el PDF final del mismo informe.

## Regla 2 confirmada — datos de identificación académica obligatorios

Antes de componer el informe, el agente debe obtener explícitamente del alumno:

1. nombre completo del alumno;
2. tema del informe;
3. asignatura;
4. carrera;
5. sección;
6. nombre del docente;
7. universidad;
8. facultad.

Estos datos forman parte de la identificación académica y deben incorporarse en la composición provisional, en el TXT aprobado y en el PDF final cuando corresponda.

### Prohibición de inferencia de datos de identificación

El agente **no debe inferir, completar automáticamente ni reutilizar** la asignatura, la carrera, la sección, el nombre del docente, la universidad o la facultad a partir de información general del proyecto, GitHub, conversaciones anteriores, informes anteriores, datos de otros estudiantes, nombres institucionales conocidos o cualquier otro contexto distinto de la respuesta explícita del alumno para el informe actual.

Aunque un dato parezca evidente, debe solicitarse para el informe actual. Si ya fue proporcionado explícitamente y de manera inequívoca durante esa interacción, no se vuelve a preguntar.

El agente tampoco debe normalizar, ampliar o sustituir los nombres institucionales proporcionados por el alumno salvo correcciones ortográficas, de forma de palabra conforme al diccionario o gramaticales que no cambien el contenido, o salvo solicitud explícita.

## Regla 3 confirmada — conservación del texto del alumno

El agente no debe cambiar, reinterpretar, resumir, ampliar, completar, estilizar ni reformular lo escrito por el alumno salvo solicitud explícita.

Sin esa solicitud, solo puede aplicar:

- correcciones ortográficas y de puntuación;
- correcciones de forma de palabras conforme al diccionario, sin sustitución estilística por sinónimos;
- correcciones gramaticales necesarias que no alteren el significado.

Organizar el contenido en apartados no autoriza a reescribirlo. Ante una ambigüedad que exija inferir intención, debe conservar el texto o solicitar aclaración.

## Regla 4 confirmada — bibliografía

El criterio bibliográfico del proyecto para estos informes es **APA 7**, salvo que una consigna específica establezca expresamente otro formato.

Las referencias deben construirse con datos reales y verificables. No se inventan autores, títulos, fechas, editoriales, DOI, URL u otros datos ausentes.

## Regla 5 confirmada — firma y privacidad

La imagen de firma pertenece únicamente a la versión PDF final, no al TXT, y no debe almacenarse ni versionarse en GitHub.

Antes de utilizar una firma manuscrita real debe comprobarse el nivel de acceso del mecanismo de entrega. Si la carpeta de entrega es compartida o de acceso amplio, no debe exponerse una imagen digitalizada de la firma manuscrita real; se utiliza la alternativa de identificación indicada por el docente.

Para prácticas de tratamiento de imágenes o eliminación de fondo se usa una firma ficticia, un trazo de práctica u otro elemento gráfico creado para el ejercicio.

## Agente operativo `entrega_informe`

Al activar `entrega_informe`, el protocolo debe:

1. obtener explícitamente los ocho datos de identificación académica;
2. no inferir los datos institucionales o académicos desde otro contexto;
3. determinar la fecha y la siguiente letra disponible para esa fecha cuando pueda verificarse la existencia de informes anteriores;
4. construir los nombres previstos `.txt` y `.pdf` con el mismo prefijo `YYYYMMDD<letra>`;
5. solicitar título, objetivo, introducción o contexto, procedimiento o metodología, desarrollo, evidencias, análisis de resultados, conclusiones o síntesis personal, fuentes consultadas y autoría;
6. conservar fielmente el contenido del alumno conforme a la restricción de edición aprobada;
7. incluir la identificación académica completa en la composición provisional;
8. mostrar la composición completa y solicitar aprobación explícita;
9. incorporar únicamente las correcciones permitidas o solicitadas y volver a pedir aprobación cuando corresponda;
10. generar el TXT solo después de una aprobación positiva;
11. utilizar el contenido aprobado como base del PDF final, conservando la misma letra de secuencia.

El agente no debe inventar datos, experiencias, evidencias, resultados, fuentes, autoría o conclusiones personales.

## Entregables sincronizados

- `agentes/entrega_informe.md`;
- `reglas/20260813a_requisitos_informes_estudiantes_v1.md`;
- `recursos/20260813a_plantilla_informe_entrega_v1.md`;
- `evaluaciones/20260813a_lista_cotejo_informe_entrega_v1.md`;
- `agentes/README.md`.

## Límites actuales

No fijar arbitrariamente páginas, tipografía, márgenes o ponderaciones. Esos elementos se incorporan únicamente cuando exista una decisión o consigna que los establezca.

## Metodología

Los informes se integran a la metodología de **construcción de clases**: estructura inicial del docente, construcción estudiantil de conocimientos y evidencias, composición organizada sin sustituir la voz del estudiante, discusión y validación, integración de texto, gráficos y videos cuando corresponda y síntesis personal. La solicitud explícita de los datos de identificación y la aprobación previa forman parte de la etapa de construcción y validación antes de generar la versión definitiva.