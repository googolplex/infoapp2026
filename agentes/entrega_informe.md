# Agente `entrega_informe`

## Propósito

Construir el nombre correcto de un informe PDF antes de su entrega.

## Disparador

`entrega_informe`

## Regla de nombre

Todo informe en PDF debe usar:

`YYYYMMDDa_nombre_del_alumno_tema.pdf`

- `YYYYMMDD`: fecha de entrega; si no hay una fecha explícita, usar la fecha local del día de ejecución.
- `a`: letra literal `a`.
- `nombre_del_alumno`: nombre indicado durante la interacción, sustituyendo espacios por `_`.
- `tema`: tema del informe, sustituyendo espacios por `_`.
- `.pdf`: extensión en minúsculas.

No se añaden todavía reglas de mayúsculas/minúsculas, eliminación de tildes o abreviación.

## Secuencia obligatoria

Al activarse el protocolo, la primera respuesta debe ser:

**¿Cuál es el nombre completo del alumno?**

No se debe pedir antes ningún otro dato ni construir el nombre final.

Después de recibir el nombre:

1. Determinar la fecha según la regla anterior.
2. Usar el tema ya conocido si es inequívoco.
3. Si el tema falta, preguntar: **¿Cuál es el tema del informe?**
4. Sustituir los espacios del nombre y del tema por `_`.
5. Construir `YYYYMMDDa_nombre_del_alumno_tema.pdf`.
6. Presentarlo como el nombre exacto del PDF que debe subirse a Google Drive.

El nombre del alumno se usa solo para construir el archivo de entrega y no debe registrarse en el repositorio.

## Metodología

El informe se considera una evidencia dentro de la metodología de construcción de clases: parte de la construcción estudiantil de conocimientos, su discusión y validación, la integración de texto, gráficos y videos y la síntesis personal del estudiante.
