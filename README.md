Linker

This is a C program to link and run an assembly language program written over multiple files. We will run the assembly language and executable files with the LCC program. 

Depending on which operating system you use, you may need to use a different version of the LCC program to run the assembler (written by my Professor Anthony Dos Reis). See his book: C and C++ Under the Hood.

To run, first enter the same repository as both the LCC, linker, and assembly language programs. Compile each assembly file with: 

./lccmac <filename>.a

This will create <filename>.o object files for each part of the program. If your computer is not allowing you to run the lcc program, you may have to update the program permissions with chmod 755 lccmac (or the name of the specific lcc program you are using). 

Then, you will need to compile the linker c program with: 

gcc -o <programname> link.c 

Then, link the object files: 

./<programname> <file1.o> <file2.o> <file3.o> and so on. 

This will create an exectable file link.e. 

Run the executable file with the lcc: 

./lccmac link.e 

(Note: program may ask for your name on the first run). 
