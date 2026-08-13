# Requisitos para informes de estudiantes — versión 1

**Proyecto:** Informática Aplicada 2026  
**Estado:** en construcción; reglas confirmadas y reglas específicas diferenciadas

## 1. Nombre de los archivos

Todo informe presentado en formato PDF debe utilizar:

`YYYYMMDDa_nombre_del_alumno_tema.pdf`

La versión textual aprobada previa al PDF debe utilizar el mismo nombre base:

`YYYYMMDDa_nombre_del_alumno_tema.txt`

Interpretación:

- `YYYYMMDD`: fecha de entrega; si no existe otra fecha indicada, fecha local del día de ejecución.
- `a`: letra literal `a`.
- `nombre_del_alumno`: nombre completo proporcionado durante la interacción.
- `tema`: tema del informe.
- Cada palabra del nombre del alumno y cada palabra del tema se separan mediante `_`, sin espacios.
- `.txt` identifica la versión textual aprobada y `.pdf` la versión PDF cuando corresponda.

No se establecen todavía reglas adicionales sobre mayúsculas/minúsculas, eliminación de tildes, abreviación de nombres o reducción del tema.

Para construir correctamente estos nombres, el agente `entrega_informe` debe obtener de forma explícita tanto el **nombre completo del alumno** como el **tema del informe**.

## 2. Título del informe

El estudiante debe proporcionar un título claro y relacionado con la actividad o tema.

## 3. Objetivo

El estudiante debe indicar qué se pretende realizar, comprobar, resolver o aprender mediante la actividad.

## 4. Introducción o contexto

El estudiante debe proporcionar la información necesaria para contextualizar el tema, problema o actividad desarrollada.

## 5. Procedimiento o metodología de trabajo

El estudiante debe describir qué hizo, con qué herramientas y en qué secuencia, con el nivel de detalle necesario para comprender y, cuando corresponda, reproducir el trabajo.

## 6. Desarrollo

El estudiante debe aportar el contenido principal del trabajo: conceptos aplicados, operaciones realizadas, decisiones tomadas, dificultades relevantes y demás información exigida por la consigna.

## 7. Evidencias

El informe debe incorporar o describir las evidencias exigidas por la actividad. Pueden ser capturas, imágenes, tablas, gráficos, resultados, archivos complementarios u otras pruebas pertinentes.

## 8. Análisis de resultados

Cuando corresponda, el estudiante debe interpretar los resultados obtenidos, explicar su significado, comparar alternativas y justificar decisiones relevantes.

## 9. Conclusiones o síntesis personal

La entrega debe cerrar con una síntesis personal del aprendizaje o de los resultados. El agente puede mejorar su redacción, pero no debe inventar conclusiones en nombre del estudiante.

## 10. Fuentes consultadas

El estudiante debe identificar las fuentes realmente utilizadas cuando corresponda. No se deben inventar referencias.

## 11. Uso de inteligencia artificial

Cuando se utilice IA en la actividad o en la preparación del informe:

- verificar información y fuentes;
- declarar el uso realizado cuando corresponda;
- proteger datos personales y reservados;
- mantener evidencia de aprendizaje propia;
- no inventar fuentes, resultados ni contenido oficial.

## 12. Autoría

El estudiante debe identificar la autoría del informe. En trabajos grupales debe poder distinguirse la contribución o evidencia individual cuando la actividad así lo requiera.

## 13. Composición y aprobación previa

El agente `entrega_informe` debe solicitar al alumno los elementos 2, 3, 4, 5, 6, 7, 8, 9, 10 y 12 antes de cerrar el informe.

Una vez reunidos los contenidos, el agente debe:

1. organizarlos en una composición coherente;
2. mejorar ortografía, gramática, puntuación y cohesión sin alterar el contenido aportado;
3. mostrar al alumno la composición completa propuesta;
4. solicitar aprobación explícita antes de generar el archivo textual definitivo;
5. si el alumno solicita cambios, incorporarlos y volver a presentar la composición;
6. solo después de una aprobación positiva, generar el archivo `YYYYMMDDa_nombre_del_alumno_tema.txt` mediante las capacidades disponibles en la conversación.

El TXT aprobado constituye la versión textual validada que puede utilizarse posteriormente como base para generar el PDF final.

## 14. Formato de entrega

Cuando la consigna indique un informe en PDF, el archivo final de entrega debe ser PDF y utilizar la nomenclatura establecida.

La primera clase utiliza una carpeta compartida de Google Drive para recopilar evidencias. El enlace concreto es operativo y puede variar, por lo que no forma parte permanente de esta regla.

## 15. Integridad de archivos en carpetas compartidas

Cada estudiante debe manipular únicamente sus propios archivos. No debe mover, reemplazar ni eliminar trabajos de otros estudiantes.

Cuando el archivo funcione como evidencia del proceso, se recomienda conservar una copia íntegra y actualizada de respaldo.

## 16. Privacidad y firma manuscrita

En carpetas compartidas o de acceso amplio no debe solicitarse ni incorporarse una imagen digitalizada de la firma manuscrita real del estudiante.

Cuando una práctica requiera trabajar con eliminación de fondo u otro tratamiento gráfico semejante, debe utilizarse una firma ficticia, un trazo de práctica u otro elemento creado para el ejercicio.

## 17. Requisitos particulares de cada actividad

Los requisitos particulares de una actividad complementan estas reglas generales y no deben generalizarse a todas las entregas.

### Primera actividad «Hola, mundo»

La primera entrega en PDF se utiliza para validar formato, identificación, generación, nomenclatura y entrega del documento.

### Práctica de eliminación de fondo

Solo cuando corresponda a esta práctica, el informe debe:

- documentar al menos tres procedimientos;
- registrar herramientas y pasos;
- aportar evidencia gráfica;
- comparar resultados;
- cerrar con una síntesis personal.

## 18. Agente asociado

El protocolo operativo se encuentra en:

`agentes/entrega_informe.md`

Al activar `entrega_informe`, el agente obtiene nombre y tema, solicita los componentes definidos para el informe, prepara una composición provisional, solicita aprobación y, tras la aprobación, genera el TXT correspondiente. Posteriormente puede producirse el PDF final cuando se solicite y exista contenido validado suficiente.

## 19. Relación con `quality control protocol`

`entrega_informe` prepara la entrega. `quality control protocol` audita posteriormente un PDF respecto de criterios identificados. Son protocolos separados y el segundo no se activa automáticamente.

## 20. Metodología de construcción de clases

El informe se integra a la metodología de **construcción de clases**: el docente proporciona una estructura inicial; el estudiante construye y organiza conocimientos, contenidos y evidencias; la información se compone, discute y valida; se integran texto, gráficos y videos cuando corresponda; y el estudiante realiza una síntesis personal. La aprobación previa del informe mantiene explícita la etapa de validación antes de producir la entrega definitiva.