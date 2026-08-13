# Misión 20260813a — Generación de informes para entregas

Objetivo: definir un estándar verificable para informes académicos de entrega en Informática Aplicada 2026, coherente con la metodología de construcción de clases, las reglas de evaluación vigentes y `quality control protocol`.

La misión deberá producir requisitos generales, una estructura base, una plantilla reutilizable y una lista de cotejo, distinguiendo requisitos confirmados de propuestas o aspectos pendientes de validación. Incluirá identificación, objetivo, desarrollo, evidencias, análisis de resultados, conclusiones, fuentes, autoría, evidencia individual en trabajos grupales, declaración de uso de IA, accesibilidad y formato de entrega.

No se fijarán arbitrariamente páginas, tipografía, márgenes, estilo bibliográfico ni ponderaciones. El estándar deberá ser aplicable a Marketing, Ingeniería en Sistemas de Producción e Ingeniería en Electrónica y mantener trazabilidad con `AGENTS.md`, `docs/contexto/README.md`, `docs/20260725a_Construccion_de_clases_Informatica_Aplicada_2026.pdf`, `docs/evaluacion.md`, `docs/contexto/20260727f_pendiente_transicion_modalidad_evaluacion.md`, `reglas/20260807a_criterio_editorial_materiales_deposito_institucional.md`, `reglas/20260807b_estilo_espanol_sin_voceo.md` y `reglas/20260807d_protocolo_quality_control_v1.md`.

Entregas previstas: `reglas/20260813a_requisitos_informes_estudiantes_v1.md`, `recursos/20260813a_plantilla_informe_entrega_v1.md` y `evaluaciones/20260813a_lista_cotejo_informe_entrega_v1.md`.

## Regla 1 confirmada — Nombre del archivo PDF

Todo informe presentado en formato PDF debe utilizar:

`YYYYMMDDa_nombre_del_alumno_tema.pdf`

La regla completa queda registrada en `reglas/20260813a_requisitos_informes_estudiantes_v1.md`.

## Agente operativo `entrega_informe`

Se incorpora `agentes/entrega_informe.md` como protocolo para construir el nombre correcto del archivo.

Al activar el comando `entrega_informe`, la primera respuesta debe solicitar el nombre completo del alumno. Una vez recibido, el agente determina la fecha, utiliza el tema ya conocido o lo solicita si falta, sustituye espacios por `_` y devuelve el nombre exacto del PDF que debe utilizarse para la entrega en Google Drive.

El agente no debe registrar nombres de alumnos en el repositorio.
