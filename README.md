compilers-assignments
=====================

This is the repository for programming assignments for **Compilers** course from Coursera.

In each PA, there're the **key files** which are modified and the output file, which is the intermediate file generated by **Makefile**. Makefiles are modified to add some extra targets to facilitate debugging/testing.

Other files are just generated by existing Makefile templates (elaborated in the course link), so include files are not added here - they are linked during compiling time only.

Key files and outputs
======================

PA1
-------
- cool.flex 
- Generates **flex**

PA2
-------
- cool.y
- Generates **parser**

PA3
-------
- cool-tree.h
- semant.h
- semant.cc 
- Generates **semant**

PA4
-------
- cgen.h
- cgen.cc
- Generates **cgen**

A customized coolc compiler can be achieved by below pipeline:
``` shell
./flex $* | ./parser $* | ./semant $* | ./cgen $*
```

