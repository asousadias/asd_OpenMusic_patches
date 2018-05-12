# The “fractalize” OpenMusic patch

Design and programming<br>
Antonio de SOUSA DIAS<br>
a.sousadias@belasartes.ulisboa.pt


## Description:
FRACTALIZE-N and FRACTALIZE-REC take two lists and generate a recursive pattern based upon the mapping of the first over the second list.

### FRACTALIZE-N
#### Inputs:
- List of MIDI Cent values
- List of MIDI Cent values
- Number of recursion levels to generate
#### Outputs:
- List of MIDI Cent values (pattern based upon the mapping of the first list over the second list)

### FRACTALIZE-REC
FRACTALIZE-REC is another recursive version of FRACTALIZE-N.
#### Inputs:
- a motif given as a MIDIcent list
- a MIDICent list of distances
- the number of recursion levels to generate.
#### Outputs:
- List of MIDI Cent values (pattern based upon the mapping of the first list over the second list)


## Remarks
The current folder consists of:<br>
- fractalize-n.omp - the main patch.
- fractalize-n-help.omp - a help patch containing an example and some operating mode instructions.
- fractalize-rec.omp - a variant of the main patch.
- fractalize_rec-help.omp - a help patch containing an example and some operating mode instructions.
- onset-dur.omp - subsidiary patch for regular onset/duration generation
- fractalize-n-help ALL.omp - same as _fractalize-n-help.omp_ but self-contained, i.e. it contains all the patches as abstractions.<br>

## History:
- 2018, May: Release on GitHub<br>
- 2008, May: OM version for release.<br>
- 2001: First OM version.<br>
- 1988: Initial design and programming in GFA Basic (Atari ST). Used in the documentary _Fernando Lanhas — Os Sete Rostos_ (António de Macedo, 1988). https://www.imdb.com/title/tt0492932<br>


### Disclaimer:
These patches are distributed in the hope that they will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.


Antonio de Sousa Dias<br>
Faculdade de Belas-Artes, Universidade de Lisboa<br>
Largo da Academia Nacional de Belas-Artes<br>
1249-058 Lisboa, Portugal<br>
http://www.belasartes.ulisboa.pt/

www.sousadias.com


