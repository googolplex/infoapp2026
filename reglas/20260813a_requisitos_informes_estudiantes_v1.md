# Requisitos para informes de estudiantes — versión 1

**Proyecto:** Informática Aplicada 2026  
**Estado:** en construcción; reglas confirmadas y reglas específicas diferenciadas

## 1. Nombre del archivo PDF

Todo informe presentado en formato PDF debe utilizar:

`YYYYMMDDa_nombre_del_alumno_tema.pdf`

- `YYYYMMDD`: fecha de entrega; si no existe otra fecha indicada, fecha local del día de ejecución.
- `a`: letra literal `a`.
- `nombre_del_alumno`: nombre proporcionado durante la interacción, sustituyendo espacios por `_`.
- `tema`: tema del informe, sustituyendo espacios por `_`.
- `.pdf`: extensión en minúsculas.

No se establecen todavía reglas adicionales sobre mayúsculas/minúsculas, eliminación de tildes, abreviación de nombres o reducción del tema.

Para construir correctamente este nombre, el agente `entrega_informe` debe obtener de forma explícita tanto el **nombre completo del alumno** como el **tema del informe** antes de generar el nombre final del archivo.

## 2. Formato de entrega

Cuando la consigna indique un informe en PDF, el archivo final de entrega debe ser PDF y utilizar la nomenclatura anterior.

La primera clase utiliza una carpeta compartida de Google Drive para recopilar evidencias. El enlace concreto es operativo y puede variar, por lo que no forma parte permanente de esta regla.

## 3. Identificación

El informe debe identificar claramente al estudiante y la actividad o tema. Cuando corresponda, puede incluir carrera y otros datos académicos necesarios para reconocer la entrega.

No incorporar datos personales que no sean necesarios para la actividad.

## 4. Estructura base

Salvo que la consigna disponga otra estructura, utilizar como base:

1. identificación de la entrega;
2. objetivo;
3. desarrollo;
4. evidencias;
5. análisis o comparación, cuando corresponda;
6. síntesis personal o conclusiones;
7. fuentes y declaración de uso de IA, cuando corresponda.

No fijar por inferencia cantidad de páginas, tipografía, márgenes, estilo bibliográfico o ponderación.

## 5. Evidencias y síntesis personal

El informe debe incorporar las evidencias exigidas por la actividad. Pueden ser capturas, imágenes, tablas, gráficos, resultados, archivos complementarios u otras pruebas pertinentes.

La entrega debe cerrar con una síntesis personal del aprendizaje o de los resultados, coherente con la metodología de construcción de clases.

## 6. Integridad de archivos en carpetas compartidas

Cada estudiante debe manipular únicamente sus propios archivos. No debe mover, reemplazar ni eliminar trabajos de otros estudiantes.

Cuando el archivo funcione como evidencia del proceso, se recomienda conservar una copia íntegra y actualizada de respaldo.

## 7. Privacidad y firma manuscrita

En carpetas compartidas o de acceso amplio no debe solicitarse ni incorporarse una imagen digitalizada de la firma manuscrita real del estudiante.

Cuando una práctica requiera trabajar con eliminación de fondo u otro tratamiento gráfico semejante, debe utilizarse una firma ficticia, un trazo de práctica u otro elemento creado para el ejercicio.

## 8. Uso de inteligencia artificial

Cuando se utilice IA en la actividad o en la preparación del informe:

- verificar información y fuentes;
- declarar el uso realizado cuando corresponda;
- proteger datos personales y reservados;
- mantener evidencia de aprendizaje propia;
- no inventar fuentes, resultados ni contenido oficial.

## 9. Requisitos particulares de cada actividad

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

## 10. Agente asociado

El protocolo operativo se encuentra en:

`agentes/entrega_informe.md`

Al activar `entrega_informe`, la primera respuesta debe solicitar conjuntamente el nombre completo del alumno y el tema del informe. Si uno de esos datos ya fue proporcionado y el otro falta, debe solicitar únicamente el faltante. Después se determina la fecha, se construye el nombre del archivo y el agente puede mostrar la estructura o generar el informe cuando exista información suficiente.

## 11. Relación con `quality control protocol`

`entrega_informe` prepara la entrega. `quality control protocol` audita posteriormente un PDF respecto de criterios identificados. Son protocolos separados y el segundo no se activa automáticamente.

## 12. Metodología de construcción de clases

El informe se integra a la metodología de **construcción de clases**: el docente proporciona una estructura inicial; el estudiante construye y organiza conocimientos y evidencias; la información se discute y valida; se integran texto, gráficos y videos cuando corresponda; y el estudiante realiza una síntesis personal.