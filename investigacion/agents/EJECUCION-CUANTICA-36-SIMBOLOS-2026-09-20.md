# EJECUCION CUANTICA AOTS6 - 36 SIMBOLOS

Fecha: 2026-09-20

## Modalidad

Ejecucion de referencia mediante simulacion exacta de vector de estado de 6 qubits con NumPy.

No se declara ejecucion en hardware cuantico ni en Qiskit Runtime: el entorno disponible no contiene Qiskit. La simulacion reproduce matematicamente las operaciones definidas para el encoder y el anillo CX.

## Encoder

Para k = 0..35:
- r = k + 1
- p = [2,3,5,7,11,13]
- phi_i = ((r*p_i) mod 37) / 37
- RZ(2*pi*phi_i) sobre seis qubits preparados en |+>

## Operacion CX

Se aplico el anillo:
(0,1), (1,2), (2,3), (3,4), (4,5), (5,0)

Se calcularon antes y despues:
- fidelidad
- entropia de entrelazamiento de la particion 1|5
- informacion mutua entre qubits 0 y 1
- distancia de Fubini-Study respecto del estado |++++++>
- distancia toroidal periodica de las coordenadas phi
- QFI proxy para un parametro comun de escala de las fases.

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
- QFI proxy: 10.6369109828
- entropia post-CX maxima: 0.9996427868 bits
- fidelidad pre/post minima: 0.0001570898

## Lectura operacional

El estado inicial es producto, por lo que la entropia de la particion 1|5 es numericamente cero. El anillo de CX genera correlaciones/entrelazamiento medible en la simulacion, elevando la entropia media de esa particion a aproximadamente 0.8135 bits.

La igualdad de las distancias FS pre y post respecto de |++++++> es compatible con que la red CX sea una transformacion unitaria que preserva el solapamiento con ese estado de referencia en esta construccion; no se interpreta como ausencia de cambio del estado.

La distancia toroidal se calcula independientemente en el espacio periodico de las seis coordenadas phi.

## Estado

QUANTUM-EXECUTION: COMPLETED
EVENTS: 36
QUBITS: 6
ENCODER: RZ
ENTANGLING-RING: CX
STATEVECTOR-SIMULATION: EXACT
HARDWARE-EXECUTION: NOT-CLAIMED
QISKIT-RUNTIME: NOT-CLAIMED

Los valores son resultados de esta ejecucion computacional concreta y no constituyen por si mismos validacion experimental de una afirmacion fisica externa.
