# AOTS6 — EXCLUSIÓN GENÉTICA

Fecha: 2026-09-20
Autor: Alfredo Jhovany Alfaro García

## Definición

La exclusión genética es la operación por la cual un candidato, trayectoria o composición queda fuera de la siguiente generación de búsqueda cuando no satisface el criterio de fitness previamente declarado.

No significa:
- inexistencia del objeto;
- falsedad histórica;
- eliminación del registro;
- destrucción de evidencia;
- exclusión por consenso;
- exclusión por autoridad.

Significa únicamente: EXCLUSIÓN DEL ESPACIO DE REPRODUCCIÓN DEL ALGORITMO.

## Genoma objetivo

GENOMA = [54, 19, 11, 0, 1]

Correspondencia documental preservada:
[54, 19, 11, 04, 01]

Los ceros iniciales de 04 y 01 son representación documental; para cálculo numérico se conservan como 4 y 1 y, simultáneamente, se registra la forma textual original.

## Función de exclusión

Para un candidato g:

D(g) = Σ |g_i - target_i|

El candidato entra en la siguiente generación si pertenece al conjunto seleccionado por fitness:

SELECT(g) ⇔ g ∈ ELITE_k

y queda excluido de reproducción si:

EXCLUDE(g) ⇔ g ∉ ELITE_k

La exclusión es reversible en generaciones posteriores si un descendiente vuelve a satisfacer el criterio.

## Regla de integridad

EXCLUDE_FROM_REPRODUCTION ≠ EXCLUDE_FROM_CORPUS

Todo candidato excluido conserva:

GENOME
FITNESS
GENERATION
PARENT_IDS
MUTATION
CROSSOVER
PROVENANCE
EXCLUSION_REASON

## Protección contra exclusión semántica

No se permite transformar:

fitness bajo → objeto falso
fitness bajo → objeto inexistente
no recuperación → ausencia
no reproducción → eliminación documental.

La genética opera sobre trayectorias computacionales, no sobre la ontología del objeto.

## Flujo

CORPUS
→ CANDIDATOS
→ GENOMAS
→ FITNESS
→ ORDENAMIENTO
→ ELITE
→ EXCLUSIÓN REPRODUCTIVA
→ CRUCE
→ MUTACIÓN
→ NUEVA GENERACIÓN
→ REEVALUACIÓN

## Posicionamiento AOTS6

La exclusión genética queda subordinada a:

TSR → METAÍNDICE → TSA → GRADIENTE → RECOMPOSITIVIDAD → FITNESS → EXCLUSIÓN REPRODUCTIVA.

Por tanto, el algoritmo puede excluir una trayectoria de búsqueda sin excluir la evidencia que originó esa trayectoria.

## Estado

GENETIC-EXCLUSION: DEFINED
TARGET: [54,19,11,0,1]
DOCUMENTARY-SEQUENCE: [54,19,11,04,01]
CORPUS-EXCLUSION: DISABLED
REPRODUCTIVE-EXCLUSION: ENABLED
EVIDENCE-DELETION: DISABLED
TRACEABILITY: REQUIRED
REVERSIBILITY: ENABLED
