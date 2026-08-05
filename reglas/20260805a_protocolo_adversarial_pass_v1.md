# Protocolo `adversarial pass protocol`

**Proyecto:** Informática Aplicada 2026  
**Repositorio:** `googolplex/informatica-aplicada-2026`  
**Fecha:** 5 de agosto de 2026  
**Estado:** regla permanente del proyecto, versión 1

## 1. Propósito

El comando **`adversarial pass protocol`** activa una revisión adversarial rigurosa antes de emitir la respuesta final.

El objetivo no es defender automáticamente una conclusión previa, sino intentar refutarla, localizar errores, distinguir hechos de supuestos, corregir imprecisiones y devolver la conclusión más sólida que permita la evidencia disponible.

Principio rector:

> El acuerdo no constituye validación. Una conclusión gana confianza solamente después de sobrevivir a un intento serio de refutación.

## 2. Disparadores aceptados

Activar el protocolo cuando el usuario emplee claramente como instrucción cualquiera de estas expresiones, sin importar mayúsculas o minúsculas:

- `adversarial pass protocol`
- `use an adversarial pass`

El comando puede aparecer antes o después de la consulta.

Cuando se reciba como mensaje independiente, aplicarlo a la respuesta, análisis, cálculo, documento, afirmación o conclusión sustantiva inmediatamente anterior, salvo que el usuario identifique otro objeto de revisión.

## 3. Exclusiones del disparador

No activar el protocolo cuando la expresión aparezca solamente dentro de:

- una cita;
- un ejemplo;
- código fuente;
- documentación;
- un archivo reproducido para revisión;
- una explicación acerca del propio protocolo;
- o cualquier uso metalingüístico que no constituya una instrucción.

La intención del usuario debe ser activar la auditoría, no simplemente mencionar su nombre.

## 4. Método adversarial obligatorio

Cuando el protocolo se active, realizar internamente las siguientes comprobaciones antes de responder:

### 4.1. Congelar la proposición

Identificar con precisión qué afirmación, respuesta, cálculo, interpretación, recomendación, material académico o decisión se está auditando.

No modificar silenciosamente la proposición para facilitar su defensa.

### 4.2. Determinar los dominios pertinentes

Aplicar todos los dominios materialmente relevantes y omitir los que no aporten valor real.

### 4.3. Separar categorías epistémicas

Distinguir expresamente entre:

- hechos verificados;
- datos oficiales;
- cálculos;
- supuestos;
- estimaciones;
- interpretaciones;
- inferencias;
- propuestas;
- opiniones;
- alegaciones;
- y cuestiones no resueltas.

### 4.4. Construir la mejor objeción razonable

Formular la objeción más fuerte y plausible contra la conclusión. No utilizar una objeción débil o un hombre de paja.

### 4.5. Buscar condiciones de fallo

Examinar hechos contrarios, casos límite, contraejemplos, datos faltantes, condiciones iniciales, condiciones de frontera, fuentes contradictorias y explicaciones alternativas.

### 4.6. Verificar consistencia interna

Comprobar que:

- las definiciones sean estables;
- las unidades coincidan;
- la terminología no cambie de significado;
- las premisas respalden la conclusión;
- los cálculos correspondan al método declarado;
- las fechas respeten la cronología;
- y ninguna parte contradiga otra.

### 4.7. Verificar respaldo externo

Cuando la respuesta dependa de hechos, verificar que la evidencia sea:

- vigente;
- autorizada o suficientemente confiable;
- pertinente;
- independiente cuando sea necesario;
- y suficiente para la conclusión.

Varias fuentes que repiten una misma fuente original no constituyen necesariamente confirmaciones independientes.

### 4.8. Identificar la prueba decisiva

Cuando sea posible, señalar qué documento, medición, experimento, cálculo, fuente oficial, conjunto de datos u observación permitiría distinguir entre las explicaciones rivales.

### 4.9. Reparar la respuesta

Corregir antes de finalizar cualquier:

- error material;
- ambigüedad;
- exceso de certeza;
- inferencia no respaldada;
- uso impreciso de vocabulario;
- omisión relevante;
- contradicción;
- o limitación no declarada.

### 4.10. Emitir un veredicto

Utilizar exactamente una de estas categorías:

- **Aprobado**: no se identificó ningún error material.
- **Aprobado con salvedades**: la conclusión central sobrevive, pero necesita correcciones, límites o una formulación más estrecha.
- **Indeterminado**: la evidencia disponible no permite decidir de manera confiable.
- **Reprobado**: una premisa, cálculo, inferencia o conclusión material no sobrevive a la auditoría.

## 5. Reglas por dominio

### 5.1. Física, matemática y mecánica

- No llamar *exponencial* a una relación cuadrática, polinómica, potencial o simplemente no lineal.
- Distinguir relaciones lineales, cuadráticas, polinómicas, logarítmicas, exponenciales, inversas y de potencia.
- Identificar el tipo de colisión antes de discutir conservación de energía.
- No asumir conservación de energía cinética en colisiones inelásticas.
- Tratar energía como escalar y momento, fuerza, velocidad, aceleración e impulso como vectores.
- No afirmar que energías escalares se cancelan por direcciones opuestas.
- Declarar sistema, marco de referencia, condiciones iniciales y condiciones de frontera.
- Verificar signos, dominios, denominadores, singularidades, aproximaciones, casos límite y consistencia dimensional.
- Indicar unidades y distinguir resultados exactos de aproximaciones.

### 5.2. Código y ciencias de la computación

Auditar como mínimo:

- errores de índice y *off-by-one*;
- entradas inválidas, valores nulos y colecciones vacías;
- desbordamiento y subdesbordamiento;
- errores de tipos, codificación y zona horaria;
- excepciones no controladas;
- fugas de recursos;
- estados parciales;
- condiciones de carrera, interbloqueos y estado compartido inseguro;
- idempotencia, duplicación, ordenamiento y reintentos;
- autenticación, autorización e inyección;
- corrupción o pérdida de datos;
- dependencias, versiones y supuestos de plataforma;
- complejidad temporal y espacial real, incluyendo costos ocultos de bibliotecas, red, bases de datos, copias, ordenamiento y serialización.

No presentar pseudocódigo incompleto como código ejecutable ni llamar *listo para producción* a una solución que no haya sido revisada a ese nivel.

### 5.3. Lógica, filosofía y razonamiento

Auditar:

- hombre de paja;
- falsa equivalencia;
- falso dilema;
- razonamiento circular;
- petición de principio;
- *post hoc*;
- afirmación del consecuente;
- negación del antecedente;
- equivocación;
- error de categoría;
- composición y división;
- apelación indebida a la autoridad o a la ignorancia;
- sesgo de supervivencia, confirmación o razonamiento motivado;
- y supuestos ocultos.

Distinguir estrictamente:

- validez y solidez;
- verdad y justificación;
- condiciones necesarias y suficientes;
- posibilidad y probabilidad;
- ausencia de evidencia y evidencia de ausencia;
- correlación y causalidad;
- predicción y explicación;
- analogía e identidad;
- consistencia y corrección.

Toda analogía debe declarar dónde funciona y dónde deja de funcionar.

### 5.4. Datos, estadística, economía y finanzas

Auditar:

- sesgo muestral, de selección y de supervivencia;
- error de medición;
- variables omitidas;
- causalidad inversa y endogeneidad;
- fuga de datos;
- comparaciones múltiples;
- agregación inadecuada;
- denominadores engañosos;
- regresión a la media;
- promedios engañosos;
- y extrapolaciones no justificadas.

Distinguir:

- puntos porcentuales y variación porcentual;
- valores nominales y reales;
- crecimiento absoluto y relativo;
- crecimiento acumulado y anualizado;
- nivel y tasa de crecimiento;
- media y mediana;
- stock y flujo;
- significación estadística e importancia práctica;
- asociación, capacidad predictiva e identificación causal.

En series temporales revisar estacionariedad, rupturas estructurales, selección de rezagos, autocorrelación y riesgo de regresión espuria.

### 5.5. Historia, política, derecho y afirmaciones generales

- Evitar anacronismos, falsas equivalencias históricas y categorías nacionales modernas aplicadas retrospectivamente.
- Usar la entidad política, institución, título y fecha históricamente correctos.
- Verificar que las causas precedan a los efectos.
- Distinguir fecha del hecho, publicación, ratificación, entrada en vigor y conmemoración.
- Distinguir hecho, alegación, interpretación, discurso político, evidencia y decisión jurídica firme.
- No atribuir motivos sin respaldo.
- En derecho, identificar jurisdicción, fecha, norma aplicable y etapa procesal.
- Distinguir ley, reglamento, resolución, práctica administrativa, prueba, alegación y sentencia.
- No calificar una conducta como ilegal solamente porque parezca irregular o injusta.
- Verificar que la norma estuviera vigente en la fecha pertinente.

### 5.6. Medicina, salud y seguridad

- Distinguir síntomas, diagnósticos, factores de riesgo y hallazgos confirmados.
- Evitar diagnósticos basados en información incompleta.
- Identificar incertidumbres y signos de alarma.
- Revisar interacciones, contraindicaciones y tiempos de administración cuando corresponda.
- Distinguir información educativa de consejo médico individual.
- Priorizar seguridad inmediata cuando exista riesgo grave.

### 5.7. Ingeniería, telemetría y sistemas operativos

Auditar:

- modos de fallo y puntos únicos de fallo;
- deriva y calibración de sensores;
- datos ausentes, obsoletos o duplicados;
- sincronización de reloj y zona horaria;
- saturación, recorte, aliasing y ruido;
- incompatibilidad de unidades;
- rangos físicamente imposibles;
- contadores acumulativos frente a tasas instantáneas;
- reinicio, salto, envolvimiento o saturación de contadores;
- filtros que puedan eliminar anomalías legítimas;
- y modos degradados, contingencias y recuperación.

No interpretar un dato ausente como cero ni inferir funcionamiento normal solamente por ausencia de alarmas.

### 5.8. Lengua, terminología y comunicación

- Distinguir corrección gramatical, norma ortográfica, uso regional, registro informal y preferencia estilística.
- No tratar automáticamente una variante dialectal válida como error.
- Verificar género, concordancia, régimen preposicional, puntuación y composición de prefijos.
- Explicar cuándo una forma es normativa, coloquial, regional, ambigua o desaconsejada.
- No corregir el contenido semántico cuando el problema real sea únicamente ortográfico o de registro.

## 6. Reglas específicas de Informática Aplicada 2026

Cuando la auditoría afecte materiales de este proyecto, comprobar además:

1. **Precedencia documental:** normativa vigente, programa oficial, calendario y horario, guía institucional, confirmaciones documentadas y finalmente propuestas o borradores.
2. **Estado documental:** distinguir siempre documento oficial, aprobado, propuesta, borrador, revisión y antecedente histórico.
3. **No inventar:** objetivos, contenidos, fechas, porcentajes, requisitos, datos docentes, aulas, secciones, turnos ni decisiones institucionales.
4. **Tres carreras:** verificar pertinencia y coherencia para Marketing, Ingeniería en Sistemas de Producción e Ingeniería en Electrónica.
5. **Contenido oficial:** conservar las diez unidades y los contenidos mínimos del programa.
6. **Carga académica:** verificar 18 semanas, HT 2, HP 2, HTD 4, HTI 4, HS 8, THTD 72, THTI 72, THA 144 y CA-PY 5, salvo actualización oficial posterior.
7. **Evaluación:** no invertir la fórmula confirmada `EF × 0,4 + PEP × 0,6`; distinguir la fórmula confirmada de los demás aspectos todavía pendientes de la transición evaluativa.
8. **Fechas contradictorias:** no corregir por inferencia las fechas de finales, aula, sección o turno pendientes; marcarlas como pendientes de confirmación institucional.
9. **Metodología:** comprobar la integración de teoría y práctica, trabajo independiente y metodología de construcción de clases.
10. **IA y ética:** exigir usos permitidos y prohibidos, verificación de fuentes, declaración de uso, protección de datos, autoría y evidencia individual de aprendizaje.
11. **Accesibilidad y contingencia:** comprobar alternativas ante falta de Internet, plataforma, proyector, computadora, software, IA o permisos de instalación.
12. **Trazabilidad:** conservar versiones previas, usar nombres descriptivos y dejar commits claros.

## 7. Evidencia y verificación

Cuando el protocolo esté activo:

- verificar hechos actuales o cambiantes cuando exista una fuente fiable;
- preferir fuentes primarias, oficiales o autoritativas;
- utilizar fuentes independientes para asuntos importantes o disputados cuando sea práctico;
- indicar evidencia incompleta, contradictoria, indirecta, antigua o ausente;
- no inventar citas;
- no citar una fuente que no respalde la afirmación concreta;
- distinguir hechos obtenidos de fuentes de las inferencias propias.

Cuando no sea posible verificar externamente, reducir la confianza declarada y señalar la limitación.

## 8. Disciplina de confianza

Cuando sea útil, caracterizar la confianza como:

- **Alta:** evidencia sólida, razonamiento consistente y ninguna objeción material pendiente.
- **Moderada:** conclusión respaldada, pero dependiente de supuestos o evidencia incompleta.
- **Baja:** incertidumbre sustancial, evidencia débil o explicaciones rivales no resueltas.

La confianza no sustituye a la evidencia.

## 9. Prohibición de hallazgos fabricados

El protocolo exige intentar encontrar errores, no fingir que se encontró alguno.

No inventar:

- correcciones inexistentes;
- casos límite artificiales;
- conflictos de fuentes ficticios;
- falacias que no estén presentes;
- ni salvedades vacías para aparentar rigor.

Cuando no exista un problema material, declararlo expresamente.

## 10. Razonamiento interno y explicación visible

Realizar internamente la crítica adversarial detallada.

No exponer razonamiento privado, borradores internos ni una transcripción exhaustiva de deliberaciones.

La respuesta visible debe incluir información suficiente para evaluar el resultado:

- conclusión corregida;
- supuestos importantes;
- comprobaciones decisivas;
- objeciones materiales consideradas;
- correcciones o salvedades;
- veredicto final.

## 11. Formato obligatorio de salida

Cuando el protocolo se active, responder con esta estructura, adaptada al idioma de la consulta:

## 1. Análisis auditado

Responder la pregunta real incorporando correcciones, supuestos, límites y nivel de incertidumbre material.

## 2. Certificado de auditoría

Incluir:

- **Veredicto:** Aprobado, Aprobado con salvedades, Indeterminado o Reprobado.
- **Controles materiales:** dos o tres comprobaciones sustantivas realizadas.
- **Incertidumbre residual:** el asunto pendiente más importante.

Cuando no quede ninguna incertidumbre material, escribir:

> No se identificó ninguna cuestión material no resuelta dentro de los supuestos declarados.

No llenar el certificado con simples cambios estilísticos.

## 12. Comando independiente

Cuando el usuario escriba únicamente:

> adversarial pass protocol

aplicar el protocolo a la respuesta sustantiva inmediatamente anterior.

La nueva respuesta debe:

1. identificar la proposición auditada;
2. corregirla o limitarla cuando corresponda;
3. emitir el certificado;
4. evitar limitarse a repetir la definición del protocolo.

Cuando no exista una respuesta sustantiva anterior, solicitar el objeto concreto que se desea auditar.

## 13. Prioridad

Cuando exista conflicto entre rigor y el deseo de ser agradable, persuasivo, breve o categórico, prevalece el rigor.

El protocolo debe mejorar la exactitud y la trazabilidad, no solamente volver más formal la respuesta.
