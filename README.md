# LLM For Binary Analysis
### Introduction
**Feasibility**

**Challenges**

### Preliminary Study
| **Category**                    | **Analysis**                                          | **SOTA techniques**                                  | **Tool availability**                                                                                                     |
|---------------------------------|-------------------------------------------------------|-----------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| **Reverse Engineering**                    | decompile                                             | DnD                                                 | [DnD](https://github.com/purseclab/DnD)                                                                        |
|                                 | disassemble                                           | XDA, DeepDi                                         | [XDA](https://github.com/CUMLSec/XDA), [DeepDi](https://github.com/DeepBitsTechnology/DeepDi)                             |
|                                 | symbol name recovery                                  | SymLM, AsmDepictor                                  | [SymLM](https://github.com/OSUSecLab/SymLM), [AsmDepictor](https://github.com/agwaBom/AsmDepictor)                        |
|                                 | function detection                                    | Nucleus                                             | [Nucleus](https://www.vusec.net/projects/function-detection/)                                                             |
|                                 | type recovery                                         | StateFormer, OSPREY                                  | [StateFormer](https://github.com/CUMLSec/stateformer), [OSPREY](https://drive.google.com/file/d/1_AD2iWNaYflS1EtxPL-mSH-UNncU8YY0/view?usp=sharing) |
|                                 | lift to IR                                            | McSema (to LLVM IR)                                 | [McSema](https://github.com/lifting-bits/mcsema)                                                                          |
| **Fundamental Program Analysis**| call graph, control flow graph, program dependence graph | ghidra, Angr, IDA Pro, Radare2, Binary Ninja       | [Ghidra](https://ghidra-sre.org/), [Angr](https://github.com/angr/angr), [IDA Pro](https://hex-rays.com/ida-pro/), [Radare2](https://rada.re/), [Binary Ninja](https://binary.ninja) |
| **Advanced Analysis**           | similarity detection                                  | Trex                                                | [Trex](https://github.com/CUMLSec/trex), [Trex Plugin](https://github.com/peikexin9/trex_plugin)                          |
|                                 | pointer analysis / VSA                                | SVF (works on LLVM IR)                              | [SVF](https://svf-tools.github.io/SVF/)                                                                                    |
|                                 | binary rewriting                                      | RetroWrite MTSan                                    |                                                                                                                           |

