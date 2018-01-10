# Reverse-Engineering-using-GDB

I am following the tutorial.
Here, I am going to play with object file using GDB.
1. I am going to do Malware Analysis with 32 bit architecture.
2. ARM assembly 
3. ARM Reverse Engineering.

There are two basic techniques that can be used during malware analysis. The first one is static and second one is dynamic analysis.

Static analysis uses software tools to examine the exacutable w/o looking at the actual decompiled instructions in Assembly.

But here my focus is on Dynamic analysis, that uses disassemeblers and debuggers to analyze malware binaries. 

Tools: IDA which is multi-platform, multi-processor disassembler and debugger. 

Disassemebler: used to convert an executable binary written in Assembly, C, C++ etc into Assembly Language Instructions, that we can debug and manipulate.

x86 Assembly Language has two choices of syntax. The AT&T syntax was dominant in the unix world since the OS was developed at AT&T Bell Labs. The Intel syntax was originally used for the documentation of the x86 paltform and was dominant in the MS-DOS and Windows Environments.

This is essential whether I am going to examine a Windows binary in PE format or a Linux binary in ELF Format.


In Case of AT&T syntax, The source comes before the destination and in the intel syntax, destination comes before the source. 

Most of the Malware is written on 32 bit architecture to affect most of the systems.

Each new version of general purpose registers is created to be backward compatible with previous processors. This means that code utilizing 8-bit registers on the 8080 chips will still function on today's 64-bit chipset.

EAX: accumlator
EBX: Base register, pointer to data in the DS segment. used to store the base address of the program.
ECX: Counter Register, used for loop and string operations
EDX: used for i/o operations. 
ESI: Source index register. Pointer to data in the segment pointed to by the DS Register.
EDI:
EBP: Base Pointer. Pointer to data on the stack. It points to the bottom of the current stack frame. used to refernce local variable.
ESP: stack Pointer, points to the top of the current stack frame.




