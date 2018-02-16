# Interpreter-using-lex-and-yaac
This is an implementation of a simple interpreter using lex and yaac for evaluating a given cfg
## Building the interpreter
yacc -y -d final_compile.y

lex final_compile.l

gcc -c y.tab.c lex.yy.c

gcc lex.yy.o y.tab.o final_compile.c -o compile
