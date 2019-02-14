A table of the easily summarisable aspects of the RISC-V Formal ISA model comparison

|                                                   | Forvis        | Grift       | Sail                    |              |           |
| ------------------------------------------------- | ------------- | ----------- | ------------------------| ------------ | --------- |
| Author/Group                                      | Bluespec      |Galois       |SRI/Cambridge            |              |           |   
| Licence                                           | MIT           |GPL3         |BSD                      |              |           |
| Metalanguage                                      | Haskell       |Haskell      |Sail                     |              |           |
| Functional coverage - Base ISA and extensions     | RV32/64IMAFDC |RV32/64GC    |RV64IMAC                 |              |           |
| Functional coverage - Privilege levels            | MUS,Sv32,39,48|M            |MUS,Sv39                 |              |           |
| Specification of assembly syntax and encoding     | no            |pp           |yes                      |              |           |
| Concurrency                                       | no            |no           |yes                      |              |           |
| Floating-point                                    | via Softfloat |via Softfloat|no                       |              |           |
| Emulation                                         | 40min Linux   |via Haskell  |4min Linux               |              |           |
| Use as test oracle in tandem verification         | yes           |in progress  |yes                      |              |           |
| Theorem-prover definitions                        | via hs-to-coq?|no           |Coq,Isa,HOL4             |              |           |
| Use in documentation                              | to LaTeX      |to text      |in RISC-V ISA            |              |           |
| Use in test generation                            | (at UPenn?)   |no           |yes                      |              |           |
| Use for concurrency-model litmus test evaluation  | no            |no           |yes                      |              |           |
| Test coverage - RISC-V compliance tests           | all           |almost all   |no (those are RV32)      |              |           |
| Test coverage - OS boots                          | Linux,FreeRTOS|no (soon?)   |Linux,FreeBSD,seL4       |              |           |
| Test coverage - Concurrency litmus tests          | no            |no           |yes                      |              |           |
| Plans for future functional coverage              | no            |full priv arc|RV32,FD,Sv32/48,PMP/PMA,N|              |           |
