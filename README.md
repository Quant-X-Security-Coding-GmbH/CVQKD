# CVQKD \(\epsilon\) Security
This document presents a strategy for an \(\epsilon\)-security proof of quantum key distribution. In a classical setting, an \(\epsilon\)-security proof derives the probability \(\epsilon\) of an attacker to succesfully guess chosen information from an encryption oracle. Several security models can be used for such a security proof. The transfer from a classical cryptographic \(\epsilon\)-security proof to a quantum setting is still ongoing research which is needed for establishing frameworks for quantum security device certification.

## What is QKD?
Quantum key distribution protocols are cryptographic key exchange protocols which leverage quantum mechanical principles. This distinguishes them from the cryptographic key exchange protocols (asymmetric cryptography) which are designed as mathematical algorithms.

## Security Level
The security level of a mathematical algorithm can be determined by computational means. The security of QKD protocols used to be called "unconditional", which led tomany misunderstandings and myths about the actual secuirty of a data transfer secured by QKD. In reality, there are other aspects in a QKD implementaion which determine it security level. They are of physical nature in the quantum component. Additionally, the data transport itself is usally encrypted with classical symmetric cryptographic algorithms such as AES-256 and OTP. In this case, the security level of the QKD-secured data transfer equals the computational security level of the used classical symmetric cryptographic algorithms.

## Key Management
Most aspects of QKD key management are handled in non-quantum components of an infrastructure. Therefore, the same key management threats apply as in a classical setting. Additional challenges might have to be considered due to the nature of symmetric keys in QKD key exchanges. In this strategy, we do not consider key management. We focus on the key exchange itself.

## License
This strategy is for public use under the conditions in the license of this repository. You are welcome to contact the contributers if you are interested in our professional support for a device specific proof or a collaboration in standardization and certification activities. 

## Contributers

* [Dr. Peter Nonnenmann](https://www.linkedin.com/in/peter-nonnenmann-737857a0/): Quantum theoretical aspects and choice of scientific sources
* [Xenia Bogomolec](https://www.linkedin.com/in/xenia-bogomolec-532981a6/): Cryptographic aspects, work package definition and roadmap for a resolution

## Strategy and Agile Roadmap
| Story                                              | Epic                              | Area of Expertise                    | Estimated time*          
|----------------------------------------------------|-----------------------------------|--------------------------------------|----------------
| Choose/define security model                       | Refine Analysis strategy          | Cryptography, Mathematics, Q-Theory  | 1-2 months
| Choose and prioritize input papers                 | Refine Analysis strategy          | Cryptography, Mathematics, Q-Theory  | 2-3 months
| Identify gaps from classical infosec perspective   | Refine Analysis strategy          | Cryptography, Mathematics, Q-Theory  | 2-3 months
| Plan integration of identified gaps                | Refine Analysis strategy          | Cryptography, Mathematics, Q-Theory  | 1-2 months
| Identify physical parameters                       | Refine Analysis strategy          | Engineering, Q-Theory                | 1-2 months
| SDP representation of trace norm                   | Math analysis of QKD protocol     | Mathematics, Q-Theory                | 2-3 months
| Asymptotic key rate calculation                    | Math analysis of QKD protocol     | Mathematics, Q-Theory                | 2-3 months
| Numerical finite key analysis (simply SVD)         | Math analysis of QKD protocol     | Mathematics, Q-Theory                | 2-3 months
| Lift collective attack to fully coherent attack    | Math analysis of QKD protocol     | Mathematics, Q-Theory                | 2-3 months
| Physical parameter estimation                      | Math analysis of QKD protocol     | Mathematics, Q-Theory, Engineering   | 2-3 months
| Public information and general sifting             | Math analysis of QKD protocol     | Mathematics, Q-Theory, Engineering   | 2-3 months
| Key map                                            | Math analysis of QKD protocol     | Mathematics, Q-Theory                | 2-3 months
| Vulnerabilitie/side channel attacks                | Math analysis of QKD protocol     | Mathematics, Q-Theory, Engineering   | 3-4 months
| Measure applicable security objectives             | Math analysis of QKD protocol     | Mathematics, Q-Theory                | 2-3 months
| Integrate Detector noise/error correction          | Detector noise/error correction   | Mathematics, Q-Theory, Engineering   | 3-4 months
| Identify gaps to classical literature              | Detector noise/error correction   | Mathematics, Q-Theory, Engineering   | 3-4 months
| Applicable playback attacks                        | Detector noise/error correction   | Mathematics, Q-Theory, Engineering   | 3-4 months
| Measure applicable security objectives             | Detector noise/error correction   | Mathematics, Q-Theory, Engineering   | 2-3 months
| Integration to adapted proof                       | Privacy amplification             | Cryptography, Mathematics, Q-Theory  | 2-3 months
| Comparison to classical hash functions             | Privacy amplification             | Cryptography, Mathematics, Q-Theory  | 2-3 months
| Options for computational representation           | Privacy amplification             | Cryptography, Mathematics, Q-Theory  | 2-3 months
| Vulnerabilitie/side channel attacks                | Privacy amplification             | Mathematics, Q-Theory, Engineering   | 2-3 months
| Measure applicable security objectives             | Privacy amplification             | Mathematics, Q-Theory, Engineering   | 2-3 months
| Vulnerabilitie/side channel attacks                | Privacy amplification             | Cryptography, Mathematics, Q-Theory  | 4-6 months
| Measure applicable security objectives             | Collective security evaluation    | Cryptography, Mathematics, Q-Theory  | 4-6 months

*in FTEs distributed to mentioned experts 

