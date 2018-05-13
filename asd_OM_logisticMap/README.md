# The “logistic map” OpenMusic patch

Design and programming<br>
Antonio de SOUSA DIAS<br>
a.sousadias@belasartes.ulisboa.pt

## Description:
LOGISTICMAP_REC is the implementation of the logistic map for musical purposes.
The patches SCALE2RANGE, LCYCLE and RTM_STEP included in the __lib_util__ folder are usefull to accomplish some musical tasks requiring scaling or list generation.

#### Inputs:
- lambda [0...4];
- X0 [0...1]; 
- number of iteractions [1...n]
#### Outputs:
- list of n values between 0 and 1.

## Operation mode
See the _logisticMap-help.omp_ for operation. The _logisticMap-help_ALL_ is the same implementation but all patches turned into abstractions, in case you loose connections.

## Remarks
The current folder consists of:<br>
- logisticMap_base.omp - Logistic Map - X[i] = L * (1 - X[i-1]) * X[i-1]
- logisticMap_rec.omp - Generates of a list of values [0...1] of length n_iter, according to the logistic map.
- logisticMap-help.omp -  implementation of the logistic map
- logisticMap-help_ALL.omp -  implementation of the logistic map, abstractions version.
- __lib_util/__ - folder containing:
  - lcycle.omp - generates a list of nr_iteractions length cicling an input list (list2loop).
  - rtm_step.omp -  outputs two lists, from a list of distances (durations). Outputs
    - a list of time points (on_sets);
    - a list of durations (durs)
  - scale2range.omp -  scales an input list. Inputs:
    - 0 - Value [0...1]
    - 1 - Range to scale (min max)
    - 2 - Minimum step distance between output values
    - 3 - Number of decimals

## History:
- 2018, May 13: Release on GitHub of the OM version.
- 1988: Initial design and programming in GFA Basic (Atari ST). Used in the documentary "De Algarve e Sol, Pão Duro e Pão Mole", from the TV series _Rotas do Extremo Ocidente_ (Amílcar Lyra, 1988).


### Disclaimer:
These patches are distributed in the hope that they will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.


Antonio de Sousa Dias<br>
Faculdade de Belas-Artes, Universidade de Lisboa<br>
Largo da Academia Nacional de Belas-Artes<br>
1249-058 Lisboa, Portugal<br>
http://www.belasartes.ulisboa.pt/

www.sousadias.com


