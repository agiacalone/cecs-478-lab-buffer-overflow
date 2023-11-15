# CECS 478 Lab: Buffer Overflow

## Assignment Description

This assignment focuses on buffer overflow attacks and how they can be carried out on poorly-programmed system programs. You may not be able to complete this assignment on a modern operating system, as modern compilers build canaries into code in order to prevent such a thing from occurring. I would recommend using an older Linux distribution in a virtual machine for this assignment (something prior to Linux kernel version 2.4), but you are welcome to attempt this on a modern OS and see if you can get it to work. Review the article [Smashing the Stack for Fun and Profit](http://phrack.org/issues/49/14.html) for a very good, detailed introduction on how to perform a stack smashing attack.

## Assignment

Given the following C code file, perform a stack smash on the [vuln.c](vuln.c) code file using a C program that you create named `exploit.c`. Your program should attempt to open up a reverse shell on the attacked program as root by exploiting the buffer (you can verify this by typing the command `whoami` on the resulting terminal). The [vuln.c](vuln.c) code must be compiled in its own, separate program and must not be altered from its original state.

Note: when running many versions of Linux, you may need to [disable some address randomization](http://gcc.gnu.org/wiki/Randomization).

## Deliverables

Submit your `exploit.c` to Github Classroom along with a writeup (written in Markdown) of how you attempted the stack smashing attack and screenshots of the output or result of a successful attack. If you are not able to succeed with the attack due to OS constraints, detail that in your writeup and explain how you would go about performing such an attack on this system (along with your C code).

### Please note:

* Your writeup *must* be done in Markdown format and must be included in the repository as a separate file. View the file `README.md` for an example of Markdown.
* Screenshots should be done in `*.jpg`, `*.png`, or `*.gif` formats, and be included individually as files in your repository (i.e. no ‘document’ with the images pasted inside). Screenshots which are too zoomed-in or otherwise unidentifiable will not be counted.

Your submission must follow the following rules, else *I will not grade it and you will receive a zero for the submission*:

* Do not use compression on your files.
* Make sure that all significant code is *commented* with your own explanations.
