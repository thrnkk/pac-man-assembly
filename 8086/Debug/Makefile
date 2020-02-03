###############################################################################
# Makefile for project 
###############################################################################

## General options
PROJECT = 
MCU = 8086
COMPILER = "MASM32"
TARGET = Debug
SHELL = C:\WINDOWS\system32\cmd.exe

## Tools general options
ASMFLAGS=/c /Zd /Zi
LDFLAGS=/CODEVIEW

## Processing Tools
ASM=ml.exe
LD=link16.exe
#  C:/Users/User/Desktop/basico/8086/Debug/Debug.exe: TOOL=LD
#     C:/Users/User/Desktop/basico/8086/Debug/basico.obj: TOOL=ASM
#        C:/Users/User/Desktop/basico/8086/basico.asm

# Build tree:
all:	Debug

Debug:	Debug.exe

Debug.exe:	basico.obj 
	$(LD) $(LDFLAGS) basico.obj,Debug.exe,nul.map,,,

basico.obj:	../basico.asm 
	$(ASM) $(ASMFLAGS) ../basico.asm

# tidy - delete all temporary files which are not involved in the target generation
tidy:

# cleanup - delete all generated files
clean:	tidy
	rm -rf Debug.exe
	rm -rf basico.obj
