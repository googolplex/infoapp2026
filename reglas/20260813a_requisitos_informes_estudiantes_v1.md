# Requisitos para informes de estudiantes — versión 1

**Proyecto:** Informática Aplicada 2026  
**Estado:** en construcción; primera regla confirmada

## Regla 1 — Nombre del archivo PDF

Todo informe presentado en formato PDF debe utilizar el siguiente formato de nombre:

`YYYYMMDDa_nombre_del_alumno_tema.pdf`

Interpretación:

- `YYYYMMDD`: fecha correspondiente a la entrega. Si no se ha indicado una fecha específica, el agente `entrega_informe` utiliza la fecha local del día en que se ejecuta el protocolo.
- `a`: letra literal `a` establecida por esta primera regla.
- `nombre_del_alumno`: nombre completo proporcionado durante la interacción, con los espacios sustituidos por `_`.
- `tema`: tema del informe, con los espacios sustituidos por `_`.
- `.pdf`: extensión en minúsculas.

Esta versión no establece todavía reglas adicionales sobre mayúsculas/minúsculas, eliminación de tildes, abreviación de nombres o reducción del tema.

## Agente asociado

El protocolo operativo para construir y verificar el nombre se encuentra en:

`agentes/entrega_informe.md`

Al activar `entrega_informe`, el primer dato que debe solicitarse es el nombre completo del alumno. El tema se toma del contexto si ya es inequívoco; si falta, se solicita después del nombre.

## Relación con la metodología de construcción de clases

El informe constituye una evidencia del proceso de construcción de clases: el estudiante desarrolla y organiza información, la discute y valida, integra texto, gráficos y videos cuando corresponda y produce una síntesis personal de aprendizaje.
