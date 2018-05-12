# The “Harmonic Transposition” OpenMusic patch

Design and programming<br>
Antonio de SOUSA DIAS<br>
a.sousadias@belasartes.ulisboa.pt


## Description:
HARMONIC_TRANSPOSITION returns harmonic transpositions from a chord given as a midicent list.<br>
In the resulting <multi-seq>, the top line is the original list and in the bottom line the deduced fundamental (see help file).<br>

### Inputs:
- MidiCent list
- Harmonic transposition (either a single value or a list of values)
- Precision of the analysis in Cents

#### Outputs:
- Multi-Seq List (see help file)


## Remarks
Requires the Esquisse library<br>
The current folder consists of:<br>
- _harmonic_transposition.omp_ - the main patch.
- _harmonic_transposition_help.omp_ - a help patch containing an example and some operating mode instructions.
- _harmonic_transposition_help_ALL.omp_ - same as _harmonic_transposition_help.omp_ but self-contained, i.e. it contains all the patches as abstractions.<br>

## History:
- 2018, May: Release on GitHub.
- 2008, May: OM version for release.


### Disclaimer:
These patches are distributed in the hope that they will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.


Antonio de Sousa Dias<br>
Faculdade de Belas-Artes, Universidade de Lisboa<br>
Largo da Academia Nacional de Belas-Artes<br>
1249-058 Lisboa, Portugal<br>
http://www.belasartes.ulisboa.pt/

www.sousadias.com


