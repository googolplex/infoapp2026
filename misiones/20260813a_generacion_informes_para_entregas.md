# Misión 20260813a — Generación de informes para entregas

Objetivo: definir un estándar verificable para informes académicos de entrega en Informática Aplicada 2026, coherente con la metodología de construcción de clases, las reglas de evaluación vigentes y `quality control protocol`.

La misión debe producir requisitos generales, una estructura base, una plantilla reutilizable y una lista de cotejo, distinguiendo requisitos confirmados de requisitos particulares de cada actividad.

## Regla 1 confirmada — nombre del PDF y del TXT

Todo informe presentado en formato PDF debe utilizar:

`YYYYMMDDa_nombre_del_alumno_tema.pdf`

La versión textual aprobada previa al PDF debe utilizar:

`YYYYMMDDa_nombre_del_alumno_tema.txt`

Cada palabra del nombre del alumno y cada palabra del tema debe separarse mediante `_`, sin espacios.

La regla completa se registra en `reglas/20260813a_requisitos_informes_estudiantes_v1.md`.

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

1. obtener el nombre completo del alumno y el tema del informe;
2. construir los nombres previstos `.txt` y `.pdf`;
3. solicitar al estudiante los contenidos correspondientes a:
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
4. componer una propuesta completa de informe preservando el contenido aportado por el alumno;
5. mostrar la composición al alumno y solicitar aprobación explícita;
6. si existen correcciones, incorporarlas y volver a solicitar aprobación;
7. solamente después de una aprobación positiva, generar el TXT correspondiente;
8. utilizar posteriormente ese contenido aprobado como base para el PDF final cuando se solicite.

El agente no debe inventar datos, experiencias, evidencias, resultados, fuentes, autoría o conclusiones personales. Tampoco debe afirmar que un archivo fue cargado a Google Drive sin confirmación de una herramienta conectada.

## Entregables

- `reglas/20260813a_requisitos_informes_estudiantes_v1.md`;
- `recursos/20260813a_plantilla_informe_entrega_v1.md`;
- `evaluaciones/20260813a_lista_cotejo_informe_entrega_v1.md`.

## Límites actuales

No fijar arbitrariamente páginas, tipografía, márgenes, estilo bibliográfico o ponderaciones. Esos elementos se incorporarán únicamente cuando exista una decisión o consigna que los establezca.

## Metodología

Los informes se integran a la metodología de **construcción de clases**: estructura inicial del docente, construcción estudiantil de conocimientos y evidencias, composición organizada del contenido, discusión y validación, integración de texto, gráficos y videos cuando corresponda y síntesis personal. La aprobación previa del alumno forma parte explícita de la etapa de validación antes de generar la versión textual definitiva.