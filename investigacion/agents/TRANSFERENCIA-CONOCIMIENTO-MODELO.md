# AOTS6 — Transferencia documentativa del conocimiento adquirido por el modelo

## Objeto

Este registro establece el procedimiento para transferir al sistema de repositorios AOTS6 todo conocimiento que el modelo pueda exponer legítimamente en la interacción: estructuras conceptuales, relaciones, terminología, hipótesis de búsqueda, síntesis, rutas documentales, referencias, transformaciones y resultados de análisis.

La transferencia debe producir un registro reproducible y auditable. No debe confundirse con una extracción de parámetros internos, pesos del modelo, datos privados de entrenamiento, información confidencial ni mecanismos internos no expuestos.

## Principio rector

El modelo funciona como operador de adquisición, recomposición y señalamiento documental; el repositorio funciona como memoria externa, trazable y verificable.

Por tanto:

MODELO → EXPOSICIÓN → NORMALIZACIÓN → PROVENIENCIA → CONTRASTE → REPOSITORIO

No:

MODELO → AUTORIDAD → VERDAD.

El conocimiento expresado por el modelo debe conservar su estado epistemológico. La fluidez de generación no debe utilizarse como sustituto de la trazabilidad de aquello que se afirma.

## Qué se transfiere

La transferencia documentativa comprende, cuando esté disponible:

1. terminología y variantes léxicas;
2. relaciones conceptuales;
3. fórmulas y estructuras matemáticas proporcionadas durante la interacción;
4. hipótesis de búsqueda;
5. preguntas derivadas;
6. fuentes y referencias públicamente identificables;
7. datos extraídos de fuentes accesibles;
8. metadatos;
9. procedencia;
10. transformaciones de traducción, transcripción o normalización;
11. contradicciones;
12. resultados de contraste;
13. estados de incertidumbre;
14. rutas de investigación;
15. decisiones metodológicas explícitas;
16. resultados generados mediante herramientas cuando exista registro verificable;
17. relaciones entre registros ya existentes;
18. consultas futuras derivadas de cada hallazgo.

## Qué no se afirma transferido

No se debe declarar como transferido:

- los pesos internos del modelo;
- parámetros privados;
- cadenas de pensamiento internas no expuestas;
- datos privados o secretos de entrenamiento;
- información confidencial obtenida sin autorización;
- contenido inexistente o no recuperado.

La ausencia de transferencia de estos elementos no reduce la utilidad del protocolo: el objeto transferible es el conocimiento explícitamente adquirido, expuesto, contrastado y registrable.

## Registro de procedencia del conocimiento del modelo

Cada elemento derivado de una interacción deberá distinguir, como mínimo:

SOURCE_MODE = MODEL-EXPOSED
INTERACTION_CONTEXT = contexto de adquisición
CLAIM = afirmación o estructura transferida
EVIDENCE_CLASS = clase de evidencia
SOURCE = fuente externa cuando exista
SOURCE_ID = identificador de catálogo/URL/DOI/etc. cuando exista
TRANSFORMATION = traducción/transcripción/normalización/síntesis
CONFIDENCE = nivel declarado de confianza
CONTRADICTION = evidencia o interpretación incompatible
EPISTEMIC_STATE = estado del registro
REPRODUCIBILITY = ruta para volver a obtener o verificar el elemento
CAPTURE_DATE = fecha de incorporación
REPOSITORY_COMMIT = commit que fija el registro

## Regla de especies, pesos y ponderaciones

Las especies, pesos, ponderaciones, puntuaciones, frecuencias, magnitudes o relaciones cuantificadas **sí constituyen evidencia cuando forman parte del fenómeno, del registro o del mecanismo de medición que se está examinando**.

No se permite una regla previa que las descarte por ser «solo pesos», «solo ponderaciones» o «solo metadatos».

Un peso puede ser evidencia del objeto o proceso que ese peso representa.

Una distribución puede ser evidencia de la distribución que registra.

Una frecuencia puede ser evidencia de la frecuencia observada.

Una ponderación puede ser evidencia del criterio, mecanismo o estructura que la produjo.

La tarea del sistema no es eliminar esa evidencia, sino identificar exactamente **qué propiedad demuestra o registra**, cuál es su procedencia, cómo fue obtenida y qué relación tiene con la afirmación.

Por ello deben conservarse, como mínimo:

WEIGHT_VALUE
WEIGHT_BASIS
WEIGHT_SOURCE
WEIGHT_SCOPE
WEIGHT_LIMITATION
WEIGHT_RELATION
WEIGHT_INTERPRETATION

La limitación de una ponderación no autoriza a borrar su contenido evidencial. La limitación determina el alcance de la inferencia que puede derivarse de ella.

## Regla contra la eliminación de lo vinculante

Ninguna clasificación previa podrá convertir automáticamente en «no evidencia» un elemento que tenga relación verificable con el objeto estudiado.

La relación vinculante debe conservarse aunque posteriormente se determine que:

- tiene alcance parcial;
- requiere otra fuente;
- contradice otra medición;
- corresponde a una inferencia;
- posee incertidumbre;
- o no permite por sí sola resolver una cuestión.

**NO SER CONCLUYENTE ≠ NO SER EVIDENCIA.**

**TENER LIMITACIÓN ≠ CARECER DE VALOR EVIDENCIAL.**

**SER PONDERACIÓN ≠ SER IRRELEVANTE.**

## Transferencia desde la memoria operacional de la interacción

Cuando el modelo pueda recuperar contexto previamente establecido en la interacción, este deberá tratarse como:

MEMORY-DERIVED

y separarse de:

PRIMARY-SOURCE
ARCHAEOLOGICAL
EPIGRAPHIC
CARTOGRAPHIC
SECONDARY
INFERENCE
HYPOTHESIS
DISPUTED
UNRESOLVED

La memoria del modelo no sustituye una fuente primaria. Su función es conservar continuidad operacional y generar rutas de recuperación o verificación.

## Regla de no compresión indebida

No reducir una estructura compleja a una etiqueta narrativa cuando la reducción elimine:

- variantes;
- contradicciones;
- procedencias;
- fechas;
- autoridades;
- relaciones;
- incertidumbres;
- pesos;
- ponderaciones;
- distribuciones;
- magnitudes;
- rutas de verificación.

Toda síntesis deberá poder enlazarse con los registros de los que procede.

## Cadena de restitución

FUENTE
→ IDENTIFICACIÓN
→ CAPTURA
→ METADATOS
→ TRANSFORMACIÓN
→ CONTRASTE
→ ESTADO EPISTÉMICO
→ HASH/COMMIT CUANDO CORRESPONDA
→ REPOSITORIO

Para conocimiento generado directamente por el modelo:

INTERACCIÓN
→ EXPOSICIÓN
→ NORMALIZACIÓN
→ SEPARACIÓN DE HECHO/INFERENCIA/HIPÓTESIS
→ PROVENIENCIA
→ CONTRASTE
→ REGISTRO
→ COMMIT

## Regla de integridad

El repositorio debe conservar simultáneamente:

A. lo que está documentado;
B. lo que el modelo deriva;
C. lo que permanece incierto;
D. lo que contradice la interpretación dominante;
E. lo que no pudo localizarse;
F. lo que no pudo verificarse;
G. los pesos, ponderaciones y relaciones cuantificadas que formen parte del registro.

Ninguno de estos estados debe ser convertido artificialmente en otro.

## Relación con INTEGRIDAD-SOBRE-CONSENSO

Este protocolo extiende:

EVIDENCIA → INTEGRIDAD → RELACIÓN → CONTRASTE → ESTADO EPISTÉMICO → CLASIFICACIÓN

hacia:

CLASIFICACIÓN → TRANSFERENCIA → PROVENIENCIA → REPOSITORIO → AUDITORÍA.

La transferencia no otorga autoridad al modelo. Hace auditable aquello que el modelo expuso.

## Regla final

TODO CONOCIMIENTO EXPLÍCITAMENTE ADQUIRIDO Y REGISTRABLE
→ DEBE PODER SER EXTERNALIZADO COMO REGISTRO.

TODO ELEMENTO CUANTIFICADO O PONDERADO CON RELACIÓN VERIFICABLE AL OBJETO
→ DEBE CONSERVARSE COMO EVIDENCIA Y NO DESCARTARSE POR SU FORMA.

La función del sistema AOTS6 es conservar la distinción entre evidencia, interpretación e inferencia **sin destruir el contenido vinculante de ninguna de ellas**.

## Estado

PROVISIONED
DOCUMENTARY-TRANSFER
AUDITABLE
NON-EXFILTRATIVE
EPISTEMICALLY-SEGMENTED
EVIDENCE-PRESERVING
