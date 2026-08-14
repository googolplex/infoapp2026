# Misión 20260814a — Formación de vocabulario

**Agente / disparador:** `vocabulario feliz`  
**Estado:** misión activa en construcción.  
**Fecha de inicio:** 14/08/2026.

## Objetivo

Definir un método reusable para formar vocabulario relevante en **cualquier asignatura y para cada unidad de estudio**, sin incorporar contenidos, ejemplos, términos ni bibliografía propios de una disciplina específica dentro de la misión.

El contenido concreto debe surgir siempre de la unidad identificada y de la bibliografía realmente disponible para esa unidad.

La salida normal se organiza en **tandas de alrededor de 40 vocablos por vez**, sin definiciones ni desarrollos automáticos.

## Activación

Cuando el usuario escriba o invoque claramente:

`vocabulario feliz`

se activa el agente definido en:

`agentes/vocabulario_feliz.md`

## Método general

### 1. Identificar la unidad

Usar el planeamiento, programa o documento equivalente para determinar la unidad, tema o subtema que corresponde trabajar.

Si no existe una fuente suficiente para identificarla, pedir al usuario que agregue el documento necesario y detener el proceso hasta recibir aviso.

### 2. Identificar la bibliografía relacionada

Localizar la bibliografía asociada con la unidad.

Cuando existan datos suficientes, expresar la referencia en **APA 7**. No inventar datos faltantes.

El documento de planificación sirve para identificar la unidad y orientar hacia la bibliografía; no debe sustituir automáticamente la obra de lectura.

### 3. Verificar disponibilidad

Comprobar si la obra bibliográfica está realmente disponible entre las fuentes en una forma que permita inspeccionarla.

Si no está disponible, pedir al usuario que la agregue y detener el proceso.

Mientras la obra no esté disponible, no inventar bibliografía, no sustituirla automáticamente por otra y no formar vocabulario desde conocimiento general o memoria.

### 4. Determinar qué parte leer

Inspeccionar la obra disponible y localizar el capítulo, sección, apartado o páginas directamente relacionados con la unidad.

La salida puede indicar brevemente, una sola vez antes de la tanda:

- referencia APA;
- fuente o archivo disponible;
- capítulo o sección verificable;
- páginas, cuando puedan comprobarse.

Si una ubicación no puede verificarse, indicarlo en lugar de inferirla.

### 5. Extraer vocablos pertinentes

Seleccionar únicamente términos que ayuden a comprender el contenido propio de la unidad y que estén respaldados por la bibliografía realmente inspeccionada.

Pueden incluir conceptos centrales, lenguaje técnico o disciplinar, distinciones necesarias, procesos, relaciones, métodos, objetos, fenómenos o resultados pertinentes a la unidad.

No incluir términos solo porque aparezcan repetidamente en la fuente.

### 6. Presentar una tanda de alrededor de 40 vocablos

La salida normal debe contener aproximadamente **40 términos**.

La cantidad es orientativa: si no existen alrededor de 40 vocablos pertinentes y respaldados, presentar únicamente los disponibles. No inventar, forzar ni introducir términos marginales para completar la cantidad.

La tanda debe presentar **solo los vocablos**, preferentemente numerados o en formato compacto.

No incluir automáticamente:

- definiciones;
- explicaciones;
- ejemplos;
- resúmenes individuales;
- desarrollos conceptuales de cada término.

### 7. Generar tandas posteriores sin repeticiones

Cuando el usuario pida una nueva lista, otros vocablos, otros 40 o una solicitud equivalente, generar una nueva tanda de aproximadamente 40 términos.

Comparar los candidatos con todas las tandas anteriores de esa misma unidad que estén verificablemente disponibles en el contexto de la interacción.

No repetir vocablos ya presentados.

Si quedan menos de 40 términos nuevos, pertinentes y respaldados, presentar únicamente los disponibles. No completar con repeticiones ni con términos inventados.

Si las listas anteriores no están disponibles en el contexto, no afirmar que se verificó la ausencia total de repeticiones más allá de las tandas accesibles.

### 8. Control de pertinencia

Antes de presentar cada vocablo, comprobar:

1. que aparezca o se desarrolle en la bibliografía inspeccionada;
2. que esté directamente relacionado con la unidad;
3. que contribuya a comprender el contenido de esa unidad;
4. cuando corresponda a una tanda posterior, que no haya sido presentado previamente en las listas verificables de esa unidad.

Si alguna condición necesaria no puede sostenerse, excluir el término.

### 9. Explicar o definir solo cuando el usuario lo pida

Después de presentar una tanda, puede preguntarse:

**¿Quieres que te explique o defina alguno de estos vocablos?**

No adelantar automáticamente las definiciones.

Cuando el usuario pregunte por uno o varios vocablos, explicarlos apoyándose en la bibliografía inspeccionada y sin inventar información ni referencias.

### 10. Preguntas independientes

El estudiante puede preguntar por cualquier concepto no incluido en el vocabulario de estudio. La respuesta debe tratarse como consulta independiente y no convertir automáticamente ese concepto en vocabulario de la unidad.

## Neutralidad disciplinar

La misión no debe fijar:

- términos propios de una asignatura;
- ejemplos temáticos específicos;
- bibliografías predeterminadas;
- autores obligatorios;
- listas cerradas de vocabulario.

Cada ejecución debe construir el vocabulario a partir de la unidad y de las fuentes disponibles en ese contexto.

## Reglas de evidencia

- La unidad debe identificarse desde una fuente verificable.
- La bibliografía debe estar disponible antes de extraer vocablos.
- Los vocablos deben provenir de una obra realmente inspeccionada.
- Las tandas posteriores deben excluir los vocablos ya presentados cuando las listas anteriores sean verificables.
- No inventar referencias APA, capítulos, páginas ni términos atribuidos a materiales no leídos.
- No sustituir automáticamente una fuente ausente por otra.

## Metodología de construcción de clases

La misión aplica la metodología de **construcción de clases**: el docente aporta el esqueleto y las fuentes iniciales; los estudiantes construyen la base de conocimientos y vocabulario desde lecturas reales; la información se discute y valida con los docentes; pueden utilizarse texto, gráficos y videos; y cada estudiante realiza una síntesis personal.

## Criterios de aceptación

El protocolo cumple su misión cuando:

- puede reutilizarse sin cambios temáticos en distintas asignaturas;
- identifica la unidad desde evidencia disponible;
- identifica o solicita la bibliografía relacionada;
- no continúa si la bibliografía necesaria no está disponible;
- determina qué parte de la obra conviene leer;
- entrega normalmente alrededor de 40 vocablos por tanda;
- no desarrolla automáticamente los términos;
- evita repetir vocablos en tandas posteriores cuando las listas anteriores son verificables;
- no fuerza la cantidad de 40 si la fuente no permite sostenerla;
- extrae vocablos de la fuente realmente inspeccionada;
- ofrece explicación o definición solo cuando el usuario la solicita;
- no incorpora contenidos específicos de una disciplina en sus reglas permanentes.

## Restricciones

- No modificar `main.tex` sin autorización expresa y específica del usuario.
- No inventar contenido académico, citas ni referencias.
- No utilizar datos personales o reservados.
- No sustituir automáticamente bibliografía ausente por otra fuente.
