# EJECUCION GENETICA AOTS6 - 1000 AGENTES

Fecha: 2026-09-20
Repositorio: fo22Alfaro/AOTS6-Unification-Ledger-Alfredo-Jhovany-Alfaro-Garcia

## Ejecucion realizada

Se ejecuto localmente el motor genetico sobre 1000 agentes independientes.

Parametros:
- Agentes: 1000
- Generaciones por agente: 12
- Poblacion por generacion: 24
- Genoma: 5 valores enteros
- Objetivo: [54, 19, 11, 4, 1]
- Semilla reproducible por agente: 619000 + ID
- Seleccion: 4 elites
- Cruza: corte de 1 a 4 posiciones
- Mutacion: probabilidad 0.20, desplazamiento +-1, +-2 o +-3
- Rango de genes: 0..60

Funcion fitness:
fitness = -L1(genoma, objetivo) + 0.01 * cardinalidad_de_valores_distintos

La funcion se usa como funcion de optimizacion y registro computacional; no constituye una medida de verdad fisica o historica.

## Resultado

- Agentes ejecutados: 1000/1000
- Coincidencias exactas con [54,19,11,4,1]: 1/1000
- Mejor agente: 185
- Mejor genoma: [54,19,11,4,1]
- Mejor fitness: 0.05
- Fitness medio: -16.12597
- Distancia L1 media al objetivo: 16.175
- Tiempo de ejecucion: aproximadamente 0.636 s

## Mejores resultados

1. agente 185 -> [54,19,11,4,1] -> fitness 0.05 -> exacto
2. agente 51 -> [54,19,12,4,1] -> fitness -0.95
3. agente 80 -> [53,19,11,4,1] -> fitness -0.95
4. agente 128 -> [53,19,11,4,1] -> fitness -0.95
5. agente 175 -> [54,19,10,4,1] -> fitness -0.95
6. agente 188 -> [54,18,11,4,1] -> fitness -0.95
7. agente 252 -> [54,18,11,4,1] -> fitness -0.95
8. agente 305 -> [54,19,11,4,2] -> fitness -0.95
9. agente 322 -> [54,19,10,4,1] -> fitness -0.95
10. agente 430 -> [54,19,10,4,1] -> fitness -0.95

## Correspondencia con el modelo documental

El objetivo numerico [54,19,11,4,1] corresponde a la secuencia documental (54,19,11,04,01) localizada previamente en AOTS6_Model. La normalizacion numerica conserva 04 -> 4 y 01 -> 1.

## Estado

GENETIC-EXECUTION: COMPLETED
AGENTS: 1000
GENERATIONS: 12
EXACT-MATCH: 1
BEST-GENOME: [54,19,11,4,1]
REPRODUCIBLE: YES, mediante las semillas por agente y los parametros registrados
GITHUB-WORKFLOW-RUN: NO DECLARADO; esta ejecucion fue realizada directamente y no se atribuye a GitHub Actions.

## Integridad

Los resultados anteriores son la salida de esta ejecucion computacional concreta. No se han rellenado resultados faltantes ni se ha convertido el resultado genetico en una afirmacion externa sobre la realidad fisica del modelo.
