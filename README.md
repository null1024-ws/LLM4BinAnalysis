# LLM For Binary Analysis
### Introduction
**Feasibility**

**Challenges**

### Preliminary Study
| **Category**                    | **Analysis**                                          | **SOTA techniques**                                  | **Tool availability**                                                                                                     |
|---------------------------------|-------------------------------------------------------|-----------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| **Reverse Engineering**                    | decompile                                             | DnD                                                 | [DnD](https://github.com/purseclab/DnD)                                                                        |
|                                 | Disassemble                                           | XDA, DeepDi                                         | [XDA](https://github.com/CUMLSec/XDA), [DeepDi](https://github.com/DeepBitsTechnology/DeepDi)                             |
|                                 | Symbol name recovery                                  | SymLM, AsmDepictor                                  | [SymLM](https://github.com/OSUSecLab/SymLM), [AsmDepictor](https://github.com/agwaBom/AsmDepictor)                        |
|                                 | Function detection                                    | Nucleus                                             | [Nucleus](https://www.vusec.net/projects/function-detection/)                                                             |
|                                 | Type recovery                                         | StateFormer, OSPREY                                  | [StateFormer](https://github.com/CUMLSec/stateformer), [OSPREY](https://drive.google.com/file/d/1_AD2iWNaYflS1EtxPL-mSH-UNncU8YY0/view?usp=sharing) |
|                                 | Lift to IR                                            | McSema (to LLVM IR)                                 | [McSema](https://github.com/lifting-bits/mcsema)                                                                          |
| **Fundamental Program Analysis**| call graph, control flow graph, program dependence graph | ghidra, Angr, IDA Pro, Radare2, Binary Ninja       | [Ghidra](https://ghidra-sre.org/), [Angr](https://github.com/angr/angr), [IDA Pro](https://hex-rays.com/ida-pro/), [Radare2](https://rada.re/), [Binary Ninja](https://binary.ninja) |
| **Advanced Analysis**           | Similarity detection                                  | Trex                                                | [Trex](https://github.com/CUMLSec/trex), [Trex Plugin](https://github.com/peikexin9/trex_plugin)                          |
|                                 | Pointer analysis / VSA                                | SVF (works on LLVM IR)                              | [SVF](https://svf-tools.github.io/SVF/)                                                                                    |
|                                 | Binary rewriting                                      | RetroWrite MTSan                                    |                                                                                                                           |

