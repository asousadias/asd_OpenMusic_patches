# The “glosa-figur” OpenMusic patch

Design and programming<br>
Antonio de SOUSA DIAS<br>
a.sousadias@belasartes.ulisboa.pt


## Description:
Given as inputs<br>
- a melodic sequence as a _Cantus Firmus_ (CF) and<br>
- a _melodic sequence_ (MS) as an ornamentation reservoir,<br>
this patch, for each two notes of the CF, finds all excerpts belonging to MS whose extreme notes form the same interval.<br>
The resulting data is prepared to be read by a score editor.

### Inputs:
- list of MIDIcents (or MIDI in the patch "glosa-figurMIDI"): the "Cantus Firmus".<br>
-  list of MIDIcents(or MIDI in the patch "glosa-figurMIDI"): the melodic sequence to be used as an ornamentation reservoir.<br>
- integer: Length of CF notes, for score viewing purposes (ms).<br>
- integer: Length of each generated note (ms).<br>
- integer: Number of staves/lines (channels).


### Outputs:
#### Leftmost output:<br>
- list of lists: output list of all values.<br>
#### Remaining output to be used with a __chord-seq__ object:<br>
- lmidic: list of MIDIcent<br>
- lonset: list of onset values (ms)<br>
- ldur: list of note durations (ms)<br>
- lchan: list of note MIDI channels<br>

## Remarks
The current folder contains:<br>
- glosa-figur.omp - the main patch.<br>
- glosa-figurMIDI.omp - a variant of the main patch (MIDI values as input).<br>
- glosa-figur-help.omp - a help patch containing an example and some operating mode instructions.<br>
- glosa-figur-help_ALL.omp - same as "glosa-figur-help.omp" but self-contained, i.e. it contains the patches "glosa-figur.omp" and "glosa-figur-help.omp" as abstractions.<br>

## References
For operating details see:<br>
Sousa Dias, A. (2008) Two examples of free transposition of audio processing techniques to the note domain in “Dói-me o luar” and Ressonâncias – Memórias. C. Agon, G. Assayag, J. Bresson (org.), _The OM Composer´s Book 2_, Paris, IRCAM / Delatour. ISBN: 2-84426-399-2. http://recherche.ircam.fr/equipes/repmus/OMBook/


## Revision history:
- 2018, May: Release on GitHub<br>
- 2009, Jan: Initial release on CICM site<br>
- 2001: Initial design and programming for use in _"Doi-me o luar"_(2001) under the name _Recursivus_<br>


### Disclaimer:
These patches are distributed in the hope that they will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.



Faculdade de Belas-Artes,<br>
Universidade de Lisboa<br>
Largo da Academia Nacional de Belas-Artes<br>
1249-058 Lisboa, Portugal<br>
http://www.belasartes.ulisboa.pt/

www.sousadias.com


