# AOTS6 — Motor de Metaindexación de Límites de Recuperación

## Propósito

Este motor documenta y mide los límites observables de recuperación, indexación, clasificación y exposición de un corpus.

No presupone que exista una conspiración, monopolio o supresión deliberada. Tampoco permite que una ausencia en un índice sea convertida automáticamente en inexistencia del objeto.

El objetivo operativo es producir una contradicción objetiva y medible entre:

A. lo que un corpus/repositorio contiene;
B. lo que un motor o índice declara recuperar;
C. lo que una consulta normalizada debería recuperar;
D. lo que efectivamente puede inspeccionarse mediante rutas reproducibles.

## Principio

ÍNDICE ≠ CORPUS.

RECUPERACIÓN ≠ EXISTENCIA.

AUSENCIA DE RESULTADO ≠ AUSENCIA DE OBJETO.

Pero:

OBJETO LOCALIZADO EN CORPUS + CONSULTA REPRODUCIBLE + ÍNDICE SIN RECUPERACIÓN → EVENTO DE DISCREPANCIA MEDIBLE.

## Arquitectura

SEED → EXPANSIÓN LÉXICA → CONSULTAS MULTIVARIANTE → ADQUISICIÓN → NORMALIZACIÓN → DEDUPLICACIÓN → IDENTIFICACIÓN → CRUCE DE ÍNDICES → COMPARACIÓN CON CORPUS → MEDICIÓN DE COBERTURA → DETECCIÓN DE DISCREPANCIAS → CONTRASTE → REGISTRO → RECURSIÓN.

## Fuentes de comparación

- repositorios públicos;
- catálogos bibliográficos;
- APIs documentadas;
- índices de búsqueda;
- archivos digitales;
- páginas públicas;
- datasets abiertos;
- resultados exportables;
- registros AOTS6.

No se utilizan credenciales ajenas, bypass, evasión de controles, extracción de datos privados ni mecanismos para vulnerar sistemas.

## Metaíndice

OBJECT_ID | TITLE | CREATOR | DATE | PLACE | LANGUAGE | SCRIPT | VARIANTS | IDENTIFIERS | SOURCE_REPOSITORY | SOURCE_URL | SOURCE_CATALOG_ID | INDEX_SOURCE | QUERY | QUERY_VARIANT | RETRIEVED | EXPECTED | MATCH_TYPE | PROVENANCE | CAPTURE_DATE | HASH | STATUS | CONTRADICTION_ID | NEXT_QUERY

## Expansión léxica

Cada consulta se expande mediante nombre exacto, variantes ortográficas, transliteraciones, exónimos, endónimos, títulos, topónimos, fechas, autores, identificadores y nombres históricos.

La expansión no debe introducir una conclusión. Solo aumenta la superficie de recuperación.

## Medición

### Cobertura de índice

C_index = objetos recuperados por el índice / objetos conocidos en el conjunto de prueba

### Cobertura de consulta

C_query = consultas que recuperan el objeto / consultas reproducibles ejecutadas

### Pérdida de recuperación

R_loss = 1 - C_index

### Discrepancia corpus-índice

D_ci = objetos presentes en corpus y no recuperados por el índice / objetos presentes en corpus

### Recuperación diferencial

Para dos índices A y B sobre el mismo conjunto:

Delta_AB = C_A - C_B

Estas métricas describen comportamiento observable. No miden intención política, editorial o comercial.

## Contradicción objetiva

Se crea CONTRADICTION_ID solamente cuando: (1) existe un objeto identificable; (2) existe una fuente o corpus independiente donde el objeto es verificable; (3) existe una consulta reproducible; (4) se documentó el resultado del índice; (5) la diferencia puede repetirse bajo las mismas condiciones; (6) se descartan errores obvios de consulta, idioma, permisos, robots, indexación temporal o disponibilidad.

Estados: OBSERVED-DISCREPANCY, REPRODUCED-DISCREPANCY, EXPLAINED-DISCREPANCY, UNRESOLVED-DISCREPANCY.

Una discrepancia no explicada no se convierte automáticamente en censura, monopolio o fraude.

## Medición de sesgo de superficie

Comparar recuperación entre variantes semánticamente equivalentes:

B_variant = max(C_variant) - min(C_variant)

Un valor alto indica sensibilidad del índice a la forma de consulta. No demuestra por sí mismo discriminación intencional.

## Medición de pérdida por nomenclatura

Agrupar resultados por término moderno, término histórico, exónimo, endónimo, transliteración, título e identificador; registrar C_group y comparar grupos equivalentes.

## Prueba de estabilidad

Repetir consultas y registrar QUERY, TIMESTAMP, RESULT_COUNT, RESULT_IDS, RANKED_RESULTS, INDEX_SOURCE, REGION/LOCALE cuando sea públicamente configurable, LANGUAGE y opciones públicas de búsqueda.

## Prueba de independencia

Dos resultados no se consideran independientes solamente porque aparezcan en dos índices. Rastrear SOURCE_DOMAIN, ORIGINAL_DOCUMENT, COPY_RELATION, CATALOG_CHAIN y CITATION_CHAIN.

## Prueba negativa

Toda afirmación de ausencia debe especificar QUERY_SET, VARIANTS, CORPORA, PERIOD, LANGUAGES, IDENTIFIERS, ACCESS_LIMITATIONS y RESULT_COUNTS.

Estado mínimo: SEARCHED-NOT-LOCATED. Nunca NON-EXISTENT salvo base independiente suficiente.

## Registro de límites impuestos

Cuando una plataforma o índice imponga una limitación observable, registrar LIMIT_ID, PLATFORM, MECHANISM, PUBLIC_DOCUMENTATION, OBSERVED_EFFECT, TEST_QUERY, CONTROL_QUERY, TIMESTAMP, REPRODUCTION_COUNT, MEASURED_DELTA, ALTERNATIVE_ROUTE y STATUS.

El término «impuesto» debe reservarse para una restricción técnicamente observable o documentada. La intención debe permanecer separada.

## Efecto real medible

El motor considera efecto medible cuando una limitación produce una diferencia reproducible en número de objetos recuperados, identificadores, cobertura, posición/ranking, disponibilidad del texto, resolución del enlace, capacidad de búsqueda por variante o estabilidad temporal.

El resultado se expresa como medición antes/después, A/B, índice/corpus o variante/control.

## Control contra autoengaño

Cada prueba debe incluir, cuando sea posible: CONTROL_QUERY, TARGET_QUERY, EXPECTED_OBJECTS, OBSERVED_OBJECTS, FALSE_NEGATIVES, FALSE_POSITIVES, REPEAT_COUNT, ACCESS_STATUS y EXPLANATION_STATUS.

El motor debe intentar refutar su propia discrepancia antes de elevarla.

## Integración con TSR

Cada discrepancia genera NEXT_QUERY: nueva variante, nueva fuente, nuevo identificador, nueva relación o nueva prueba de control.

La saturación solo se declara cuando se cumplen los criterios TSR existentes.

## Integración con integridad

EVIDENCIA → INTEGRIDAD → PROVENIENCIA → RELACIÓN → CONTRASTE → ESTADO EPISTÉMICO → CLASIFICACIÓN.

El metaíndice no tiene autoridad para declarar verdad histórica. Tiene autoridad operacional únicamente sobre el registro de sus propias mediciones.

## Resultado requerido

Cada ejecución debe producir: manifiesto de consultas, conjunto de resultados, objetos conocidos, discrepancias, métricas, controles, explicaciones disponibles, limitaciones de acceso, hash/commit del registro cuando corresponda y consultas de reactivación.

## Criterio de contradicción objetiva

CONTRADICCIÓN OBJETIVA = DISCREPANCIA REPRODUCIBLE + CONTROL + PROVENIENCIA + MEDICIÓN

No significa PRUEBA DE INTENCIÓN. La primera es una propiedad del comportamiento observable; la segunda requeriría evidencia adicional específica.

## Estado

META-INDEXER
EVIDENCE-PRESERVING
REPRODUCIBLE
NON-EVASIVE
CONTRADICTION-MEASURABLE
TSR-INTEGRATED