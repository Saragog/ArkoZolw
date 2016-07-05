English

Author: Andrzej Dackiewicz
Project written in Assembly ( Mips 32 processor ).
The goal of this project was to implement simple LOGO language (LOGO Komeniusz).
This language is very popular in Poland.
Many childreen make their first steps in programming with this language.
Logo komeniusz is a program used for learning basics of programming.
Turtle is used for drawing lines on bmp file. The lines are drawn with
Brensenham algorithm.

5 operations are possible:
- ustaw - setting position for turtle
- podnies - raise turtle so that it can't draw lines when moving
- opusc - reducing the turtle so that it can draw lines again
- naprzod - telling turtle to go forward ( if reduced it will draw a line )
- obrot - telling turtle to turn itself

Files used to make program work:
- pusty.bmp - file to which the result of work is saved. At the start the file
is cleaned.
- katy.txt - file that has the values of sine and cosine of degrees (0-89) used
for calculating the final position of turtle ( after operation naprzod ).
- turtle.txt - this file contains commands and arguments for turtle.
There is an example inside and result in bmp file.
- projektzolw.asm - source code of the program.


Most important labels of program:

- tworziwykonaj - analysis of read characters from file turtle.txt and
choosing operation. If incorrect set of characters - there is no such operation
is thrown. Works until there are operations in turtle.txt file.

- naprzod - Here Bresenham algorythm is used and appropriate dots are saved in
pusty.bmp file.

czytajliczbe - used for reading numbers from turtle.txt file that are
arguments of operations.
_________________________________________________________________________________

Polish

Autor: Andrzej Dackiewicz
Projekt zosta³ napisany w Asemblerze (Mips 32).
Celem projektu by³a implementacja prostego jezyka LOGO (LOGO Komeniusz).

Pelna dokumentacja projektu znajduje sie w pliku: "DokumentacjaZolw.pdf".