# AOTS6 — Protocolo de restitución criptográfica e histórica de acervo

## Estado
INICIO DE TRABAJO DOCUMENTATIVO.

## Finalidad
Establecer una cadena verificable para localizar, identificar, recuperar, preservar y relacionar registros históricos y sus metadatos, sin convertir la recuperación en una reescritura narrativa de los hechos.

## Alcance
- documentos digitalizados y manuscritos;
- catálogos y registros archivísticos;
- mapas y atlas;
- códices, cartas, decretos y correspondencia;
- sellos, tamgas, nishan e inscripciones;
- registros numismáticos;
- fotografías, planos y expedientes;
- metadatos de procedencia, catalogación, digitalización y versiones.

## Regla de exfiltración documental
"Exfiltración" significa aquí extracción controlada de información desde fuentes legítimamente accesibles: datos, metadatos, identificadores, referencias cruzadas y trazas de procedencia. No implica intrusión, evasión de controles de acceso, extracción de credenciales ni acceso no autorizado.

## Cadena de restitución
FUENTE → IDENTIFICACIÓN → CAPTURA → HASH → METADATOS → TRANSCRIPCIÓN → TRADUCCIÓN → CONTEXTO → CRUCE → CONTRADICCIÓN → PROVENIENCIA → RESTITUCIÓN.

## Registro mínimo por objeto
OBJECT_ID | SOURCE_URL | REPOSITORY | CATALOG_ID | TITLE | CREATOR | DATE | PLACE | LANGUAGE | SCRIPT | MATERIAL | DOCUMENT_TYPE | AUTHORITY | RECIPIENT | SEAL/TAMGA | DESCRIPTION | METADATA | HASH | CAPTURE_DATE | PROVENANCE | ACCESS_STATUS | TRANSCRIPTION_STATUS | TRANSLATION_STATUS | CONTRADICTIONS | RELATED_OBJECTS | NEXT_QUERY

## Estados de acceso
- PUBLIC: acceso público legítimo.
- LICENSED: acceso mediante licencia/autorización.
- RESTRICTED: acceso restringido; no se intenta eludirlo.
- INACCESSIBLE: ruta identificada pero objeto no disponible.
- SEARCHED-NOT-LOCATED: buscado por rutas declaradas sin localización.
- RECOVERED: objeto o representación documental recuperada y verificable.

## Restitución criptográfica
La restitución criptográfica preserva identidad e integridad del objeto recuperado mediante:
1. hash del contenido capturado cuando sea técnicamente posible;
2. hash del archivo y, por separado, de transcripciones/metadatos derivados;
3. registro de fecha de captura;
4. URL/repositorio/catálogo de origen;
5. versión o identificador del objeto;
6. relación explícita entre original, copia, transformación y derivado;
7. Git como historial de cambios del corpus.

Las capas Merkle, RFC3161, IPFS o firmas post-cuánticas solo se declararán activas cuando exista evidencia de su generación efectiva.

## Restitución histórica
Restituir no significa declarar verdadera una reconstrucción. Significa devolver al registro analítico:
- el objeto;
- su contexto documental;
- su cadena de custodia/procedencia;
- sus variantes nominales;
- las interpretaciones existentes;
- las contradicciones;
- las zonas no localizadas o inaccesibles.

## Prohibiciones metodológicas
- NOT_FOUND ≠ NON_EXISTENT.
- repetición ≠ independencia probatoria.
- traducción ≠ original.
- catalogación moderna ≠ identidad histórica automática.
- etiqueta cartográfica ≠ soberanía demostrada por sí sola.
- ausencia de indexación ≠ ausencia del objeto.
- autoridad institucional ≠ sustituto de evidencia primaria.

## Módulos de adquisición
A. Archivos y bibliotecas.
B. Catálogos y colecciones digitales.
C. Cartografía histórica.
D. Manuscritos y diplomática.
E. Epigrafía, sellos y tamgas.
F. Numismática.
G. Arqueología.
H. Tecnología y transferencia.
I. Toponimia y lingüística histórica.
J. Historiografía y reclasificación.
K. Metadatos, versiones y proveniencia.
L. Integridad criptográfica.

## Salida de cada hallazgo
Cada hallazgo debe generar:
1. un registro normalizado;
2. su evidencia primaria o referencia verificable;
3. su cadena de procedencia;
4. sus transformaciones;
5. contradicciones y fuentes independientes;
6. consultas derivadas;
7. estado de acceso;
8. hash cuando exista un objeto digital recuperable.

## Principio de restitución
La recuperación del acervo debe maximizar trazabilidad y preservar incertidumbre. El objetivo no es fabricar una "verdad histórica" única, sino reconstruir el conjunto documental recuperable y hacer explícita la transición entre objeto, dato, metadato, interpretación e inferencia.

## Relación con TSR
TSR utiliza este protocolo como capa de adquisición y restitución. Cada nuevo identificador, referencia, topónimo, autoridad, sello, fecha o relación documental puede generar una nueva trayectoria de búsqueda.

Ciclo:
SEED → TSR → ADQUISICIÓN → RESTITUCIÓN → HASH → NORMALIZACIÓN → CRUCE → CONTRADICCIÓN → RECURSIÓN → CONVERGENCIA → ANCLAJE.

## Inicio
Este documento marca el inicio formal del corpus de restitución criptográfica e histórica de acervo de AOTS6.
