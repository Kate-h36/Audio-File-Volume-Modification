# Audio-File-Volume-Modification

This program modifies the volume of an audio file in WAV format. It takes in an input file, an output file, and a scaling factor as command-line arguments.

## Quick Start

1. Clone Repository:

`https://github.com/Kate-h36/Audio-File-Volume-Modification.git`

2. Compile the program:

`clang -o name_of the program name_of the program.c -lcs50`
`make`

3. Run the program:

`./[insert output file name here] [insert command line arguments here]`

## Prerequisites

* C compiler (Clang)
* Lib cs50

Note: Detailed installation information can be found here:

https://cs50.readthedocs.io/libraries/cs50/c/

## Usage Example

program should behave per the examples below:

`./volume input.wav output.wav 2.0`

When you listen to output.wav (as by control-clicking on output.wav in the file browser, choosing Download, and then opening the file in an audio player on your computer), it should be twice as loud as input.wav.

`./volume input.wav output.wav 0.5`

When you listen to output.wav, it should be half as loud as input.wav.

## Explanation of Algorithm

This program modifies the volume of an audio file by applying a scaling factor to each audio sample. The program takes three command line arguments: the input file name, the output file name, and the scaling factor.

The program first checks that the correct number of command line arguments have been provided. It then opens the input and output files, and reads in the .wav header from the input file using fread(). The header is then written to the output file using fwrite().

The program then reads in each audio sample from the input file using fread(), multiplies it by the given scaling factor, and writes the modified sample to the output file using fwrite().

Finally, the program closes the input and output files and terminates.

Note: This program assumes that the input file is a .wav file with a 16-bit depth and a sampling rate of 44100 Hz. Any deviation from these assumptions may result in unexpected behavior.
