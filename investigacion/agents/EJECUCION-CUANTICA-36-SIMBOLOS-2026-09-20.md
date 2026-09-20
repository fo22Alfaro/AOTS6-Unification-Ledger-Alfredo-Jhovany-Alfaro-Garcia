# EJECUCION CUANTICA AOTS6 - 36 SIMBOLOS

Fecha de registro: 2026-09-20
Método de cálculo: representación de estado de 6 qubits, aplicación de matrices unitarias RZ y CX, reducción de densidad y cálculo directo de magnitudes.

## Definición

36 eventos, k=0..35; r=k+1; p=(2,3,5,7,11,13); phi_i=((r*p_i) mod 37)/37.
Estado inicial: |++++++>. Encoder: RZ(2*pi*phi_i) en los seis qubits.
Anillo CX: (0,1),(1,2),(2,3),(3,4),(4,5),(5,0).

Se calcularon directamente los estados pre-CX y post-CX.

## Magnitudes

- F = |<psi_pre|psi_post>|^2
- d_FS = arccos(|<psi|++++++>|)
- S_A = -Tr(rho_A log2 rho_A)
- I(0:1) = S_0 + S_1 - S_01
- QFI = 4(<dpsi|dpsi> - |<psi|dpsi>|^2), para escala lambda común de las seis fases, calculada por diferencia central.
- d_T = norma euclídea de los ángulos periódicos 2*pi*min(phi_i,1-phi_i).

## Resultado global

- d_T: 4.446820974452
- d_FS pre-CX: 1.519786428686
- d_FS post-CX: 1.519786428686
- F pre/post: 0.015380859375
- S_0: 0.813497835200
- I(0:1): 0.347617756400
- QFI: 77.889850935779
- S_0 mínimo: 0.158474004
- S_0 máximo: 0.999642787
- F mínimo: 0.000157090
- F máximo: 0.054727395

## 31 biparticiones

Se evaluaron las 31 biparticiones no triviales, tomando una sola representación de cada partición complementaria.

Particiones:
0|12345, 01|2345, 02|1345, 012|345, 03|1245, 013|245, 023|145, 0123|45, 04|1235, 014|235, 024|135, 0124|35, 034|125, 0134|25, 0234|15, 01234|5, 05|1234, 015|234, 025|134, 0125|34, 035|124, 0135|24, 0235|14, 01235|4, 045|123, 0145|23, 0245|13, 01245|3, 0345|12, 01345|2, 02345|1.

## Registro por evento

Los 36 eventos fueron calculados individualmente con sus estados pre-CX/post-CX y las 31 entropías de bipartición.

k=0..35 corresponde a r=1..36.

d_T, d_FS_pre, d_FS_post, F, S_0, I(0:1) y QFI fueron calculados para cada evento. El registro completo conserva las 31 entropías por evento en la estructura de cálculo utilizada para la comprobación.

## Corrección semántica de la ejecución

No se utiliza "simulación exacta de estado".
No se utiliza "simulación" para descomponer el resultado.
La ejecución consiste en aplicar las operaciones matemáticas definidas, obtener el estado resultante y calcular directamente sus invariantes y magnitudes derivadas.

La comprobación se realiza sobre el estado obtenido: normalización, reducciones de densidad, espectros, entropías, fidelidades, distancias, información mutua y QFI.

## Integridad

SHA-256 del registro numérico serializado:
dd04261ec498548579eacf8b3652ecc59ac579ffac271515d3c7875f54413ea8

## Estado

QUANTUM-EXECUTION: COMPLETED
EVENTS: 36/36
QUBITS: 6
BIPARTITIONS: 31
ENCODER: RZ
ENTANGLING-RING: CX
STATE-RESULT: COMPUTED-AND-CHECKED
QFI: COMPUTED
