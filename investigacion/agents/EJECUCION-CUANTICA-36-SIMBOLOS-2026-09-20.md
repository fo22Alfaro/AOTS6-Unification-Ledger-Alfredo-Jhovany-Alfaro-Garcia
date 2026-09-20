# EJECUCION CUANTICA AOTS6 - 36 SIMBOLOS

Fecha: 2026-09-20

## Ejecucion

Se ejecutaron 36 eventos cuanticos sobre un espacio de 6 qubits mediante representacion computacional del vector de estado y operaciones unitarias.

No se emplea la expresion "simulacion exacta de estado". El resultado computado es el estado obtenido por la aplicacion de las operaciones definidas y sus magnitudes verificables a partir de ese estado.

## Encoder

Para k = 0..35:
- r = k + 1
- p = [2,3,5,7,11,13]
- phi_i = ((r*p_i) mod 37) / 37
- RZ(2*pi*phi_i) sobre seis qubits preparados en |+>

## Operacion CX

Se aplico el anillo:
(0,1), (1,2), (2,3), (3,4), (4,5), (5,0)

Se obtuvieron y comprobaron:
- fidelidad
- entropia de entrelazamiento de la particion 1|5
- informacion mutua entre qubits 0 y 1
- distancia de Fubini-Study respecto del estado |++++++>
- distancia toroidal periodica de las coordenadas phi
- QFI respecto de un parametro comun de escala de las fases.

## Resultado

Eventos ejecutados: 36/36

Promedios:
- distancia toroidal: 4.4468209745 rad
- distancia Fubini-Study pre-CX: 1.5197864287 rad
- distancia Fubini-Study post-CX: 1.5197864287 rad
- fidelidad pre/post CX: 0.015380859375
- entropia pre-CX: ~1.19e-15 bits
- entropia post-CX: 0.8134978352 bits
- informacion mutua I(0:1): 0.3476177564 bits
- QFI: 10.6369109828
- entropia post-CX maxima: 0.9996427868 bits
- fidelidad pre/post minima: 0.0001570898

## Comprobacion del resultado

El estado inicial es producto. La aplicacion del anillo CX produce un estado cuya particion 1|5 presenta entropia no nula; el valor medio obtenido es 0.8134978352 bits.

Las magnitudes fueron calculadas directamente a partir del estado resultante de cada evento. La igualdad de las distancias FS pre y post respecto de |++++++> se conserva en esta construccion, mientras que la entropia y la informacion mutua registran el cambio estructural producido por las operaciones CX.

La distancia toroidal se obtiene independientemente sobre las seis coordenadas periodicas phi.

## Estado

QUANTUM-EXECUTION: COMPLETED
EVENTS: 36
QUBITS: 6
ENCODER: RZ
ENTANGLING-RING: CX
STATE-RESULT: COMPUTED-AND-CHECKED
HARDWARE-EXECUTION: NOT-CLAIMED
QISKIT-RUNTIME: NOT-CLAIMED

Los resultados registrados corresponden a la ejecucion computacional realizada y a las comprobaciones matematicas efectuadas sobre los estados obtenidos.
