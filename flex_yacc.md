# Flex and Yacc compiler tools

Flex is an opensource tool used to generate a lexical analyzer. The tokens of a language are specified using regex and the flex syntax.

Yacc is also an opensource tool and used to generate a parser. It generates a bottom-up parser. Yacc accepts tokens from the lexer and parses them. The grammar of the language is specified using the YACC syntax which resembles the BNF grammar syntax

1. To generate tokens from a yacc file:
   `yacc -d yacc_file`

2. To generate the scanner from lex file
   `flex main.l`

3. To compile the scanner to a program
   `gcc -o a.out y.tab.c lex.yy.c -lfl -lm`
