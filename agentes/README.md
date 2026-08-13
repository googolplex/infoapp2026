# Agentes del proyecto

Esta carpeta contiene protocolos operativos reutilizables de Informática Aplicada 2026.

## `entrega_informe`

Archivo: `agentes/entrega_informe.md`

Disparador: `entrega_informe`

Función: preparar la identificación, nomenclatura, estructura y contenido validado de un informe de entrega en TXT y, cuando se solicite, en PDF.

Al iniciar un informe, el agente debe obtener explícitamente para la interacción actual: nombre completo del alumno, tema, asignatura, carrera, sección, nombre del docente, universidad y facultad. No debe inferir ni reutilizar los datos institucionales o académicos desde conversaciones anteriores, GitHub, otros informes u otro contexto.

La nomenclatura utiliza `YYYYMMDD<letra>_nombre_del_alumno_tema`, con letras secuenciales por día (`a`, `b`, `c`, ...). El TXT y el PDF del mismo informe conservan la misma letra.

El agente debe conservar fielmente el texto del alumno: salvo solicitud explícita, solo puede aplicar correcciones ortográficas, de forma de palabra conforme al diccionario y gramaticales que no alteren el significado.

Los agentes deben respetar la metodología de **construcción de clases** y las reglas permanentes del proyecto.