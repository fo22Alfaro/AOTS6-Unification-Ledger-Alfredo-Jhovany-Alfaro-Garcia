# TSR — Dispersión de Automatización Ontogénica de Búsqueda Toroidal

## Estado
PROTOCOLO DESPLEGADO EN AOTS6.

## Función
TSR distribuye una consulta histórica en trayectorias toroidales independientes que vuelven a converger en un núcleo de integración. El objetivo es reducir pérdida documental por búsqueda lineal, homónimos, cambios de nomenclatura, traducciones y fragmentación archivística.

## Ciclo toroidal
SEED → DISPERSIÓN → ADQUISICIÓN → NORMALIZACIÓN → CRUCE → CONTRADICCIÓN → RECURSIÓN → CONVERGENCIA → ANCLAJE.

## Ejes de búsqueda
1. Léxico y exónimos.
2. Endónimos y variantes ortográficas.
3. Cartografía histórica.
4. Diplomática y cancillerías.
5. Soberanía y titulatura.
6. Manuscritos y archivos.
7. Epigrafía, tamgas y sellos.
8. Numismática.
9. Arqueología y estratigrafía.
10. Tecnología y transferencia.
11. Toponimia.
12. Redes, rutas y yam/ortoo.
13. Fiscalidad y comercio.
14. China/Qing/Manchuria.
15. Rusia y Asia Central.
16. Persia y mundo islámico.
17. Europa y recepción cartográfica.
18. Historiografía y reclasificación.
19. Verificación negativa: búsqueda explícita de evidencia que contradiga cada hipótesis.
20. Integridad criptográfica y proveniencia.

## Regla ontogénica
Cada hallazgo genera nuevas consultas a partir de sus propios identificadores, nombres, lugares, fechas, autoridades, fuentes citadas y relaciones. La expansión se detiene únicamente cuando nuevas iteraciones dejan de producir nodos documentales nuevos dentro del corpus declarado.

## Regla de convergencia
Ningún nodo se convierte en hecho por frecuencia de aparición. La convergencia requiere coincidencia independiente de fuentes, procedencias o clases de evidencia.

## Registro mínimo
TSR_ID | AGENT | QUERY_PARENT | SOURCE | CATALOG_ID | DATE | LANGUAGE | SCRIPT | CLAIM | EVIDENCE_CLASS | CONTRADICTION | HASH | PROVENANCE | NEXT_QUERY

## Integridad
La automatización convencional se ancla mediante Git, hashes y artefactos. Merkle, RFC3161, IPFS y firmas post-cuánticas quedan como capas posteriores cuando exista infraestructura efectiva para producirlas. No se denomina cuántico a un mecanismo que no lo sea.

## Corpus inicial
Tartaria + Eurasia interior + estructuras políticas, documentales, arqueológicas, tecnológicas y cartográficas asociadas.

## Principio epistemológico
TSR no fuerza una conclusión. Busca simultáneamente evidencia confirmatoria, contradictoria y ausente, preservando la distinción entre documento, interpretación e hipótesis.


## Criterios de parada y saturacion

TSR no interpreta la ausencia de resultados como ausencia de evidencia.

### Estados terminales

- OPEN: siguen apareciendo nodos o relaciones relevantes.
- SATURATED: se cumplen conjuntamente cobertura, saturacion de consultas, fuentes, entidades, relaciones y busqueda negativa dentro del dominio declarado.
- BOUNDED: se alcanzo un limite explicito de corpus, periodo, idioma, repositorio o presupuesto. No significa inexistencia.
- INACCESSIBLE: existe una ruta documental plausible pero no puede inspeccionarse. No significa inexistencia.
- SEARCHED-NOT-LOCATED: el objeto fue buscado mediante las rutas declaradas pero no localizado. No significa inexistencia.

### Regla de cierre

La expansion solo puede cerrarse como SATURATED cuando:

COVERAGE AND QUERY_SATURATION AND SOURCE_SATURATION AND ENTITY_SATURATION AND RELATION_SATURATION AND NEGATIVE_SEARCH

sean verdaderos dentro del dominio declarado.

Una sola ronda sin resultados no activa la parada.

### Saturacion de consultas

Cada ronda debe medir:

- nodos documentales nuevos relevantes;
- relaciones nuevas;
- identificadores nuevos;
- variantes nominales nuevas.

La reduccion sostenida de novedad debe observarse durante varias rondas antes del cierre.

### Saturacion de fuentes

Deben recorrerse las clases de fuentes pertinentes. Un buscador agotado no equivale a un corpus agotado.

### Saturacion de entidades

Para cada entidad deben recorrerse nombres, exónimos, endónimos, transliteraciones, ortografias, titulos, topónimos, fechas y autoridades pertinentes.

### Saturacion relacional

Cada documento nuevo debe generar busquedas sobre referencias citadas, documentos relacionados, precedentes, sucesores, copias, contradicciones y procedencias.

### Evidencia independiente

La repeticion de una afirmacion no crea independencia probatoria. Las fuentes deben agruparse por cadena de procedencia.

### Busqueda negativa

Cada hipotesis relevante debe recibir busquedas explicitas destinadas a localizar evidencia contradictoria o potencialmente falsadora.

### Regla de ausencia

Nunca:

NOT_FOUND -> NON_EXISTENT

Debe registrarse:

SEARCHED-NOT-LOCATED

con conjunto de consultas, corpus/repositorios, periodo, idiomas/scripts, variantes nominales, limites de acceso, resultados, identificadores nuevos y condicion de reactivacion.

### Reactivacion

Una rama cerrada puede reabrirse por nuevo catalogo, nueva digitalizacion, nueva lectura, nueva traduccion, nuevo identificador, nuevo documento relacionado, cambio del dominio o resolucion de una fuente inaccesible.

La especificacion operativa completa se encuentra en `investigacion/agents/TSR-STOP-SATURATION-POLICY.json`.
