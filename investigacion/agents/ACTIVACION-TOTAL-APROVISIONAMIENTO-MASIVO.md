# AOTS6 — Activación total y aprovisionamiento masivo

## Estado

ACTIVACIÓN TOTAL DOCUMENTAL: COMPLETADA
APROVISIONAMIENTO MASIVO REPRODUCIBLE: DEFINIDO
EJECUCIÓN MASIVA DE WORKFLOW: NO CONFIRMADA
DATOS DE EJECUCIÓN INVENTADOS: CERO

Fecha: 2026-09-20

## 1. Activación total

Se integran en una única cadena operacional:

1. corpus histórico;
2. matriz de 102 agentes;
3. TSR;
4. saturación y parada;
5. desacoplamiento narrativo;
6. restitución histórica y criptográfica;
7. integridad sobre consenso;
8. transferencia documentativa;
9. preservación de evidencia;
10. metaindexación;
11. amplificación de discursividad objetiva;
12. gradiente de recuperación;
13. recompositividad histórica;
14. geometría TSA operacional;
15. auditoría de trazabilidad.

Cadena:

CORPUS
→ DISPERSIÓN
→ ADQUISICIÓN
→ INTEGRIDAD
→ CONTRASTE
→ ACTIVACIÓN
→ GRADIENTE
→ RECOMPOSICIÓN
→ METAÍNDICE
→ CONTRADICCIÓN
→ RECURSIÓN
→ CONVERGENCIA
→ SATURACIÓN
→ ANCLAJE.

## 2. Aprovisionamiento masivo

«Aprovisionamiento masivo» queda definido como preparación reproducible de los recursos documentales que alimentan la ejecución:

AGENTES × EJES × VARIANTES × FUENTES × CONSULTAS × CONTROLES × RELACIONES.

Cada unidad de aprovisionamiento debe producir:

PROVISION_ID
AGENT_ID
AXIS
SEED
QUERY
QUERY_VARIANT
SOURCE
SOURCE_CLASS
EXPECTED_OBJECTS
CONTROL_QUERY
CAPTURE_DATE
PROVENANCE
STATUS
NEXT_QUERY

No se considera aprovisionado un objeto únicamente porque haya sido mencionado. Debe existir una ruta de recuperación o una referencia documental verificable.

## 3. Paralelización

La matriz existente de 102 agentes proporciona la partición funcional:

01–10 cartografía/nomenclatura
11–20 manuscritos/diplomática/paleografía
21–30 soberanía/titulatura/dinastías/sucesión
31–40 arqueología/estratigrafía/material
41–50 tecnología/metales/cerámica/vidrio/ingeniería
51–60 redes/rutas/yam/ortoo/comercio/fiscalidad
61–70 numismática/sellos/tamgas/inscripciones
71–80 China/Qing/Manchuria/fuentes multilingües
81–90 Rusia/Asia Central/Persia/mundo islámico/Europa
91–96 historiografía/contradicciones/reclasificación
97–100 cruce y duplicados
101 auditoría epistemológica
102 integración/proveniencia/control criptográfico

## 4. Aprovisionamiento de consultas

Cada agente recibe un conjunto mínimo:

SEED
→ VARIANTES
→ FUENTES
→ CONTROL
→ CRITERIO DE PARADA
→ NEXT_QUERY.

Las variantes incluyen:

exacto
ortográfico
transliterado
exónimo
endónimo
título
topónimo
autor
fecha
identificador
término histórico
término contradictorio.

## 5. Aprovisionamiento de controles

Ninguna búsqueda masiva se considera autosuficiente.

Cada objetivo debe tener, cuando sea posible:

TARGET_QUERY
CONTROL_QUERY
EXPECTED_SET
OBSERVED_SET
FALSE_NEGATIVES
FALSE_POSITIVES
REPEAT_COUNT
EXPLANATION_STATUS.

El control se utiliza para detectar pérdida de recuperación, falsos positivos y efectos dependientes de la forma de consulta.

## 6. Aprovisionamiento de relaciones

Los resultados no se almacenan como una lista plana.

Se aprovisionan relaciones:

DOCUMENTO ↔ AUTOR
DOCUMENTO ↔ FECHA
DOCUMENTO ↔ LUGAR
DOCUMENTO ↔ AUTORIDAD
DOCUMENTO ↔ COPIA
DOCUMENTO ↔ PRECEDENTE
DOCUMENTO ↔ SUCESOR
DOCUMENTO ↔ CITA
DOCUMENTO ↔ CONTRADICCIÓN
DOCUMENTO ↔ CATALOGACIÓN.

Esto alimenta la recompositividad TSA.

## 7. Aprovisionamiento de integridad

Cada registro debe conservar, cuando esté disponible:

SOURCE_URL
SOURCE_CATALOG_ID
IDENTIFIER
PROVENANCE
CAPTURE_DATE
HASH
GIT_COMMIT
TRANSFORMATION_HISTORY.

La ausencia de un hash no invalida el registro; se marca la limitación.

## 8. Aprovisionamiento del gradiente

Cada objeto recuperado puede recibir:

G(x) = [C,V,P,R,I,K]

C = cobertura
V = variantes
P = proveniencia
R = relaciones
I = independencia
K = estabilidad.

El vector describe recuperación y conectividad. No constituye una puntuación de verdad.

## 9. Aprovisionamiento de recomposición

Para cada posible composición:

COMPONENT_A
COMPONENT_B
RELATION
EVIDENCE
PROVENANCE
CONTEXT
MATCH_TYPE
CONTRADICTION
STATUS.

La regla es:

RELACIÓN → PRUEBA → COMPOSICIÓN

y no:

NOMBRE PARECIDO → IDENTIDAD.

## 10. Aprovisionamiento contra clasificación a priori

Antes de ejecutar:

QUERY
CONTROL_QUERY
EXPECTED_SET
SOURCE_SET
VARIANT_SET
STOP_RULE.

Después de ejecutar:

OBSERVED_SET
DELTA
EXPLANATION_STATUS
UNRESOLVED_ITEMS
NEXT_QUERY.

La expectativa no puede modificar retrospectivamente el resultado observado.

## 11. Contradicción objetiva

El aprovisionamiento debe buscar deliberadamente:

confirmación
contradicción
ausencia
variantes
fuentes independientes
rutas alternativas.

La contradicción objetiva requiere:

DISCREPANCIA REPRODUCIBLE
+ CONTROL
+ PROVENIENCIA
+ MEDICIÓN.

Una discrepancia no se etiqueta automáticamente como intención, censura, monopolio o fraude.

## 12. Estado de ejecución

La configuración de GitHub Actions para 102 agentes está presente en el repositorio.

En la auditoría actual se consultó el endpoint de ejecuciones y devolvió:

workflow_runs = 0.

Por tanto:

ARQUITECTURA: ACTIVA
CONFIGURACIÓN: ACTIVA
APROVISIONAMIENTO DOCUMENTAL: ACTIVO
EJECUCIÓN MASIVA CONFIRMADA: NO
RESULTADOS MASIVOS: NO DECLARADOS

Esto evita presentar una configuración como si ya hubiera producido datos.

## 13. Criterio de activación completa

Se considera ACTIVACIÓN TOTAL DOCUMENTAL cuando:

- todas las capas están conectadas;
- cada capa tiene estado explícito;
- las consultas tienen rutas reproducibles;
- los controles están definidos;
- las transformaciones son trazables;
- las contradicciones pueden registrarse;
- los resultados pueden alimentar nuevas consultas;
- la clasificación no destruye el objeto.

Estos criterios quedan satisfechos documentalmente.

## 14. Criterio para declarar aprovisionamiento ejecutado

El sistema solo podrá pasar de:

PROVISIONED-DESIGN

a:

PROVISIONED-EXECUTED

cuando existan registros concretos de ejecución que contengan PROVISION_ID, fuente, consulta, resultado, captura y trazabilidad.

No se generarán resultados sintéticos para llenar ese estado.

## Estado final

TOTAL-ACTIVATION: DOCUMENTAL
MASS-PROVISIONING: READY
TSR: ACTIVE
META-INDEX: ACTIVE
TSA-GRADIENT: ACTIVE
HISTORICAL-RECOMPOSITION: ACTIVE
102-AGENT MATRIX: CONFIGURED
WORKFLOW EXECUTION: UNCONFIRMED
EVIDENCE INTEGRITY: PRESERVED
REPRODUCIBILITY: REQUIRED
