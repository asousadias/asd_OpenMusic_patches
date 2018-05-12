# The _palimpsesto flt_ OpenMusic patch

Design and programming<br>
Antonio de SOUSA DIAS<br>
a.sousadias@belasartes.ulisboa.pt

## Description:
The “palimpsesto flt” is an OpenMusic patch, originally programmed in 2002, that transposes to the note domain the operations of filtering and morphing that we find in the audio domain.<br>
His operating mode is anchored on the idea of palimpsest, and its operation mode can be described as follows:  it takes two input MIDI files or "chord-seq" (a source file and a modulator file) and produces a third MIDI file according to one of two main operation modes (the Method parameter).<br>
The first mode, keeps only the notes from the source file that are equal to the notes of the modulation file, or, in a slight variant possibility, it keeps those notes having the same pitch class. It is thus a resulting hybridization between spectral multiplication and the use of comb filters.<br>
The second mode, “rounds” all notes from the source file to the nearest notes of the modulation file, or again, in a slight variant possibility, it rounds them to the near pitch class.<br>
The 2009 version is a revised one where a Time Adjust parameter has been added to adjust the length of the two input chord sequences.<br>

### Inputs:
- chord-seq 1. A chord-seq object used as source.
- chord-seq 2. A chord-seq object used as filter/modulator.<br>
- Time adjust (integer):<br>

	0-No change;
	1-Length of Inp-1 set to length of Inp-2;
	2 (or else) -Length of Inp-2 set to length of Inp-1.
	
- Method (integer):<br>

	0-Band pass note;
	1-Band pass pitch class;
	2-Round to nearest note;
	3-Round to nearest pitch class.
	
### Outputs:
- Chord sequence object data.

## Remarks
The current folder consists of:<br>
- palimpsesto-flt.omp - the main patch.<br>
- palimpsesto-flt-help.omp - a help patch containing an example and some operating mode instructions.<br>
- palimpsesto-flt-help_ALL.omp - same as "palimpsesto-flt-help.omp" but self-contained, i.e. it contains the patch "palimpsesto-flt.omp" as an abstraction.<br>

## References
For operating details see:<br>
Sousa Dias, A. “Two examples of free transposition of audio processing techniques to the note domain in “Dói-me o luar” and Ressonâncias – Memórias”. C. Agon, G. Assayag, J. Bresson (org.), The OM Composer´s Book. 2, Paris, IRCAM / Delatour, 2008.
ISBN: 2-84426-399-2.
http://recherche.ircam.fr/equipes/repmus/OMBook/


## Revision history:
- 2018, May: Release on GitHub<br>
- 2010, Jan 12: Minor correction to adjust select values on select object<br>
- 2009, Jan: Initial release on CICM site<br>
- 2002-2003: Initial design and programming for use in _Ressonâncias-Memórias_(2003)<br>

## Disclaimer:
These patches are distributed in the hope that they will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.<br>

Faculdade de Belas-Artes,<br>
Universidade de Lisboa<br>
Largo da Academia Nacional de Belas-Artes<br>
1249-058 Lisboa, Portugal<br>

www.sousadias.com


