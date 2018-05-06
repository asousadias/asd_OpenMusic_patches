# The “palimpsesto flt” OpenMusic patch

Antonio de SOUSA DIAS

www.sousadias.com


## DESCRIPTION:
The “palimpsesto flt” is an OpenMusic patch that transposes to the note domain the operations of filtering and morphing that we find in the audio domain.
His operating mode is anchored on the idea of palimpsest, and its operation mode can be described as follows:  it takes two input MIDI files or "chord-seq" (a source file and a modulator file) and produces a third MIDI file according to one of two main operation modes (the Method parameter).
The first mode, keeps only the notes from the source file that are equal to the notes of the modulation file, or, in a slight variant possibility, it keeps those notes having the same pitch class. It is thus a resulting hybridization between spectral multiplication and the use of comb filters.
The second mode, “rounds” all notes from the source file to the nearest notes of the modulation file, or again, in a slight variant possibility, it rounds them to the near pitch class.
The 2009 version is a revised one where a Time Adjust parameter has been added to adjust the length of the two input chord sequences.

### INPUTS:
-chord-seq 1. A chord-seq object used as source.
-chord-seq 2. A chord-seq object used as filter/modulator.
-Time adjust (integer)
	0-No change;
	1-Length of Inp-1 set to length of Inp-2;
	2 (or else) -Length of Inp-2 set to length of Inp-1.
-Method (integer)
	0-Band pass note;
	1-Band pass pitch class;
	2-Round to nearest note;
	3-Round to nearest pitch class.

### OUTPUT:
-Chord sequence object data.

# REMARKS
The current folder consists of:
- palimpsesto-flt.omp - the main patch
- palimpsesto-flt-help.omp - a help patch containing an example and some operating mode instructions.
- palimpsesto-flt-help_ALL.omp - same as "palimpsesto-flt-help.omp" but self-contained, i.e. it contains the patch "palimpsesto-flt.omp" as an abstraction.

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

12 Jan 2010: Minor correction to adjust select values on select object

## Disclaimer:
These patches are distributed in the hope that they will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

Faculdade de Belas-Artes,
Universidade de Lisboa
Largo da Academia Nacional de Belas-Artes
1249-058 Lisboa, Portugal

www.sousadias.com


