# x86 Assembly Cheat

[![Build Status](https://travis-ci.org/cirosantilli/x86-assembly-cheat.svg?branch=master)](https://travis-ci.org/cirosantilli/x86-assembly-cheat)

x86 userland minimal examples tutorial. Hundreds of runnable asserts. Containers (ELF), linking, calling conventions. System land cheat at: <https://github.com/cirosantilli/x86-bare-metal-examples>

1.  [Getting started](getting-started.md)
1.  Introduction
    1.  [How to learn](how-to-learn.md)
    1.  [Instruction sets](instruction-sets.md)
        1.  [Other architectures](other-architectures.md)
            1.  [ARM](https://github.com/cirosantilli/arm-assembly-cheat)
            1.  [RISC-V](risc-v.md)
            1.  [Microcontrollers](microcontrollers.md)
            1.  [Educational architectures](educational-architectures.md)
                1. [Y86](y86.md)
        1.  [RISC vs CISC](risc-vs-cisc.md)
            1.  [Microcode](microcode.md)
        1.  [System vs application programming](system-vs-application-programming.md)
        1.  [Flynn's Taxonomy](flynns-taxonomy.md)
    1.  [Assemblers](assemblers.md)
        1.  [gas/](gas/)
        1.  [nasm/](nasm/)
    1.  [Pros and cons of assembly](pros-and-cons-of-assembly.md)
    1.  [Intel processor history](intel-processor-history.md)
    1.  [Intel vs AT&T syntax](intel-vs-atet-syntax.md)
        1.  [intel2gas](intel2gas.md)
    1.  [Implementations](implementations.md)
    1.  [Extensions](extensions.md)
    1.  [CPU architecture](cpu-architecture.md)
        1.  [CPU Optimizations](cpu-optimizations.md)
        1.  [CPU bugs](cpu-bugs.md)
        1.  [Cache](cache.md)
        1.  [Instruction level parallelism](instruction-level-parallelism.md)
            1.  [Pipeline](pipeline.md)
            1.  [Branch prediction](branch-prediction.md)
            1.  [Superscalar](superscalar.md)
            1.  [VLIW](vliw.md)
            1.  [SIMT](simt.md)
        1.  [CPU benchmarks](cpu-benchmarks.md)
1.  [IA-32](ia-32.md)
    1.  [main.asm](main.asm)
    1.  [hello_world.asm](hello_world.asm)
    1.  Base concepts
        1.  [Registers](registers.asm)
            1. [Segment registers](segment_registers.asm)
        1.  [Addressing](addressing.asm)
        1.  [Endianess](endianess.asm)
    1.  Instructions
        1.  mov family
            1. [MOV](mov.asm)
            1. [MOVZX](movzx.asm)
            1. [MOVSX](movsx.asm)
            1. [CMOVcc](cmovcc.asm)
            1. [XCHG](xchg.asm)
            1. [LEA](lea.asm)
        1.  Flags
            1. [SETcc](setcc.asm)
        1.  Arithmetic
            1.  Addition
                1. [ADD](add.asm)
                1. [ADC](adc.asm)
                1. [INC](inc.asm)
            1.  Subtraction
                1. [SUB](sub.asm)
                1. [SBB](sbb.asm)
                1. [DEC](dec.asm)
            1.  Multiplication
                1. [MUL](mul.asm)
                1. [IMUL](imul.asm)
                1. [NEG](neg.asm)
            1.  Division
                1. [DIV](div.asm)
                1. [IDIV](idiv.asm)
            1.  [CDQ](cdq.asm)
            1.  Comparison
                1. [CMP](cmp.asm)
        1.  Bit-wise
            1.  Boolean
                1. [NOT](not.asm)
                1. [AND](and.asm)
                1. [OR](or.asm)
                1. [XOR](xor.asm)
                1. [TEST](test_instruction.asm)
            1.  Shifts
                1. [SHL, SHR](shl.asm)
                1. [SAL, SAR](sal.asm)
                1. [ROL, ROR](rol.asm)
            1.  Test
                [BT](bt.asm)
                [BTR](btr.asm)
                [BTC](btc.asm)
        1.  Branching
            1.  [Jcc](jcc.asm)
            1.  [JMP](jmp.asm)
                1. [JMP indirect](jmp_indirect.asm)
            1.  [LOOPcc](loopcc.asm)
        1.  [Stack instructions](stack-instrucastions.md)
            1. [enter](enter.asm)
            1. [leave](leave.asm)
            1. [pusha](pusha.asm)
            1. [pushf](pushf.asm)
        1.  [String instructions](string-instructions.md)
            1. [rep](rep.asm)
            1. [cmps](cmps.asm)
            1. [lods](lods.asm)
            1. [movs](movs.asm)
            1. [scas](scas.asm)
            1. [stos](stos.asm)
        1.  [Floating point](floating-point.md)
            1.  [FPU](fpu.asm)
            1.  [SIMD](simd.asm)
                1. [FMA](fma.md)
        1.  [Synchronization](synchronization.md)
            1. [XADD](xadd.asm)
            1. [CMPXCHG](cmpxchg.asm)
            1. [BTS](bts.asm)
            1. PAUSE TODO
        1.  Misc
            1. [RDRAND](rdrand.asm)
            1. [POPCNT](popcnt.asm)
            1. [RDTSC](rdtsc.asm)
            1. [NOP](nop.asm)
            1. [CPUID](cpuid.asm)
    1.  [Calling conventions](calling-conventions.md)
        1.  [cdecl](cdecl.md)
        1.  [cdecl examples](cdecl.asm)
        1.  [stdcall](stdcall.asm)
    1.  [Linux](linux/)
1.  [x86-64](x86-64/)
1.  [Containers](containers.md)
    1.  [ELF](elf.md)
        1. [ELF Hello World Tutorial](http://www.cirosantilli.com/elf-hello-world)
1.  Dynamic libraries
    1.  [ld-linux.so](ld-linux-so.md)
        1.  [ldd](ldd.md)
1.  [Compiler generated](compiler-generated/)
1.  [Binutils](binutils.md)
    1.  [ld](ld.md)
        1. [Linker scripts](linker-scripts/)
    1.  [readelf](readelf.md)
    1.  [objcopy](objcopy.md)
    1.  [objdump](objdump.md)
    1.  [size](size.md)
1.  [misc](misc.md)
1.  [Bibliography](bibliography.md)
1.  Related tutorials
    1. [x86 Instruction Encoding Tutorial](https://github.com/cirosantilli/x86-instruction-encoding-tutorial)
    1. [C++ Cheat](https://github.com/cirosantilli/cpp-cheat)
    1. [Linux Cheat](https://github.com/cirosantilli/linux-cheat)

WIP

1.  Binutils
    1. [ar](ar.md)
    1. [elfedit](elfedit.md)
    1. [nm](nm.md)
    1. [strip](strip.md)
1.  [DWARF](dwarf.md)
1.  [Symbol Versioning](symbol-versioning.md)
1.  [Debug registers](debug-registers.md)
