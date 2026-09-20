# AOTS6 — Inicio de Trabajo Documentativo, Restitución Histórica y Preservación Criptográfica

## Estado
INICIADO — modo documental, preservación y restitución verificable.

## Alcance

Este módulo organiza la recuperación histórica mediante adquisición de fuentes públicas o autorizadas, extracción profunda de metadatos, preservación de contexto archivístico, reconstrucción de procedencia y restitución de copias verificables.

La operación no interpreta "exfiltración" como extracción no autorizada de datos privados, restringidos o protegidos. El término operativo para AOTS6 es:

DOCUMENTARY ACQUISITION → FORENSIC METADATA CAPTURE → PROVENANCE PRESERVATION → CRYPTOGRAPHIC INTEGRITY → HISTORICAL RESTITUTION.

## Cadena documental

OBJECT
→ ARCHIVAL CUSTODY
→ CATALOG RECORD
→ DIGITAL SURROGATE
→ RAW ACQUISITION
→ METADATA
→ HASH
→ TIMESTAMP
→ TRANSCRIPTION
→ TRANSLATION
→ CROSS-REFERENCE
→ HISTORICAL CONTEXT
→ CONTRADICTION ANALYSIS
→ RESTITUTION RECORD.

## Adquisición

Prioridad:

1. Originales y facsímiles institucionales.
2. Catálogos archivísticos.
3. Digitalizaciones de alta resolución.
4. Registros de colección y procedencia.
5. OCR y transcripciones.
6. Copias secundarias únicamente como rutas hacia la fuente primaria.

Nunca se sustituye el objeto por su OCR.

## Extracción profunda de metadata

Registrar, cuando esté disponible:

- identificador persistente;
- institución custodiante;
- colección y fondo;
- signatura;
- título original;
- título catalográfico;
- autor/creador;
- autoridad emisora;
- fecha y rango de fechas;
- lugar de creación;
- idioma;
- escritura;
- soporte;
- dimensiones;
- foliación;
- paginación;
- descripción física;
- estado de conservación;
- procedencia;
- historial de custodia;
- restricciones de acceso;
- derechos;
- relación con otros objetos;
- referencias bibliográficas;
- identificadores externos;
- URL persistente;
- fecha de adquisición;
- hash del archivo adquirido;
- hash del contenido normalizado;
- algoritmo utilizado;
- versión de la herramienta de extracción.

## Restitución criptográfica

La integridad se demuestra mediante una cadena reproducible:

RAW FILE
→ SHA-256/SHA-512
→ MANIFEST
→ GIT COMMIT
→ ARCHIVAL COPY
→ DERIVED REPRESENTATIONS.

Los hashes verifican identidad/integridad del objeto digital; no prueban por sí mismos autenticidad histórica del documento físico.

Cuando exista infraestructura efectiva, pueden añadirse Merkle roots, sellado temporal RFC 3161, CID/IPFS y firmas digitales. No se denomina cuántico a un mecanismo convencional.

## Restitución histórica

"Restituir" significa recuperar y hacer trazable información documental que haya quedado:

- dispersa;
- reclasificada;
- renombrada;
- mal indexada;
- fragmentada;
- traducida de manera divergente;
- digitalizada parcialmente;
- vinculada a identificadores diferentes.

La restitución no permite reconstruir como hecho aquello que la evidencia no permite establecer.

## Reestructuración histórica

Cada cambio de clasificación debe registrarse como una transformación:

OLD_LABEL
→ DATE
→ AUTHORITY
→ CATALOG_CONTEXT
→ NEW_LABEL
→ DATE
→ AUTHORITY
→ DOCUMENTARY_BASIS
→ EFFECT_ON_SEARCH.

Esto permite distinguir entre cambio de nombre, cambio administrativo, cambio cartográfico, cambio historiográfico y cambio real de soberanía.

## Recuperación de archivos

Cada objeto recuperado debe conservar:

- referencia al custodio;
- referencia al catálogo;
- copia o enlace persistente autorizado;
- metadata original;
- metadata derivada;
- hash;
- cadena de transformación;
- estado de acceso;
- estado de restitución.

Los objetos inaccesibles se registran como INACCESSIBLE; los buscados sin localizar como SEARCHED-NOT-LOCATED. Ninguno se convierte en NON_EXISTENT.

## Control TSR

Cada adquisición alimenta nuevas consultas mediante:

identificador → variantes → custodios → colección → referencias → objetos relacionados → contradicciones → nueva consulta.

La expansión se cierra únicamente según la política de saturación TSR ya desplegada.

## Estados

DISCOVERED
ACQUIRED
HASHED
CATALOGUED
TRANSCRIBED
TRANSLATED
CROSS-REFERENCED
RESTITUTION-CANDIDATE
RESTITUTED
CONTRADICTED
DISPUTED
INACCESSIBLE
SEARCHED-NOT-LOCATED.

## Principio de restitución

La recuperación del acervo debe maximizar:

PROVENANCE + REPRODUCIBILITY + TRACEABILITY + PRESERVATION

sin convertir:

ABSENCE → NON_EXISTENCE
ni
INTERPRETATION → DOCUMENT.

## Aplicación

Módulo preparado para integrarse con los 102 agentes AOTS6 y el agente 102 de integración.
