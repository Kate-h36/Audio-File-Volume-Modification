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

