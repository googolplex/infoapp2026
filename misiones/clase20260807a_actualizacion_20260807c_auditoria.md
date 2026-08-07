# Actualización de la misión clase20260807a — auditoría y perfiles de egreso — 07/08/2026

## Propósito

Registrar el estado posterior al control de calidad académico aplicado al Volumen 1 de **Cuadernos de Informática Aplicada — Informática Aplicada 2026**, las correcciones ya incorporadas al PDF y los pendientes que todavía requieren verificación o incorporación manual.

Este documento complementa:

- `misiones/clase20260807a.md`;
- `misiones/clase20260807a_actualizacion_20260807b.md`;
- `clases/20260807a_estado_material_clase_inicial_v1.md`.

La directiva sobre `main.tex` continúa vigente: **no modificar, sobrescribir, subir ni realizar commits sobre `main.tex` sin autorización expresa y específica del usuario**.

## Estado técnico más reciente recibido

El usuario entregó una nueva compilación `main.pdf` con **21 páginas**.

Huella SHA-256 de esta compilación:

`c99a3dd5d86631573607936ad047498af768a33670eb8025539226e5772d9183`

La nueva versión incorpora, además de los apéndices ya existentes, los siguientes bloques:

- `E. Calendario académico del periodo`;
- `F. Calendario de clases`;
- `G. Carga académica de la asignatura`;
- `G.1. ¿Qué significa esta carga académica?`.

## Estado de los cuestionamientos de la auditoría

### 1. Matriz de carga académica — atendido

La versión de 21 páginas ya incorpora una tabla compacta con:

- HT = 2 h;
- HP = 2 h;
- HTD = 4 h;
- HTI = 4 h;
- HS = 8 h;
- THTD = 72 h;
- THTI = 72 h;
- THA = 144 h;
- CA-PY = 5.

La explicación posterior aclara que el trabajo independiente forma parte de la dedicación académica prevista y no equivale necesariamente a una tarea rígida de cuatro horas adicionales cada semana.

El texto cita el Reglamento específico del sistema de créditos académicos de carreras de grado de la FP-UNA, Resolución 25/10/15-00, Acta 1218/19/05/2025, Anexo 01.

### 2. Calendario institucional y 21/11/2026 — omisión documental atendida; interpretación pendiente

La versión actual declara expresamente que el periodo institucional de clases se extiende hasta el **21/11/2026** y que el planeamiento de cátedra actualmente utilizado no asigna una actividad específica a ese sábado.

Por lo tanto, ya no existe una omisión silenciosa del cierre institucional. Sin embargo, **no se debe inventar una clase, taller o actividad para el 21/11** hasta contar con una confirmación institucional de que esa fecha debe contener una actividad efectiva de Informática Aplicada.

La afirmación del informe de auditoría según la cual existiría un déficit automático de cuatro semanas no queda demostrada únicamente por el calendario y el planeamiento disponibles. Debe mantenerse diferenciada de los hechos documentados.

### 3. Relación entre 18 semanas, 144 horas, 27 h/CA-PY y 5 créditos — pendiente de trazabilidad completa

El documento ya explica que el reglamento institucional contempla **18 semanas de actividades académicas, incluidas evaluaciones parciales y finales**, y utiliza un normalizador de **27 horas de trabajo académico por crédito**.

Permanece pendiente documentar de manera primaria y sin inferencias la relación exacta entre:

- 18 semanas académicas;
- 144 horas totales de la asignatura;
- normalizador de 27 h/CA-PY;
- asignación de 5 CA-PY a Informática Aplicada.

Los valores no deben presentarse como resultado de una división realizada por el equipo docente. Los 5 CA-PY deben quedar trazados a la fuente curricular oficial que los asigna a la materia o a la regla institucional específica de cálculo/redondeo correspondiente.

### 4. Transversalidad por carrera — fuentes oficiales localizadas; incorporación al PDF pendiente

Para responder al hallazgo de transversalidad de carrera se localizaron en el sitio web oficial de FP-UNA los perfiles institucionales de las tres carreras atendidas por la asignatura:

- Ingeniería en Marketing: `https://www.pol.una.py/carreras/imk/`;
- Ingeniería en Sistemas de Producción: `https://www.pol.una.py/carreras/isp/`;
- Ingeniería en Electrónica: `https://www.pol.una.py/carreras/iek/`.

Estas fuentes permiten justificar una contextualización breve de las actividades sin crear tres programas diferentes:

- **Marketing:** datos, gráficos e información para apoyar decisiones;
- **Sistemas de Producción:** procesos, productividad y análisis;
- **Electrónica:** datos, documentación y herramientas informáticas relacionadas con sistemas y tecnologías.

Se propusieron las siguientes claves bibliográficas para una futura versión de `referencias.bib`:

- `fpunaPerfilMarketing`;
- `fpunaPerfilProduccion`;
- `fpunaPerfilElectronica`.

La incorporación textual propuesta para `main.tex` debe mantenerse breve y con tono cercano al estudiante, indicando que Informática Aplicada conserva una base común pero contextualiza ejemplos y actividades según los perfiles de egreso oficiales de FP-UNA.

**Estas tres referencias todavía no aparecen en la bibliografía de la compilación `main.pdf` de 21 páginas; por tanto, no se actualiza todavía la copia bibliográfica versionada del repositorio.** Cuando el usuario entregue una compilación en la que ya estén incorporadas, registrar una nueva versión de la bibliografía en lugar de sobrescribir el snapshot histórico `v1`.

### 5. Referencia al feriado del 15/08/2026 — corrección técnica pendiente

En la versión de 21 páginas aparece literalmente el texto `(paraguay2025ley7544)` en el calendario académico y en la tabla de clases, en lugar de una cita bibliográfica resuelta.

La entrada tampoco aparece en la bibliografía final de esta compilación.

En una próxima revisión manual de `main.tex` debe utilizarse la clave bibliográfica mediante el comando de cita correspondiente —por ejemplo, `\parencite{paraguay2025ley7544}`— y comprobar que la entrada exista efectivamente en `referencias.bib`.

## Fuentes oficiales nuevas para transversalidad

Para la siguiente iteración bibliográfica se propone conservar:

```bibtex
@online{fpunaPerfilMarketing,
  author  = {{Universidad Nacional de Asunción, Facultad Politécnica}},
  title   = {Ingeniería en Marketing},
  url     = {https://www.pol.una.py/carreras/imk/},
  urldate = {2026-08-07},
  note    = {Información institucional y perfil del egresado de la carrera},
  langid  = {spanish}
}

@online{fpunaPerfilProduccion,
  author  = {{Universidad Nacional de Asunción, Facultad Politécnica}},
  title   = {Ingeniería en Sistemas de Producción},
  url     = {https://www.pol.una.py/carreras/isp/},
  urldate = {2026-08-07},
  note    = {Información institucional y perfil del egresado de la carrera},
  langid  = {spanish}
}

@online{fpunaPerfilElectronica,
  author  = {{Universidad Nacional de Asunción, Facultad Politécnica}},
  title   = {Ingeniería en Electrónica},
  url     = {https://www.pol.una.py/carreras/iek/},
  urldate = {2026-08-07},
  note    = {Información institucional y perfil del egresado de la carrera},
  langid  = {spanish}
}
```

## Criterio de cierre de la auditoría

El estado actual puede considerarse **sustancialmente mejorado**, pero la auditoría no debe declararse completamente cerrada hasta que se verifiquen o incorporen los siguientes puntos:

1. resolver bibliográficamente `paraguay2025ley7544`;
2. incorporar la contextualización breve de las tres carreras con sus fuentes oficiales;
3. completar la trazabilidad institucional de `144 h / 27 h / 5 CA-PY`;
4. confirmar, si corresponde, el tratamiento académico del sábado 21/11/2026;
5. mantener pendiente la decisión docente sobre cuáles dos actividades conservarán carácter sumativo en la segunda etapa.

## Metodología

Toda corrección derivada de la auditoría debe mantenerse integrada con la metodología de **construcción de clases**: el docente presenta un esqueleto inicial; los estudiantes construyen la base de conocimientos y alimentan la matriz de información; los contenidos se contrastan, discuten y validan; se incorporan texto, gráficos y videos cuando corresponda; y cada estudiante realiza una síntesis personal antes de finalizar la clase.
