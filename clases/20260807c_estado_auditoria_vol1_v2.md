# Estado de auditoría y continuidad — Volumen 1 — 07/08/2026

## Propósito

Este registro resume el estado más reciente del **Volumen 1 de Cuadernos de Informática Aplicada — Informática Aplicada 2026** después del control de calidad académico y de las correcciones incorporadas al PDF.

Debe leerse junto con:

- `clases/20260807a_estado_material_clase_inicial_v1.md`, que conserva el estado histórico de la clase inicial;
- `misiones/clase20260807a_actualizacion_20260807c_auditoria.md`, que documenta en detalle los hallazgos y decisiones derivados de la auditoría;
- `misiones/clase20260807a_actualizacion_20260807d_autoria_portada.md`, que registra la actualización de autoría y portada;
- `misiones/clase20260807a_cierre_final_20260807e.md`, que formaliza el cierre operativo de la misión de preparación de la clase del 08/08/2026.

## Última compilación recibida

Archivo: `main.pdf`

- páginas: **21**;
- SHA-256: `c99a3dd5d86631573607936ad047498af768a33670eb8025539226e5772d9183`.

`main.tex` continúa bajo edición directa del usuario y no debe modificarse, sobrescribirse, subirse ni commitearse sin autorización expresa y específica.

## Nuevos bloques incorporados

La compilación de 21 páginas incorpora:

- calendario académico del periodo;
- calendario de clases;
- explicación del feriado del 15/08/2026;
- carga académica de la asignatura;
- explicación del significado del trabajo con acompañamiento docente y del trabajo independiente.

La tabla de carga académica actualmente muestra:

| Sigla | Valor |
|---|---:|
| HT | 2 h |
| HP | 2 h |
| HTD | 4 h |
| HTI | 4 h |
| HS | 8 h |
| THTD | 72 h |
| THTI | 72 h |
| THA | 144 h |
| CA-PY | 5 |

El documento vincula estas horas con el Reglamento específico del sistema de créditos académicos de carreras de grado de la FP-UNA, Resolución 25/10/15-00.

## Auditoría: estado de resolución

### Resuelto o sustancialmente atendido

- **Matriz de carga horaria:** ya está visible y explicada para el estudiante.
- **Trabajo independiente:** se aclara su finalidad académica y su relación con las evidencias, revisión y síntesis.
- **Cierre institucional del 21/11/2026:** la fecha ya se menciona expresamente y se diferencia del cronograma del planeamiento.
- **Fórmula final:** se conserva `EF × 0,4 + PEP × 0,6`.

### Pendientes

1. **21/11/2026:** confirmar si debe existir una actividad efectiva de Informática Aplicada ese sábado. No inventar taller o clase sin respaldo institucional.
2. **18 semanas / 144 h / 27 h / 5 CA-PY:** completar la trazabilidad institucional exacta de estos cuatro parámetros, especialmente la asignación de 5 CA-PY.
3. **Feriado del 15/08:** corregir la cita literal `(paraguay2025ley7544)` y asegurar la existencia de la entrada correspondiente en `referencias.bib`.
4. **Segunda etapa:** permanece pendiente la decisión sobre cuáles dos de las tres actividades actualmente listadas conservarán carácter sumativo.
5. **Transversalidad:** las fuentes oficiales ya están localizadas, pero el párrafo correspondiente todavía no aparece en el PDF de 21 páginas.

## Perfiles de egreso oficiales localizados

Para contextualizar Informática Aplicada sin alterar su núcleo común se utilizarán las páginas oficiales de FP-UNA:

- Ingeniería en Marketing — `https://www.pol.una.py/carreras/imk/`;
- Ingeniería en Sistemas de Producción — `https://www.pol.una.py/carreras/isp/`;
- Ingeniería en Electrónica — `https://www.pol.una.py/carreras/iek/`.

Claves bibliográficas propuestas para la próxima versión de `referencias.bib`:

- `fpunaPerfilMarketing`;
- `fpunaPerfilProduccion`;
- `fpunaPerfilElectronica`.

La contextualización pedagógica puede resumirse así:

- Marketing: datos, gráficos e información para apoyar decisiones;
- Sistemas de Producción: procesos, productividad y análisis;
- Electrónica: datos, documentación y herramientas informáticas relacionadas con sistemas y tecnologías.

El criterio es mantener una **base común para las tres carreras** y variar ejemplos o actividades cuando sea pedagógicamente pertinente, apoyándose siempre en los perfiles institucionales publicados por FP-UNA.

## Autoría y portada — actualización posterior

La autoría prevista del Volumen 1 queda integrada por:

1. **Roger Román Armoa García**;
2. **Hilda Echegaray de Palacios**;
3. **Víctor Hugo Santacruz Delvalle**.

La próxima compilación debe mantener esta autoría de forma coherente en portada, metadatos de LaTeX, página legal y demás elementos editoriales pertinentes.

Se preparó durante la sesión una nueva portada gráfica en formato PNG con los tres nombres bajo la denominación **Autores**. El archivo generado tiene dimensiones **1024 × 1536 px** y SHA-256 `74ae39c3e23bd3e26a9ad5f0f251d36476ee6b5ee5c6f3ed929a7436428d9d8d`.

La imagen no fue incorporada al repositorio. Antes de versionar recursos gráficos nuevos debe considerarse la lista de exclusión de archivos que el usuario definirá para GitHub.

`main.tex` continúa bajo control directo del usuario; la actualización de autoría en el fuente se realiza manualmente salvo autorización expresa posterior.

## Bibliografía versionada

La copia histórica continúa en:

`recursos/bibliografia/20260807a_referencias_cuaderno_vol1_v1.bib`

No sobrescribirla. Cuando el usuario entregue una nueva compilación que incluya efectivamente las referencias de perfiles, el reglamento, el calendario y la referencia del feriado correctamente resuelta, crear una **nueva versión bibliográfica** en lugar de modificar el snapshot `v1`.

## Metodología

La incorporación de ejemplos por carrera y los demás ajustes derivados de la auditoría deben seguir la metodología de **construcción de clases**: estructura inicial del docente, construcción estudiantil de la base de conocimientos y matriz de información, discusión y validación conjunta, integración de texto, gráficos y videos, y síntesis personal antes del cierre de cada clase.

## Cierre operativo de la misión

La misión de preparación de la clase inicial prevista para el **08/08/2026** queda **formalmente concluida** mediante:

`misiones/clase20260807a_cierre_final_20260807e.md`

Los pendientes enumerados en este documento quedan transferidos a futuras misiones de revisión editorial, curricular o de continuidad del Volumen 1 y **no se consideran bloqueantes para el desarrollo de la clase inicial**.

Las reglas permanentes de estilo, control de `main.tex`, exclusión de archivos auxiliares de Git y metodología de construcción de clases continúan vigentes después del cierre.
