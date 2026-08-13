# Misión 20260813a — Generación de informes para entregas

Objetivo: definir un estándar verificable para informes académicos de entrega en Informática Aplicada 2026, coherente con la metodología de construcción de clases, las reglas de evaluación vigentes y `quality control protocol`.

La misión debe producir requisitos generales, una estructura base, una plantilla reutilizable y una lista de cotejo, distinguiendo requisitos confirmados de requisitos particulares de cada actividad.

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

Ejemplo para tres informes generados el 13/08/2026:

- `20260813a_nombre_del_alumno_tema.pdf`
- `20260813b_nombre_del_alumno_otro_tema.pdf`
- `20260813c_nombre_de_otro_alumno_tema.pdf`

El agente debe utilizar la siguiente letra disponible cuando pueda comprobar que ya se generó otro informe en la misma fecha dentro del contexto, archivos o sesión disponibles. No debe reutilizar deliberadamente una letra ya asignada a otro informe del mismo día cuando esa información sea verificable.

Si no existe evidencia disponible de un informe anterior en esa fecha, se utiliza `a`. La letra forma parte tanto del nombre del TXT aprobado como del PDF final correspondiente y debe mantenerse igual entre ambas versiones del mismo informe.

La regla completa se registra en `reglas/20260813a_requisitos_informes_estudiantes_v1.md` y debe mantenerse sincronizada con el protocolo `agentes/entrega_informe.md`.

## Regla 2 confirmada — datos de identificación académica obligatorios

Antes de componer el informe, el agente debe obtener explícitamente del alumno los siguientes datos:

1. nombre completo del alumno;
2. tema del informe;
3. asignatura;
4. carrera;
5. sección;
6. nombre del docente;
7. universidad;
8. facultad.

Estos datos forman parte de la identificación académica del informe y deben incorporarse en la composición provisional, en el TXT aprobado y en el PDF final cuando corresponda.

### Prohibición de inferencia de datos de identificación

El agente **no debe inferir, completar automáticamente ni reutilizar** la asignatura, la carrera, la sección, el nombre del docente, la universidad o la facultad a partir de:

- información general del proyecto;
- este repositorio GitHub;
- conversaciones anteriores;
- informes anteriores;
- datos de otros estudiantes;
- nombres institucionales conocidos por el agente;
- cualquier otro contexto distinto de la respuesta explícita del alumno para el informe actual.

Aunque un dato parezca evidente o coincida con el contexto de Informática Aplicada 2026, debe ser solicitado para el informe actual.

Si uno o más de estos datos ya fueron proporcionados explícitamente y de manera inequívoca durante la interacción correspondiente al informe actual, no es necesario volver a preguntarlos. El agente debe solicitar únicamente los datos faltantes.

El agente tampoco debe corregir, normalizar, ampliar o sustituir los nombres institucionales proporcionados por el alumno salvo correcciones ortográficas, de forma de palabra conforme al diccionario o gramaticales que no cambien el contenido, o salvo solicitud explícita del alumno.

## Hallazgos de la primera clase

El material de la clase inicial y sus registros de estado documentan que:

- la primera entrega en PDF funciona como «Hola, mundo» para validar formato, identificación, generación, nomenclatura y entrega;
- las evidencias se recopilan en la carpeta de Google Drive indicada por el profesor;
- cada estudiante debe manipular únicamente sus propios archivos en carpetas compartidas;
- deben protegerse los elementos sensibles en carpetas de acceso amplio;
- las actividades deben conservar evidencias y una síntesis personal;
- la práctica específica de eliminación de fondo exige al menos tres procedimientos, herramientas y pasos, evidencia gráfica, comparación de resultados y síntesis personal.

Los requisitos de la práctica de eliminación de fondo no se convierten en requisitos generales de todos los informes.

## Agente operativo `entrega_informe`

El agente se conserva en `agentes/entrega_informe.md`.

Al activar `entrega_informe`, el protocolo debe:

1. obtener explícitamente del alumno los datos de identificación del informe: nombre completo, tema, asignatura, carrera, sección, nombre del docente, universidad y facultad;
2. no inferir ninguno de esos datos desde otro contexto y solicitar únicamente los que todavía falten;
3. determinar la fecha de entrega y la siguiente letra disponible para esa fecha cuando pueda verificarse la existencia de informes anteriores;
4. construir los nombres previstos `.txt` y `.pdf` utilizando el mismo prefijo `YYYYMMDD<letra>` para ambas versiones;
5. solicitar al estudiante los contenidos correspondientes a:
   - título del informe;
   - objetivo;
   - introducción o contexto;
   - procedimiento o metodología de trabajo;
   - desarrollo;
   - evidencias;
   - análisis de resultados;
   - conclusiones o síntesis personal;
   - fuentes consultadas;
   - autoría;
6. componer una propuesta completa de informe preservando el contenido aportado por el alumno y respetando las restricciones vigentes de edición;
7. incluir en la composición provisional la identificación académica completa proporcionada por el alumno;
8. mostrar la composición al alumno y solicitar aprobación explícita;
9. si existen correcciones, incorporar únicamente las permitidas o solicitadas y volver a solicitar aprobación;
10. solamente después de una aprobación positiva, generar el TXT correspondiente;
11. utilizar posteriormente ese contenido aprobado como base para el PDF final cuando se solicite, conservando la misma letra asignada al TXT.

El agente no debe inventar datos, experiencias, evidencias, resultados, fuentes, autoría o conclusiones personales. Tampoco debe afirmar que un archivo fue cargado a Google Drive sin confirmación de una herramienta conectada.

## Entregables

- `reglas/20260813a_requisitos_informes_estudiantes_v1.md`;
- `recursos/20260813a_plantilla_informe_entrega_v1.md`;
- `evaluaciones/20260813a_lista_cotejo_informe_entrega_v1.md`.

## Límites actuales

No fijar arbitrariamente páginas, tipografía, márgenes, estilo bibliográfico o ponderaciones. Esos elementos se incorporarán únicamente cuando exista una decisión o consigna que los establezca.

## Metodología

Los informes se integran a la metodología de **construcción de clases**: estructura inicial del docente, construcción estudiantil de conocimientos y evidencias, composición organizada del contenido, discusión y validación, integración de texto, gráficos y videos cuando corresponda y síntesis personal. La solicitud explícita de los datos de identificación y la aprobación previa del alumno forman parte de la etapa de construcción y validación antes de generar la versión textual definitiva.