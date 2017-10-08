# LogoCompiler
Logo language compiler written in C. Use of Bison as a parser generator and flex as a lexical analyser generator. LOGO is an educational programming language.
The base of the language is to draw with simple instructions. FORWARD n (n being a number) draws a line - the size of the line is proportionnal to n. LEFT n makes the drawer rotate n degrees counter clockwise. RIGHT n makes the drawer rotate n degrees clockwise.

I implemented different options : 
- You can use different colors by two different ways : either writting the name of the color before the line you want to draw (for example : RED 50), either writting the RGB code of the color (for example : COLOR 0x65CFDB). To move the pencil without DRAWING, you can use TRANSPARENT
- You can draw different objects directly using their name followed by a number, which represents its size : SQUARE, STAR, CIRCLE
- You can define functions (or, more accurately, MACROS) using DEFINE FONCTION n [ ... ]; then use the n-th function with USE FUNCTION n.

There is an example of a LOGO program and its corresponding draw in the src folder.
