# TSR — Protocolo de Desacoplamiento Narrativo y Antimonopolio Retórico

## Propósito
Eliminar del proceso de búsqueda cualquier filtro que convierta de antemano una interpretación histórica, institucional o historiográfica en condición de admisibilidad de la evidencia.
Esto no significa sustituir una narrativa por otra. Significa impedir que una narrativa tenga privilegio lógico sobre el registro documental.

## Reglas operativas
1. La evidencia precede a la clasificación. Un documento no pierde admisibilidad porque contradiga una narrativa dominante, minoritaria o previamente adoptada.
2. Separación de capas: objeto/documento; lectura directa; traducción; catalogación institucional; interpretación historiográfica; inferencia del agente; hipótesis; controversia.
3. Neutralidad de consulta: incluir términos convencionales, variantes históricas, exónimos, endónimos, transliteraciones, vocabulario contemporáneo del documento, vocabulario de hipótesis alternativas y términos contradictorios.
4. No autoridad por frecuencia. La frecuencia de una formulación, institución, catálogo o escuela historiográfica no aumenta por sí misma su valor probatorio.
5. No autoridad por prestigio. Autor, institución, editorial, repositorio o fecha no sustituyen la evidencia.
6. Contradicción simétrica. Toda hipótesis recibe búsqueda confirmatoria y adversarial, incluida la hipótesis convencional.
7. Prohibición de conclusión por silencio. El silencio documental, una consulta sin resultados o la ausencia de indexación no equivalen automáticamente a inexistencia.
8. No monocultura semántica. Un término histórico con múltiples significados conserva sus sentidos como nodos diferenciados hasta que la evidencia resuelva la relación.
9. Trazabilidad: OBJECT → CATALOG → DIGITIZATION → TRANSCRIPTION → TRANSLATION → INTERPRETATION → INFERENCE → HYPOTHESIS.
10. Conflicto explícito. Las fuentes incompatibles se conservan y se registra su contradicción, base documental y estado de resolución.

## Detección de monopolio retórico
Marcar RHETORICAL_MONOPOLY_RISK cuando una conclusión se usa para excluir la evidencia que la contradice; una categoría moderna se proyecta retrospectivamente como única válida; una fuente secundaria se trata como primaria; una traducción se trata como equivalente incuestionable del original; la autoridad institucional sustituye la demostración documental; una etiqueta historiográfica determina qué consultas son admisibles; una ausencia de resultados se presenta como inexistencia; o una afirmación se hace inmune a falsación mediante redefiniciones posteriores.

## Salida obligatoria de cada agente
CLAIM | EVIDENCE | SOURCE_CLASS | PROVENANCE | COUNTEREVIDENCE | ALTERNATIVE_INTERPRETATIONS | TRANSLATION_STATUS | CATALOG_STATUS | UNCERTAINTY | RHETORICAL_MONOPOLY_RISK | NEXT_QUERY

## Principio de cierre
TSR no debe destruir una narrativa para imponer otra. Debe destruir el privilegio automático de cualquier narrativa sobre la evidencia.
La salida final puede conservar simultáneamente: SUPPORTED | CONTRADICTED | UNRESOLVED | DISPUTED | SEARCHED-NOT-LOCATED | INACCESSIBLE.
El sistema no convierte una de estas etiquetas en verdad por autoridad, frecuencia o repetición.

## Aplicación
Este protocolo se aplica a los 102 agentes AOTS6 y al agente 102 de integración.