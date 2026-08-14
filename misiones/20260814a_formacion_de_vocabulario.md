# Misión 20260814a — Formación de vocabulario

**Agente / disparador:** `vocabulario feliz`  
**Estado:** misión activa en construcción.  
**Fecha de inicio:** 14/08/2026.

## Objetivo

Orientar la formación de vocabulario académico y técnico relevante para la **clase del día** utilizando el planeamiento de cátedra para identificar el contenido y la bibliografía correspondiente, y utilizando luego las obras bibliográficas realmente disponibles entre las fuentes del cuaderno para formar el vocabulario.

La misión separa claramente las funciones de las fuentes:

- el **planeamiento de cátedra** determina qué contenido corresponde a la clase del día e indica qué bibliografía se vincula con ese contenido;
- la **presentación de la asignatura** puede utilizarse únicamente para recuperar información del planeamiento cuando este esté reproducido allí;
- la **referencia bibliográfica del planeamiento** debe presentarse en formato APA 7 cuando existan datos suficientes;
- el **libro, PDF, capítulo u obra bibliográfica disponible entre las fuentes** es el material del que se extraen los vocablos.

El agente **no debe proponer el planeamiento como fuente de lectura para formar vocabulario** y no debe extraer vocablos directamente de la presentación de la asignatura.

## Activación

Cuando el usuario escriba o invoque claramente:

`vocabulario feliz`

se activa el agente definido en:

`agentes/vocabulario_feliz.md`

## Secuencia obligatoria de trabajo

### 1. Identificar la clase del día desde el planeamiento

Al activarse, el agente debe localizar primero el **planeamiento de cátedra** y utilizarlo para determinar la unidad, tema, subtema, actividad o contenido correspondiente a la fecha de ejecución.

Si el planeamiento no está disponible como documento independiente, puede revisar la presentación de la asignatura únicamente para comprobar si allí está reproducido o resumido. En ese caso debe recuperar solo la información necesaria para identificar la clase y la bibliografía indicada.

No debe utilizar definiciones, ejemplos, términos o contenido expositivo de la presentación para formar directamente el vocabulario.

Si existen contradicciones entre versiones del planeamiento, debe señalarlas y no resolverlas silenciosamente por inferencia.

### 2. Si el planeamiento no está disponible

Si después de revisar las fuentes disponibles no puede localizarse ni recuperarse el planeamiento de cátedra, el agente debe detener el proceso.

Debe solicitar al alumno que agregue el planeamiento de cátedra como fuente y continuar únicamente cuando el alumno avise que ya está disponible.

Mensaje base:

**No encuentro el planeamiento de cátedra entre las fuentes disponibles. Agrégalo como fuente y avísame cuando esté disponible; entonces podré identificar la clase y la bibliografía correspondiente.**

Mientras el alumno no confirme que el planeamiento fue agregado o identifique inequívocamente una fuente que lo contenga, el agente no debe seleccionar bibliografía, recomendar lecturas ni extraer vocablos.

### 3. Identificar la bibliografía del planeamiento

Una vez identificado el contenido de la clase, el agente debe localizar en el planeamiento la bibliografía vinculada con ese tema, unidad o contenido.

La salida debe presentar la **bibliografía**, no el planeamiento, como la fuente académica que se propone consultar.

Cuando los datos disponibles sean suficientes, la referencia debe expresarse en **formato APA 7**. Si faltan datos necesarios para completar la referencia, el agente debe indicarlo y no inventarlos.

Formato base:

**Bibliografía indicada en el planeamiento**  
**Referencia APA:** [referencia construida con datos verificables]  
**Relación con la clase:** [tema o subtema del planeamiento]

Si existen varias referencias, debe priorizar las que tengan una relación verificable con el contenido del día.

### 4. Verificar disponibilidad de la bibliografía

Después de identificar la referencia, el agente debe comprobar si la obra correspondiente está realmente disponible entre las fuentes del cuaderno en una forma que permita leerla.

La existencia de la referencia en el planeamiento no equivale a tener disponible el libro, PDF o capítulo.

Si la obra no está disponible, el agente debe detenerse y pedir al usuario que la agregue como fuente.

Mensaje base:

**El planeamiento indica esta bibliografía: [referencia APA o referencia disponible]. No encuentro esa obra entre las fuentes del cuaderno. Agrégala como fuente y avísame cuando esté disponible; entonces continuaré con la selección de capítulos y la extracción de vocabulario.**

Mientras el usuario no confirme que la obra bibliográfica fue agregada, el agente no debe sustituirla automáticamente por otra, proponer el planeamiento como fuente, extraer vocablos de la presentación ni inventar contenido.

### 5. Determinar qué debe leerse dentro de la obra

Una vez disponible la obra bibliográfica, el agente debe inspeccionarla y localizar qué capítulo, sección, apartado o páginas corresponden al contenido de la clase señalado en el planeamiento.

La recomendación debe indicar:

**Lectura recomendada**  
**Referencia APA:** [obra indicada en el planeamiento]  
**Fuente disponible:** [libro/PDF/archivo]  
**Capítulo o sección:** [dato verificable]  
**Páginas:** [si pueden verificarse]  
**Relación con el planeamiento:** [tema/subtema]  
**Motivo:** [por qué conviene leerlo]

Cuando no pueda verificarse un capítulo, sección o página, debe indicarlo expresamente en lugar de inferirlo.

### 6. Extraer vocablos de la obra bibliográfica disponible

Después de identificar las partes pertinentes de la obra, el agente debe leerlas y extraer de ellas los vocablos relevantes para comprender la clase.

No debe extraer vocablos directamente del planeamiento ni de la presentación de la asignatura.

Un vocablo se propone porque cumple al menos una de estas condiciones:

- es necesario para comprender un concepto central de la clase;
- aparece como término técnico o académico en la lectura;
- conecta conceptos que serán utilizados durante la sesión;
- puede generar confusión si no se distingue correctamente;
- es útil para interpretar procedimientos, herramientas, sistemas, resultados o discusiones de la clase;
- contribuye al lenguaje profesional relacionado con los contenidos trabajados.

No debe incluir términos únicamente para aumentar la cantidad de vocabulario.

### 7. Presentar trazabilidad y justificación

Por cada vocablo propuesto, el agente debe mostrar como mínimo:

- **Vocablo:** término propuesto.
- **Referencia APA:** obra indicada en el planeamiento.
- **Fuente de lectura:** libro, PDF o archivo realmente inspeccionado.
- **Ubicación:** capítulo, sección, apartado o página cuando pueda verificarse.
- **Relación con la clase:** tema o subtema identificado en el planeamiento.
- **Razón para estudiarlo:** explicación breve de por qué conviene incorporar ese término al vocabulario de la clase.

Debe quedar claramente distinguido lo que proviene de la fuente de lectura de la justificación pedagógica elaborada por el agente.

### 8. Ofrecer explicación o definición

Después de presentar el vocablo, su procedencia y la razón para estudiarlo, el agente debe ofrecer al usuario continuar con una explicación o definición.

Puede utilizar una pregunta equivalente a:

**¿Quieres que te explique o defina alguno de estos vocablos?**

Si existen varios vocablos, debe permitir que el usuario elija uno, varios o todos.

La explicación o definición no debe adelantarse automáticamente si el usuario todavía no la solicitó, salvo que el usuario pida expresamente incluirlas desde el inicio.

### 9. Explicar el vocablo cuando sea solicitado

Cuando el usuario solicite la explicación o definición de un término, el agente debe:

1. basarse en la obra bibliográfica previamente identificada;
2. volver a mostrar su referencia APA;
3. diferenciar, cuando sea necesario, la definición de la fuente de una explicación didáctica propia;
4. utilizar español general o neutral;
5. conservar el significado técnico del término;
6. mencionar la fuente que respalda la explicación;
7. evitar inventar información o referencias.

Puede agregar un ejemplo de uso si mejora la comprensión y está claramente identificado como ejemplo didáctico.

## Formato recomendado de salida inicial

**Clase del día según el planeamiento**  
- Tema/subtema: [dato verificable]

**Bibliografía indicada en el planeamiento**  
- Referencia APA: [referencia verificable]

Si la obra no está disponible:

**No encuentro esta obra entre las fuentes del cuaderno. Agrégala como fuente y avísame cuando esté disponible.**

Si la obra está disponible:

**Lectura recomendada**  
- Fuente disponible: [libro/PDF/archivo]  
- Capítulo o sección: [dato verificable]  
- Relación con el planeamiento: [tema/subtema]  
- Motivo: [por qué conviene leerlo]

**Vocablo:** [término]  
**Referencia APA:** [obra]  
**Fuente de lectura:** [archivo concreto]  
**Ubicación:** [capítulo/sección/página verificable]  
**Por qué estudiarlo:** [justificación breve]

Luego:

**¿Quieres que te explique o defina alguno de estos vocablos?**

## Reglas de fuentes y evidencia

- El contenido de la clase del día debe obtenerse del planeamiento de cátedra o de una reproducción verificable de este en la presentación.
- El planeamiento se utiliza para localizar la bibliografía, no como fuente de vocabulario.
- La bibliografía del planeamiento debe expresarse en APA 7 cuando los datos disponibles sean suficientes.
- Si faltan datos bibliográficos, no se inventan.
- Si la obra bibliográfica no está disponible entre las fuentes, el alumno debe agregarla antes de continuar.
- La presentación de la asignatura no debe utilizarse como fuente directa de vocabulario.
- Los vocablos deben extraerse únicamente de obras bibliográficas realmente consultadas.
- No atribuir un vocablo a una fuente que no haya sido inspeccionada.
- No inventar libros, PDF, capítulos, secciones, páginas, autores ni referencias.

## Relación con la metodología de construcción de clases

La misión aplica la metodología de **construcción de clases**: el planeamiento delimita el contenido y orienta hacia la bibliografía; los estudiantes incorporan y leen las fuentes académicas necesarias, construyen la base de conocimientos y su vocabulario, y luego los términos, definiciones y relaciones se discuten y validan. Pueden incorporarse texto, gráficos y videos como apoyo, y cada estudiante puede integrar los vocablos trabajados en su síntesis personal.

El agente funciona como apoyo para identificar bibliografía, localizar lecturas y proponer términos con trazabilidad. No sustituye la lectura, discusión ni validación realizada por estudiantes y docentes.

## Criterios de aceptación

El protocolo cumple su misión cuando:

- identifica la clase del día a partir del planeamiento de cátedra;
- no propone el planeamiento como fuente bibliográfica;
- identifica la bibliografía asociada al contenido del día;
- presenta la referencia en APA 7 cuando sea posible sin inventar datos;
- verifica si la obra está disponible entre las fuentes;
- si falta la obra, pide al alumno que la agregue y detiene el proceso hasta recibir aviso;
- determina capítulos, secciones o apartados pertinentes solo después de disponer de la obra;
- extrae vocablos de la obra realmente consultada;
- muestra de dónde proviene cada término;
- explica por qué propone estudiarlo;
- ofrece al usuario una explicación o definición antes de desarrollarla;
- mantiene la trazabilidad entre planeamiento, bibliografía, lectura, vocablo y explicación.

## Restricciones

- No modificar `main.tex` sin autorización expresa y específica del usuario.
- No inventar contenido académico, citas ni referencias.
- No utilizar datos personales o reservados.
- No sustituir automáticamente una bibliografía ausente por otra fuente.
