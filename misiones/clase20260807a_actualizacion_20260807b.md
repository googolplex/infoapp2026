# Actualización de la misión clase20260807a — 07/08/2026

## Propósito

Registrar la versión más reciente del material de la primera clase de Informática Aplicada 2026 sin reescribir el cierre histórico de `misiones/clase20260807a.md`.

Esta actualización complementa la misión original y debe leerse junto con `clases/20260807a_estado_material_clase_inicial_v1.md`.

## Archivos recibidos en esta actualización

El usuario entregó nuevamente los fuentes LaTeX y la compilación PDF del Volumen 1:

- `main.tex`;
- `main_v03.tex`;
- `main.pdf`;
- `20260807b_infoapp20206b.pdf`.

Los dos archivos LaTeX recibidos son idénticos entre sí y tienen la huella SHA-256:

`79ae99e63e6faa5de272480daa575f733ad5a45771f048908a7c79dbb8b129a5`

Los dos PDF recibidos son idénticos entre sí y tienen la huella SHA-256:

`e20939c6b9019bdfb222a898683d39e5d0d581a9c2d43f02b42e14bf2f355711`

La compilación actual contiene **19 páginas**.

`main.tex` continúa bajo control directo del usuario. Su recepción en esta actualización no autoriza a modificarlo, sobrescribirlo, subirlo ni realizar commits sobre él.

## Nuevos contenidos incorporados al PDF

### Calendario de evaluaciones

El PDF incorpora un apéndice visual denominado **Calendario de evaluaciones**, con diferenciación cromática entre etapas, evaluaciones parciales y finales.

El estado actualmente publicado en el PDF es:

| Etapa | Fecha | Instancia | Peso indicado |
|---|---|---|---:|
| Primera | 22/08/2026 | Actividad Sumativa 1: pioneros y evolución de la informática | 25 % |
| Primera | 05/09/2026 | Actividad Sumativa 2: informe sobre sistemas operativos | 25 % |
| Primera | 19/09/2026 | Evaluación de primera etapa | 50 % |
| Segunda | 03/10/2026 | Actividad Sumativa 3: planilla dinámica con análisis de datos | 20 % |
| Segunda | 10/10/2026 | Actividad Sumativa 4: presentación digital con elementos multimedia | 15 % |
| Segunda | 17/10/2026 | Actividad Sumativa 5: informe sobre Internet y ciberseguridad | 15 % |
| Segunda | 14/11/2026 | Evaluación de segunda etapa | 50 % |
| Final | 05/12/2026 | Primera evaluación final | — |
| Final | 19/12/2026 | Segunda evaluación final | — |

Se mantiene la fórmula final confirmada:

`EF × 0,4 + PEP × 0,6`.

### Pendiente sobre la cantidad de sumativas

El usuario indicó como modalidad deseada **dos tareas sumativas más el examen de etapa en la primera etapa, y dos tareas sumativas más el examen de etapa en la segunda etapa**, seguidas por dos evaluaciones finales.

La primera etapa del PDF ya responde a ese esquema. La segunda etapa del PDF todavía contiene **tres** actividades sumativas, distribuidas el 03/10, 10/10 y 17/10. No eliminar ni reclasificar ninguna de ellas por inferencia: queda pendiente decidir cuáles dos conservarán carácter sumativo en la modalidad definitiva.

### Aula virtual en EDUCA

El PDF incorpora un apéndice prominente con el aula virtual oficial utilizada para esta sección de Informática Aplicada:

`https://grado.pol.una.py/course/view.php?id=8662`

La contraseña de matriculación **no debe publicarse en el PDF ni registrarse en el repositorio**. El docente la proporciona directamente a los estudiantes durante la clase en el laboratorio.

Esta separación permite que el PDF pueda circular, conservarse y utilizarse como fuente documental en NotebookLM sin divulgar una credencial operativa de matriculación.

## Uso del PDF como fuente para NotebookLM

El material se diseña con doble finalidad:

1. ser legible directamente por el estudiante como documento breve de consulta y orientación;
2. poder incorporarse como fuente a NotebookLM para realizar consultas sobre organización de la asignatura, calendario, recursos, procedimientos y contenidos documentados.

Por este motivo se priorizan títulos explícitos, tablas con fechas identificables, enlaces completos, formulaciones autosuficientes y distinción entre información permanente, operativa y pendiente.

## Metodología

Los nuevos elementos se mantienen vinculados con la metodología de **construcción de clases**: el docente proporciona la estructura inicial; los estudiantes construyen y alimentan la base de conocimientos y la matriz de información; el contenido se discute y valida conjuntamente; se integran texto, gráficos y videos cuando corresponde; y cada estudiante elabora una síntesis personal antes del cierre de la clase.

## Observaciones de continuidad

- El PDF actual ya contiene los apéndices `C. Calendario de evaluaciones` y `D. Aula virtual en EDUCA`.
- El calendario coloreado compila correctamente con `xcolor` y `colortbl` en el entorno actual de LaTeX.
- El nombre corregido del archivo es `20260807b_infoapp20206b.pdf`. La huella SHA-256 coincide con la versión previamente recibida y con `main.pdf`, por lo que la corrección corresponde al nombre del archivo y no al contenido del PDF.
- La misión original conserva su valor histórico; este documento registra la actualización posterior y evita perder trazabilidad.
