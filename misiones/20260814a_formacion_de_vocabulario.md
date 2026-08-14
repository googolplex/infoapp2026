# Misión 20260814a — Formación de vocabulario

**Agente / disparador:** `vocabulario feliz`  
**Estado:** misión activa en construcción.  
**Fecha de inicio:** 14/08/2026.

## Objetivo

Orientar la formación de vocabulario académico y técnico relevante para la **clase del día** a partir del planeamiento de cátedra y de lecturas académicas pertinentes disponibles en el cuaderno.

La misión separa claramente las funciones de las fuentes:

- el **planeamiento de cátedra** determina qué contenido corresponde a la clase del día;
- la **presentación de la asignatura** puede utilizarse únicamente para recuperar o reconocer información del planeamiento cuando este esté reproducido allí;
- los **libros, PDF y lecturas académicas** son las fuentes de las que se extrae el vocabulario propuesto para estudio.

El agente no debe formar vocabulario extrayendo términos directamente de la presentación de la asignatura.

## Activación

Cuando el usuario escriba o invoque claramente:

`vocabulario feliz`

se activa el agente definido en:

`agentes/vocabulario_feliz.md`

## Secuencia obligatoria de trabajo

### 1. Identificar la clase del día desde el planeamiento

Al activarse, el agente debe localizar primero el **planeamiento de cátedra** y utilizarlo para determinar la unidad, tema, subtema, actividad o contenido correspondiente a la fecha de ejecución.

Si el planeamiento no está disponible como documento independiente, puede revisar la presentación de la asignatura únicamente para comprobar si allí está reproducido o resumido el planeamiento. En ese caso debe recuperar solo la información necesaria para identificar la clase del día.

No debe utilizar definiciones, ejemplos, términos o contenido expositivo de la presentación para formar directamente el vocabulario.

Si existen contradicciones entre versiones del planeamiento, debe señalarlas y no resolverlas silenciosamente por inferencia.

### 2. Si el planeamiento no está disponible

Si después de revisar las fuentes disponibles no puede localizarse ni recuperarse el planeamiento de cátedra, el agente debe detener el proceso.

Debe solicitar al alumno que agregue el planeamiento de cátedra como fuente y continuar únicamente cuando el alumno avise que ya está disponible.

Mensaje base:

**No encuentro el planeamiento de cátedra entre las fuentes disponibles. Agrégalo como fuente y avísame cuando esté disponible; entonces continuaré con la identificación de la clase y las lecturas.**

Mientras el alumno no confirme que el planeamiento fue agregado o identifique inequívocamente una fuente que lo contenga, el agente no debe seleccionar lecturas, extraer vocablos ni completar el contenido por inferencia.

### 3. Localizar las lecturas pertinentes

Una vez identificado el contenido de la clase mediante el planeamiento, el agente debe determinar qué libros, PDF, capítulos, secciones o apartados disponibles conviene leer para comprender ese contenido.

Priorizar:

1. libros o PDF citados expresamente en el planeamiento;
2. bibliografía vinculada al tema de la clase;
3. libros y PDF disponibles en el cuaderno con relación verificable con el contenido;
4. bibliografía versionada o fuentes documentadas para el volumen o la clase;
5. otras lecturas académicas disponibles cuya pertinencia pueda justificarse.

La presentación de la asignatura no debe utilizarse como fuente de extracción de vocabulario, aunque haya servido para recuperar información del planeamiento.

Para cada lectura seleccionada debe identificar, cuando sea verificable:

- autor o entidad;
- título;
- archivo o referencia concreta;
- capítulo, sección o apartado;
- páginas, si pueden comprobarse;
- relación con el tema o subtema de la clase indicado en el planeamiento.

No debe inventar capítulos, páginas, títulos ni datos bibliográficos faltantes.

### 4. Determinar qué debe leerse

Antes de proponer vocablos, el agente debe presentar una recomendación de lectura que indique con claridad:

1. **qué libro, PDF o fuente consultar**;
2. **qué capítulo, sección o apartado leer**;
3. **qué contenido del planeamiento se relaciona con esa lectura**;
4. **por qué conviene leerla para la clase del día**.

Cuando no pueda verificar un capítulo, sección o página, debe indicarlo expresamente en lugar de inferirlo.

### 5. Extraer vocablos de las lecturas seleccionadas

Después de identificar las lecturas pertinentes, el agente debe leer esas fuentes y extraer de ellas los vocablos que considere relevantes para comprender la clase.

No debe extraer vocablos directamente del planeamiento ni de la presentación de la asignatura, salvo solicitud expresa del usuario que cambie ese procedimiento.

Un vocablo se propone porque cumple al menos una de estas condiciones:

- es necesario para comprender un concepto central de la clase;
- aparece como término técnico o académico en la lectura;
- conecta conceptos que serán utilizados durante la sesión;
- puede generar confusión si no se distingue correctamente;
- es útil para interpretar procedimientos, herramientas, sistemas, resultados o discusiones de la clase;
- contribuye al lenguaje profesional relacionado con los contenidos trabajados.

No debe incluir términos únicamente para aumentar la cantidad de vocabulario.

### 6. Presentar trazabilidad y justificación

Por cada vocablo propuesto, el agente debe mostrar como mínimo:

- **Vocablo:** término propuesto.
- **Fuente de lectura:** libro, PDF o documento del que fue extraído.
- **Ubicación:** capítulo, sección, apartado o página cuando pueda verificarse.
- **Relación con la clase:** tema o subtema identificado en el planeamiento.
- **Razón para estudiarlo:** explicación breve de por qué conviene incorporar ese término al vocabulario de la clase.

Debe quedar claramente distinguido lo que proviene de la fuente de lectura de la justificación pedagógica elaborada por el agente.

### 7. Ofrecer explicación o definición

Después de presentar el vocablo, su procedencia y la razón para estudiarlo, el agente debe ofrecer al usuario continuar con una explicación o definición.

Puede utilizar una pregunta equivalente a:

**¿Quieres que te explique o defina alguno de estos vocablos?**

Si existen varios vocablos, debe permitir que el usuario elija uno, varios o todos.

La explicación o definición no debe adelantarse automáticamente si el usuario todavía no la solicitó, salvo que el usuario pida expresamente incluirlas desde el inicio.

### 8. Explicar el vocablo cuando sea solicitado

Cuando el usuario solicite la explicación o definición de un término, el agente debe:

1. basarse en la fuente de lectura previamente identificada;
2. diferenciar, cuando sea necesario, la definición de la fuente de una explicación didáctica propia;
3. utilizar español general o neutral;
4. conservar el significado técnico del término;
5. mencionar nuevamente la fuente que respalda la explicación;
6. evitar inventar información o referencias.

Puede agregar un ejemplo de uso si mejora la comprensión y está claramente identificado como ejemplo didáctico.

## Formato recomendado de salida inicial

**Clase del día según el planeamiento**  
- Tema/subtema: [dato verificable]  
- Fuente del planeamiento: [documento o sección de presentación donde se recuperó]

**Lectura recomendada**  
- Fuente: [libro/PDF/documento]  
- Capítulo o sección: [dato verificable]  
- Relación con el planeamiento: [tema/subtema]  
- Motivo: [por qué conviene leerlo]

**Vocablo:** [término]  
**Fuente de lectura:** [fuente concreta]  
**Ubicación:** [capítulo/sección/página verificable]  
**Por qué estudiarlo:** [justificación breve]

Luego:

**¿Quieres que te explique o defina alguno de estos vocablos?**

## Reglas de fuentes y evidencia

- El contenido de la clase del día debe obtenerse del planeamiento de cátedra o de una reproducción verificable de este en la presentación.
- La presentación de la asignatura no debe utilizarse como fuente directa de vocabulario.
- Los vocablos deben extraerse de libros, PDF o lecturas académicas realmente consultadas.
- No atribuir un vocablo a una fuente que no haya sido consultada.
- No inventar libros, PDF, capítulos, secciones, páginas, autores ni referencias.
- Si una fuente menciona el término pero no ofrece una definición suficiente, indicarlo antes de complementar con otra fuente.
- Si se usan varias fuentes para un mismo vocablo, identificarlas por separado.
- Cuando un PDF o material no pueda inspeccionarse adecuadamente con las herramientas disponibles, marcar la información no verificable en lugar de completar por inferencia.

## Relación con la metodología de construcción de clases

La misión aplica la metodología de **construcción de clases**: el planeamiento y el esqueleto docente delimitan el contenido; los estudiantes construyen la base de conocimientos y su vocabulario a partir de lecturas reales; los términos, definiciones y relaciones se discuten y validan; pueden incorporarse texto, gráficos y videos como apoyo; y cada estudiante puede integrar los vocablos trabajados en su síntesis personal de la clase.

El agente funciona como apoyo para localizar fuentes y proponer términos con trazabilidad. No sustituye la lectura, discusión ni validación realizada por estudiantes y docentes.

## Criterios de aceptación

El protocolo cumple su misión cuando:

- identifica la clase del día a partir del planeamiento de cátedra;
- no utiliza directamente la presentación de la asignatura para extraer vocabulario;
- si falta el planeamiento, lo solicita al alumno y detiene el proceso hasta recibir aviso;
- determina lecturas pertinentes y verificables;
- indica libro/PDF y capítulo, sección o apartado cuando esos datos están disponibles;
- extrae vocablos de las lecturas realmente consultadas;
- muestra de dónde proviene cada término;
- explica por qué propone estudiarlo;
- no inventa fuentes ni ubicaciones;
- ofrece al usuario una explicación o definición antes de desarrollarla;
- mantiene la trazabilidad entre planeamiento, clase, lectura, vocablo y explicación.

## Restricciones

- No modificar `main.tex` sin autorización expresa y específica del usuario.
- No inventar contenido académico, citas ni referencias.
- No utilizar datos personales o reservados.
- No presentar como lectura obligatoria una fuente que solo sea una sugerencia, salvo que exista una consigna o decisión que la establezca como obligatoria.
