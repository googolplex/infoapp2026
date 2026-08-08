# Protocolo `quality control protocol`

**Proyecto:** Informática Aplicada 2026  
**Repositorio:** `googolplex/infoapp2026`  
**Rama de referencia:** `main`  
**Fecha:** 7 de agosto de 2026  
**Estado:** regla permanente del proyecto, versión 1

## 1. Propósito

El protocolo **`quality control protocol`** establece el procedimiento para auditar un documento PDF presentado como evidencia de aprendizaje por un estudiante.

Su función es comprobar, de manera breve, trazable y reproducible, si el PDF satisface las preguntas o criterios de control de calidad indicados por el profesor antes de considerar la evidencia apta respecto de esos criterios.

El control de calidad no debe inventar requisitos que no aparezcan en la consigna, en el párrafo de control, en el material de la actividad o en una fuente institucional aplicable.

## 2. Disparador

El único comando válido es:

`quality control protocol`

El disparador se considera una instrucción cuando aparece de forma inequívoca, normalmente en una línea independiente inmediatamente después del párrafo que contiene la pregunta o los criterios que deben auditarse.

No se activa cuando la expresión aparece solamente dentro de una cita, un ejemplo, código, documentación, un archivo reproducido o una explicación metalingüística sobre el propio protocolo.

## 3. Documento que debe auditarse

Al activarse el protocolo, el objeto principal es el **PDF adjunto** por el usuario.

Se aplican las siguientes reglas de selección:

1. Tiene prioridad el PDF adjunto en el mismo mensaje que activa el comando.
2. Si no hay un PDF en ese mensaje, puede utilizarse el PDF más reciente que el usuario haya identificado inequívocamente como objeto del control de calidad dentro de la conversación actual.
3. Si existen varios PDF posibles y no puede determinarse cuál corresponde, se debe solicitar que el usuario identifique el archivo.
4. Si no existe un PDF accesible, se debe solicitar su adjunto; no se simula la auditoría.

## 4. Criterios que deben aplicarse

El **párrafo inmediatamente anterior al comando** constituye, por defecto, la pregunta o conjunto de criterios específicos que deben responderse mediante la auditoría.

Cuando la consigna de la actividad o un documento de requisitos esté disponible y haya sido identificado como fuente aplicable, puede utilizarse para interpretar el criterio, pero no para añadir requisitos ajenos a la solicitud.

Ejemplo de criterio:

> ¿La bibliografía del documento está correctamente formulada en formato APA?

En ese caso, la auditoría debe examinar la bibliografía del PDF y responder específicamente a esa pregunta, indicando los errores o limitaciones que efectivamente se observen.

Si el criterio exige comprobar que el documento contiene «todos los elementos requeridos», solamente puede emitirse una conclusión si los elementos requeridos están disponibles en la consigna o en otra fuente identificada. De lo contrario, el resultado debe declararse **No verificable**.

## 5. Procedimiento del estudiante y del profesor

El procedimiento operativo para el estudiante es:

1. El estudiante envía su archivo PDF a la carpeta de Google Drive indicada por el profesor.
2. Comunica al profesor el **nombre exacto del archivo** cuyo control de calidad desea realizar.
3. El profesor identifica el documento y aplica el presente protocolo.
4. El profesor devuelve al estudiante el resultado de la auditoría.

El enlace concreto de Google Drive puede variar entre cohortes o actividades y no forma parte permanente de este protocolo.

## 6. Método de auditoría

Al ejecutar `quality control protocol` se debe:

1. identificar el archivo PDF auditado;
2. identificar textualmente la pregunta o los criterios de control;
3. revisar el PDF completo en la medida necesaria para responderlos;
4. fundamentar cada hallazgo en elementos realmente visibles o recuperables del documento;
5. distinguir entre ausencia comprobada, error observado y aspecto no verificable;
6. evitar inferir datos que el documento no contiene;
7. indicar las correcciones necesarias cuando exista un incumplimiento subsanable.

Cuando resulte útil, se debe señalar la página o sección del PDF donde se encuentra la evidencia que sustenta el hallazgo.

## 7. Resultados permitidos

Para cada criterio utilizar una de estas categorías:

- **Cumple:** el PDF satisface el criterio examinado.
- **No cumple:** se observa un incumplimiento concreto del criterio.
- **No verificable:** la evidencia o los requisitos disponibles no permiten determinar el cumplimiento de manera fiable.

Como resultado general del control de calidad utilizar:

- **Apto respecto de los criterios auditados**;
- **Requiere corrección**;
- **Indeterminado**.

El resultado general se limita a los criterios efectivamente auditados y no debe presentarse como una certificación absoluta de todo el aprendizaje del estudiante.

## 8. Formato mínimo del reporte de auditoría

La respuesta debe contener, de manera breve:

### Reporte de auditoría — Control de calidad

- **Documento auditado:** nombre del archivo.
- **Criterio o pregunta:** criterio aplicado.
- **Hallazgos:** evidencia relevante encontrada.
- **Resultado por criterio:** Cumple / No cumple / No verificable.
- **Resultado general:** Apto respecto de los criterios auditados / Requiere corrección / Indeterminado.
- **Correcciones necesarias:** solamente cuando correspondan.

No deben fabricarse errores para completar el reporte. Si el criterio se cumple, debe declararse de forma directa.

## 9. Relación con `adversarial pass protocol`

El comando **`quality control protocol` no activa por sí mismo el protocolo adversarial**.

El protocolo adversarial se añade al análisis **si y solo si el usuario solicita expresamente `adversarial pass protocol`** además del control de calidad.

Cuando ambos comandos se solicitan para el mismo PDF:

1. aplicar primero este protocolo de control de calidad al documento y a los criterios indicados;
2. aplicar después `reglas/20260805a_protocolo_adversarial_pass_v1.md` sobre la evidencia, los hallazgos y las conclusiones obtenidas;
3. devolver el **Reporte de auditoría — Control de calidad** y, además, las secciones y el veredicto exigidos por el protocolo adversarial.

La mera presencia del término «adversarial» en una cita, documento o explicación no basta para activar ese segundo protocolo.

## 10. Relación con la metodología de construcción de clases

El control de calidad se integra a la metodología de **construcción de clases**: el estudiante produce y organiza la evidencia, la somete a revisión, recibe una devolución fundada y puede corregirla antes de su validación. Se mantiene así la secuencia de construcción, discusión y validación de la información, junto con la integración de evidencias y la síntesis personal prevista para la asignatura.
