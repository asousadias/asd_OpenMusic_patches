# The “glosa-figur” OpenMusic patch

porgramming: Antonio de SOUSA DIAS


## DESCRIPTION:
Given a melodic sequence as a Cantus Firmus (CF) and a melodic sequence as an ornamentation reservoir (MS). For each two notes of the CF, this patch finds all excerpts belonging to MS whose extreme notes form the same interval.
The resulting data is prepared to be read by a score editor.

### Inputs:
-list of MIDIcents (or MIDI in the patch "glosa-figurMIDI"): the "Cantus Firmus"
-list of MIDIcents(or MIDI in the patch "glosa-figurMIDI"): the melodic sequence to be used as an ornamentation reservoir.
-integer: Length of CF notes, for score viewing purposes (ms)
-integer: Length of each generated note (ms)
-integer: Number of staves/lines (channels)

### Outputs:
Leftmost output:
-list of lists: output list of all values.

Remaining output to be used with a chord-seq:
-lmidic: list of MIDIcent
-lonset: list of onset values (ms)
-ldur: list of note durations (ms)
-lchan: list of note MIDI channels

# Remarks
The current folder consists of:
glosa-figur.omp - the main patch
glosa-figurMIDI.omp - a variant of the main patch (MIDI values as input)
glosa-figur-help.omp - a help patch containing an example and some operating mode instructions.
glosa-figur-help_ALL.omp - same as "glosa-figur-help.omp" but self-contained, i.e. it contains the patcehs "glosa-figur.omp" and "glosa-figur-help.omp" as abstractions.

# Operation
For operating details see:
Sousa Dias, A. “Two examples of free transposition of audio processing techniques to the note domain in “Dói-me o luar” and Ressonâncias – Memórias”
in
C. Agon, G. Assayag, J. Bresson (org.), The OM Composer´s Book. 2, Paris, IRCAM / Delatour, 2008.
ISBN: 2-84426-399-2.
http://recherche.ircam.fr/equipes/repmus/OMBook/


I hope it will be useful.

Antonio de Sousa Dias
Universidade de Lisboa, Faculdade de Belas-Artes
a.sousadias@belasartes.ulisboa.pt
2009-2018

# Revision history:




## Disclaimer:
These patches are distributed in the hope that they will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

Faculdade de Belas-Artes,
Universidade de Lisboa
Largo da Academia Nacional de Belas-Artes
1249-058 Lisboa, Portugal

www.sousadias.com


