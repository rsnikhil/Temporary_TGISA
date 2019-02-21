A table of the easily summarisable aspects of the RISC-V Formal ISA model comparison.  It should be read together with the filled-in markdown template descriptions for each model.  This table describes the current state of the models only, not work in progress and future plans. 

|                                                   | Forvis        | Grift       | Sail                    | Riscv-semantics     |           | 
| ------------------------------------------------- | ------------- | ----------- | ------------------------| ------------------- | --------- |
| Author/Group                                      | Bluespec      |Galois       |SRI/Cambridge            | MIT                 |           |   
| Licence                                           | MIT           |GPL3         |BSD                      | MIT                 |           |
| Metalanguage                                      | Haskell       |Haskell      |Sail                     | Haskell             |           |
| Functional coverage - Base ISA and extensions     | RV32/64IMAFDC |RV32/64GC    |RV64IMAC                 | RV32/64IMAF         |           |
| Functional coverage - Privilege levels            | MUS,Sv32,39,48|M            |MUS,Sv39                 | SV39                |           |
| Specification of assembly syntax and encoding     | no            |pp           |yes                      | no                  |           |
| Concurrency                                       | no            |no           |yes                      | no                  |           |
| Floating-point                                    | via Softfloat |via Softfloat|no                       | Softfloat           |           |
| Emulation                                         | 40min Linux   |via Haskell  |4min Linux               | ?                   |           |
| ...emulation speed                                | ??? IPS       |??? IPS      |300K on Intel i7-7700    | 100K on 6700HQ      |           |
| Use as test oracle in tandem verification         | yes           |no           |yes                      | yes                 |           |
| Theorem-prover definitions                        | via hs-to-coq?|no           |Coq,Isa,HOL4             | yes                 |           |
| Use in documentation                              | to LaTeX      |to text      |in RISC-V ISA            | no                  |           |
| Use in test generation                            | (at UPenn?)   |no           |yes                      | no                  |           |
| Use for concurrency-model litmus test evaluation  | no            |no           |yes                      | no                  |           |
| Test coverage - riscv-tests suite                 | ???           |???          |yes                      | yes                 |           |
| Test coverage - RISC-V compliance tests           | all           |almost all   |no (those are RV32)      | yes                 |           |
| Test coverage - OS boots                          | Linux,FreeRTOS|no           |Linux,FreeBSD,seL4       | Linux               |           |
| Test coverage - Concurrency litmus tests          | no            |no           |yes                      | no                  |           |

