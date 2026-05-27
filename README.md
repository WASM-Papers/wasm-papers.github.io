# WasmSec — WebAssembly Security Papers

> A curated collection of academic papers covering the intersection of **WebAssembly and security** from memory safety and sandboxing to malware detection, formal verification, program analysis, dataset generation and side-channel attacks.

**Live site:** [wasm-papers.github.io](https://wasm-papers.github.io)

---

## About

WebAssembly (Wasm) is a production runtime powering some of the world's most critical applications - **Photoshop, Figma, AutoCAD, Google Earth, Cloudflare Workers, Zoom**, and many more. Its promise of near-native performance in a portable, sandboxed format has driven rapid adoption across browsers, edge computing, IoT, and serverless platforms.

Despite its sandboxing design, WebAssembly introduces a range of security concerns like memory corruption from C/C++ source, cryptojacking, malware obfuscation, Spectre-style side channels, runtime bugs, and the absence of default mitigations like stack canaries or ASLR.

This repository tracks academic research addressing these challenges. All papers have been **manually reviewed** and selected based on direct relevance to WebAssembly security.


---

## Papers

### Surveys & Empirical Studies

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [SoK: Analysis Techniques for WebAssembly](https://arxiv.org/abs/2401.05943) | Harnes, Morrison | arXiv | 2024 | [PDF](https://arxiv.org/abs/2401.05943) | — |
| [WebAssembly and Security: a review](https://arxiv.org/abs/2407.12297) | Perrone, Romano | arXiv | 2024 | [PDF](https://arxiv.org/abs/2407.12297) | — |
| [Avengers, Assemble! Survey of WebAssembly Security Solutions](https://ieeexplore.ieee.org/document/9860829) | Kim, Jang, Shin | IEEE CLOUD 2022 | 2022 | [PDF](https://ieeexplore.ieee.org/document/9860829) | — |
| [New Kid on the Web: A Study on the Prevalence of WebAssembly in the Wild](https://intellisec.de/pubs/2019a-dimva.pdf) | Musch, Wressnegger, Johns, Rieck | DIMVA 2019 | 2019 | [PDF](https://intellisec.de/pubs/2019a-dimva.pdf) | — |
| [An Empirical Study of Real-World WebAssembly Binaries](https://dl.acm.org/doi/epdf/10.1145/3442381.3450138) | Hilbig, Lehmann | WWW 2021 | 2021 | [PDF](https://dl.acm.org/doi/epdf/10.1145/3442381.3450138) | — |
| [Characterizing and Detecting WebAssembly Runtime Bugs](https://dl.acm.org/doi/10.1145/3624743) | Zhang et al. | ACM TOSEM | 2023 | [PDF](https://dl.acm.org/doi/10.1145/3624743) | — |
| [A Comprehensive Study of WebAssembly Runtime Bugs](https://ieeexplore.ieee.org/document/10123536) | Wang et al. | IEEE SANER 2023 | 2023 | [PDF](https://ieeexplore.ieee.org/document/10123536) | — |
| [An Empirical Study of Bugs in WebAssembly Compilers](https://dl.acm.org/doi/10.1109/ASE51524.2021.9678776) | Romano, Liu, Kwon, Wang | IEEE ASE 2021 | 2021 | [PDF](https://dl.acm.org/doi/10.1109/ASE51524.2021.9678776) | [Code](https://wasm-compiler-bugs.github.io/) |
| [Intel Software Guard Extensions Applications: A Survey](https://dl.acm.org/doi/10.1145/3593021) | Will, Maziero | ACM Computing Surveys | 2023 | — | — |
| [WebAssembly across Platforms: Running Native Apps in the Browser, Cloud, and Edge](https://doi.org/10.63282/3050-9246.IJETCSIT-V311P112) | Rusum | IJETCSIT | 2022 | — | — |
| [Wasmizer: Curating WebAssembly-driven Projects on GitHub](https://arxiv.org/abs/2303.09623) | Nicholson et al. | arXiv | 2023 | [PDF](https://arxiv.org/abs/2303.09623) | [Code](https://github.com/arash-mazidi/WASMIZER) |

---

### Memory Safety & Binary Security

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [Everything Old is New Again: Binary Security of WebAssembly](https://www.usenix.org/system/files/sec20-lehmann.pdf) | Lehmann, Kinder, Pradel | USENIX Security 2020 | 2020 | [PDF](https://www.usenix.org/system/files/sec20-lehmann.pdf) | [Code](https://github.com/sola-st/wasm-binary-security) |
| [MSWasm: Soundly Enforcing Memory-Safe Execution of Unsafe Code](https://arxiv.org/pdf/2208.13583) | Michael et al. | arXiv | 2026 | [PDF](https://arxiv.org/pdf/2208.13583) | — |
| [Iris-MSWasm: Elucidating and Mechanising the Security Invariants of Memory-Safe WebAssembly](https://dl.acm.org/doi/10.1145/3689722) | Legoupil et al. | OOPSLA 2024 | 2024 | [PDF](https://dl.acm.org/doi/10.1145/3689722) | [Code](https://github.com/logsem/MSWasm) |
| [Position Paper: Progressive Memory Safety for WebAssembly](https://dl.acm.org/doi/pdf/10.1145/3337167.3337171) | Disselkoen, Renner, Garfinkel, Levy | HASP 2019 | 2019 | [PDF](https://dl.acm.org/doi/pdf/10.1145/3337167.3337171) | — |
| [Memory Safety Preservation for WebAssembly](https://arxiv.org/abs/1910.09586) | Vassena | arXiv | 2019 | [PDF](https://arxiv.org/abs/1910.09586) | — |
| [Security Risks of Porting C Programs to WebAssembly](https://arxiv.org/pdf/2112.11745) | Stiévenart, De Roover, Ghafari | arXiv | 2021 | [PDF](https://arxiv.org/pdf/2112.11745) | — |
| [The Security Risk of Lacking Compiler Protection in WebAssembly](https://arxiv.org/pdf/2111.01421) | Stiévenart, Ghafari, De Roover | arXiv | 2021 | [PDF](https://arxiv.org/pdf/2111.01421) | — |
| [Bringing Binary Exploitation at Port 80: Understanding C Vulnerabilities in WebAssembly](https://www.scitepress.org/publishedPapers/2024/128524/pdf/index.html) | Massidda et al. | SECRYPT 2024 | 2024 | [PDF](https://www.scitepress.org/publishedPapers/2024/128524/pdf/index.html) | — |
| [An Analysis of Modern Web Security Vulnerabilities Inside WebAssembly Applications](https://arxiv.org/pdf/2603.09426) | Corrias et al. | arXiv | 2026 | [PDF](https://arxiv.org/pdf/2603.09426) | [Code](https://anonymous.4open.science/r/wasm-pocs/) |
| [WASP: Stack protection for WebAssembly](https://www.sciencedirect.com/science/article/pii/S1383762125003388) | Massey, Olivier | Journal of Systems Architecture | 2026 | [PDF](https://www.sciencedirect.com/science/article/pii/S1383762125003388) | [Code](https://github.com/ermassey/wasp) |
| [Defending Buffer Overflows in WebAssembly: A Transpiler Approach](https://arxiv.org/pdf/2604.03859) | Feng | arXiv | 2026 | [PDF](https://arxiv.org/pdf/2604.03859) | — |
| [RichWasm: Safe, Fine-Grained, Shared-Memory Interoperability in WebAssembly](https://arxiv.org/abs/2401.08287) | Paraskevopoulou et al. | arXiv | 2024 | [PDF](https://arxiv.org/abs/2401.08287) | [Code](https://github.com/RichWasm/RichWasm-artifact) |
| [Indexed Types for a Statically Safe WebAssembly](https://dl.acm.org/doi/10.1145/3632922) | Geller, Frank, Bowman | POPL 2024 | 2024 | [PDF](https://dl.acm.org/doi/10.1145/3632922) | — |
| [WALMA: Learning to See Memory Corruption in WebAssembly](https://arxiv.org/pdf/2603.24167) | Draissi, Sadeghi | arXiv | 2026 | [PDF](https://arxiv.org/pdf/2603.24167) | — |
| [Wemby's Web: Hunting for Memory Corruption in WebAssembly](https://dl.acm.org/doi/10.1145/3728937) | Draissi et al. | ISSTA 2025 | 2025 | [PDF](https://dl.acm.org/doi/10.1145/3728937) | [Code](https://github.com/uni-due-syssec/wemby) |

---

### Sandboxing & Isolation

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [Provably-Safe Multilingual Software Sandboxing using WebAssembly](https://www.usenix.org/conference/usenixsecurity22/presentation/bosamiya) | Bosamiya, Lim, Parno | USENIX Security 2022 | 2022 | [PDF](https://www.usenix.org/conference/usenixsecurity22/presentation/bosamiya) | [Code](https://github.com/secure-foundations/provably-safe-sandboxing-wasm-usenix22) |
| [WaVe: a verifiably secure WebAssembly sandboxing runtime](https://ieeexplore.ieee.org/document/10179357) | Johnson et al. | IEEE S&P 2023 | 2023 | [PDF](https://ieeexplore.ieee.org/document/10179357) | [Code](https://wave.programming.systems/) |
| [SFI safety for native-compiled Wasm (VeriWasm)](https://www.ndss-symposium.org/wp-content/uploads/ndss2021_5B-3_24078_paper.pdf) | Johnson et al. | NDSS 2021 | 2021 | [PDF](https://www.ndss-symposium.org/wp-content/uploads/ndss2021_5B-3_24078_paper.pdf) | [Code](https://veriwasm.programming.systems) |
| [Gobi: WebAssembly as a Practical Path to Library Sandboxing](https://arxiv.org/abs/1912.02285) | Narayan et al. | arXiv | 2019 | [PDF](https://arxiv.org/abs/1912.02285) | — |
| [Put Your Memory in Order: Efficient Domain-based Memory Isolation for WASM](https://dl.acm.org/doi/10.1145/3576915.3623205) | Lei et al. | ACM CCS 2023 | 2023 | [PDF](https://dl.acm.org/doi/10.1145/3576915.3623205) | [Code](https://github.com/PKU-ASAL/PKUWA) |
| [Going beyond the Limits of SFI: Hardware-Assisted In-Process Isolation with HFI](https://research.google/pubs/going-beyond-the-limits-of-sfi-flexible-and-secure-hardware-assisted-in-process-isolation-with-hfi/) | Narayan et al. | ASPLOS 2023 | 2023 | [PDF](https://research.google/pubs/going-beyond-the-limits-of-sfi-flexible-and-secure-hardware-assisted-in-process-isolation-with-hfi/) | [Code](https://github.com/PLSysSec/hfi-root) |
| [Donky: Domain Keys — Efficient In-Process Isolation for RISC-V and x86](https://www.usenix.org/conference/usenixsecurity20/presentation/schrammel) | Schrammel et al. | USENIX Security 2020 | 2020 | [PDF](https://www.usenix.org/conference/usenixsecurity20/presentation/schrammel) | [Code](https://github.com/IAIK/Donky) |
| [WASHADOW: Protecting WebAssembly Memory Through VM-Aware Shadow Memory](https://ieeexplore.ieee.org/document/10945011) | Jiang, Hua | IEEE TrustCom 2024 | 2024 | [PDF](https://ieeexplore.ieee.org/document/10945011) | — |
| [WASMSEPA: Effectively Protecting WebAssembly Through Privilege Separation](https://ieeexplore.ieee.org/abstract/document/11173483) | Jiang, Hua | IEEE QRS 2025 | 2025 | [PDF](https://ieeexplore.ieee.org/abstract/document/11173483) | — |
| [VMCANARY: Effective Memory Protection for WebAssembly via VM-assisted Approach](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10366728) | Zhang et al. | IEEE QRS 2023 | 2023 | [PDF](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10366728) | — |
| [metaSafer: A Technique to Detect Heap Metadata Corruption in WebAssembly](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10296897) | Song, Park, Kwon | IEEE Access | 2023 | [PDF](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10296897) | — |
| [CAGE: Hardware-Accelerated Safe WebAssembly](https://arxiv.org/abs/2408.11456) | Fink et al. | arXiv | 2024 | [PDF](https://arxiv.org/abs/2408.11456) | [Code](https://github.com/TUM-DSE/cage-meta) |
| [POSTER: Leveraging eBPF to enhance sandboxing of WebAssembly runtimes](https://dl.acm.org/doi/10.1145/3579856.3592831) | Abbadini et al. | EuroSys 2023 | 2023 | [PDF](https://dl.acm.org/doi/10.1145/3579856.3592831) | — |
| [WARD: Efficient Memory Protection for WebAssembly on Tiny Embedded Systems](https://doi.org/10.1109/ACCESS.2025.3650447) | Shin et al. | IEEE Access | 2026 | — | — |
| [eWASM: Practical Software Fault Isolation for Reliable Embedded Devices](https://ieeexplore.ieee.org/document/9211422) | Peach et al. | IEEE TCAD | 2020 | [PDF](https://ieeexplore.ieee.org/document/9211422) | [Code](https://github.com/gwsystems/awsm/) |

---

### Formal Verification & Type Systems

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [Mechanising and Verifying the WebAssembly Specification](https://dl.acm.org/doi/10.1145/3167082) | Watt | CPP 2018 | 2018 | [PDF](https://dl.acm.org/doi/10.1145/3167082) | [Code](https://github.com/WasmCert/WasmCert-Isabelle) |
| [CT-Wasm: Type-Driven Secure Cryptography for the Web Ecosystem](https://dl.acm.org/doi/10.1145/3290390) | Watt et al. | PACMPL | 2019 | [PDF](https://dl.acm.org/doi/10.1145/3290390) | — |
| [A Self-certifying Compilation Framework for WebAssembly](https://dl.acm.org/doi/abs/10.1007/978-3-030-67067-2_7) | Namjoshi, Xue | VMCAI 2021 | 2021 | [PDF](https://dl.acm.org/doi/abs/10.1007/978-3-030-67067-2_7) | [Code](https://github.com/nokia/web-assembly-self-certifying-compilation-framework) |
| [Automatically Eliminating Speculative Leaks from Cryptographic Code with Blade](https://dl.acm.org/doi/10.1145/3434330) | Vassena et al. | POPL 2021 | 2021 | [PDF](https://dl.acm.org/doi/10.1145/3434330) | [Code](https://github.com/PLSysSec/blade) |
| [Indexed Types for a Statically Safe WebAssembly](https://dl.acm.org/doi/10.1145/3632922) | Geller, Frank, Bowman | POPL 2024 | 2024 | [PDF](https://dl.acm.org/doi/10.1145/3632922) | — |
| [SecWasm: Information Flow Control for WebAssembly](https://dl.acm.org/doi/10.1007/978-3-031-22308-2_5) | Bastys et al. | ESORICS 2022 | 2022 | [PDF](https://dl.acm.org/doi/10.1007/978-3-031-22308-2_5) | [Code](https://github.com/womeier/secwasm) |
| [Automated Verification for Secure Messaging Protocols and Their Implementations](https://ieeexplore.ieee.org/document/7961995) | Kobeissi, Bhargavan, Blanchet | IEEE EuroS&P 2017 | 2017 | [PDF](https://ieeexplore.ieee.org/document/7961995) | — |

---

### Static Analysis & Program Analysis

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [Wasmati: An Efficient Static Vulnerability Scanner for WebAssembly](https://arxiv.org/pdf/2204.12575) | Brito, Santos | arXiv | 2022 | [PDF](https://arxiv.org/pdf/2204.12575) | — |
| [WasmA: A Static WebAssembly Analysis Framework for Everyone](https://ieeexplore.ieee.org/document/10123627) | Breitfelder et al. | IEEE SANER 2023 | 2023 | [PDF](https://ieeexplore.ieee.org/document/10123627) | — |
| [WASSAIL: a WebAssembly Static Analysis Library](https://2021.programming-conference.org/details/proweb-2021-papers/3/Wassail-a-WebAssembly-Static-Analysis-Library) | Stiévenart | ProWeb 2021 | 2021 | — | [Code](https://github.com/acieroid/wassail) |
| [Compositional Information Flow Analysis for WebAssembly Programs](https://soft.vub.ac.be/Publications/2020/vub-tr-soft-20-11.pdf) | Stiévenart, De Roover | SCAM 2020 | 2020 | [PDF](https://soft.vub.ac.be/Publications/2020/vub-tr-soft-20-11.pdf) | [Code](https://github.com/acieroid/wassail/releases/tag/scam2020) |
| [Static Stack-Preserving Intra-Procedural Slicing of WebAssembly](https://dl.acm.org/doi/10.1145/3510003.3510070) | Stiévenart, Binkley | ICSE 2022 | 2022 | [PDF](https://dl.acm.org/doi/10.1145/3510003.3510070) | — |
| [That's a Tough Call: Challenges of Call Graph Construction for WebAssembly](https://dl.acm.org/doi/10.1145/3597926.3598104) | Lehmann, Tip | ISSTA 2023 | 2023 | [PDF](https://dl.acm.org/doi/10.1145/3597926.3598104) | — |
| [BREWASM: A General Static Binary Rewriting Framework for WebAssembly](https://arxiv.org/pdf/2305.01454) | Cao et al. | arXiv | 2023 | [PDF](https://arxiv.org/pdf/2305.01454) | [Code](https://github.com/security-pride/BREWasm) |
| [Discovering Vulnerabilities in WebAssembly with Code Property Graphs](https://syssec.dpss.inesc-id.pt/projects/tr-wasmati.pdf) | Lopes | IST Master's Thesis | 2020 | [PDF](https://syssec.dpss.inesc-id.pt/projects/tr-wasmati.pdf) | — |

---

### Fuzzing & Dynamic Analysis

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [WAFL: Binary-Only WebAssembly Fuzzing with Fast Snapshots](https://dl.acm.org/doi/10.1145/3503921.3503924) | Haßler, Maier | ROOTS 2021 | 2021 | [PDF](https://dl.acm.org/doi/10.1145/3503921.3503924) | [Code](https://github.com/fgsect/WAFL) |
| [Fuzzm: Finding Memory Bugs through Binary-Only Instrumentation and Fuzzing of WebAssembly](https://arxiv.org/abs/2110.15433) | Lehmann, Torp | arXiv | 2021 | [PDF](https://arxiv.org/abs/2110.15433) | — |
| [WBSan: WebAssembly Bug Detection for Sanitization and Binary-Only Fuzzing](https://dl.acm.org/doi/10.1145/3696410.3714622) | Wu et al. | WWW 2025 | 2025 | [PDF](https://dl.acm.org/doi/10.1145/3696410.3714622) | — |
| [WRTESTER: Differential Testing of WebAssembly Runtimes via Semantic-aware Binary Generation](https://arxiv.org/pdf/2312.10456) | Cao et al. | arXiv | 2023 | [PDF](https://arxiv.org/pdf/2312.10456) | — |
| [WASMaker: Differential Testing of WebAssembly Runtimes via Semantic-Aware Binary Generation](https://dl.acm.org/doi/10.1145/3650212.3680358) | Cao et al. | ISSTA 2024 | 2024 | [PDF](https://dl.acm.org/doi/10.1145/3650212.3680358) | [Code](https://github.com/security-pride/WASMaker) |
| [WADIFF: A Differential Testing Framework for WebAssembly Runtimes](https://dl.acm.org/doi/pdf/10.1109/ASE56229.2023.00188) | Zhou et al. | IEEE ASE 2023 | 2023 | [PDF](https://dl.acm.org/doi/pdf/10.1109/ASE56229.2023.00188) | — |
| [Wapplique: Testing WebAssembly Runtime via Execution Context-Aware Bytecode Mutation](https://dl.acm.org/doi/10.1145/3650212.3680340) | Zhao, Zeng | ISSTA 2024 | 2024 | [PDF](https://dl.acm.org/doi/10.1145/3650212.3680340) | — |
| [DRWASI: LLM-assisted Differential Testing for WebAssembly System Interface Implementations](https://dl.acm.org/doi/pdf/10.1145/3716379) | Zhang et al. | ACM TOSEM | 2026 | [PDF](https://dl.acm.org/doi/pdf/10.1145/3716379) | — |
| [ESFuzzer: An Efficient Way to Fuzz WebAssembly Interpreter](https://www.mdpi.com/2079-9292/13/8/1498) | Han et al. | Electronics | 2024 | [PDF](https://www.mdpi.com/2079-9292/13/8/1498) | — |
| [FreeWavm: Enhanced WebAssembly Runtime Fuzzing via Parse Tree Mutation and Snapshot](https://dl.acm.org/doi/10.1145/3728877) | Qian et al. | ISSTA 2025 | 2025 | [PDF](https://dl.acm.org/doi/10.1145/3728877) | [Code](https://github.com/messi-q/FreeWavm) |
| [WAGEN: Detecting WebAssembly Runtime Bugs With Grammar-Guided Program Mutation](https://ieeexplore.ieee.org/document/11205981) | Lu et al. | IEEE Trans. Reliability | 2025 | [PDF](https://ieeexplore.ieee.org/document/11205981) | — |
| [WASMDYPA: Effectively Detecting WebAssembly Bugs via Dynamic Program Analysis](https://ieeexplore.ieee.org/document/10589844) | Zheng, Hua | IEEE SANER 2024 | 2024 | [PDF](https://ieeexplore.ieee.org/document/10589844) | — |
| [Wasabi: A Framework for Dynamically Analyzing WebAssembly](https://dl.acm.org/doi/10.1145/3297858.3304068) | Lehmann, Pradel | ASPLOS 2019 | 2019 | [PDF](https://dl.acm.org/doi/10.1145/3297858.3304068) | [Code](https://github.com/danleh/wasabi) |
| [Wasm-R3: Record-Reduce-Replay for Realistic and Standalone WebAssembly Benchmarks](https://arxiv.org/abs/2409.00708) | Baek et al. | arXiv | 2024 | [PDF](https://arxiv.org/abs/2409.00708) | [Code](https://github.com/sola-st/wasm-r3) |
| [WEST: Specification-Based Test Generation for WebAssembly](https://ieeexplore.ieee.org/abstract/document/11334667) | Youn, Shin, Ryu | ASE 2025 | 2025 | [PDF](https://ieeexplore.ieee.org/abstract/document/11334667) | — |

---

### Cryptojacking Detection & Defense

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [MineSweeper: An In-depth Look into Drive-by Cryptocurrency Mining and Its Defense](https://dl.acm.org/doi/10.1145/3243734.3243858) | Konoth et al. | ACM CCS 2018 | 2018 | [PDF](https://dl.acm.org/doi/10.1145/3243734.3243858) | [Code](https://github.com/vusec/minesweeper) |
| [MinerRay: Semantics-Aware Analysis for Ever-Evolving Cryptojacking Detection](https://dl.acm.org/doi/10.1145/3324884.3416580) | Romano, Zheng, Wang | ASE 2020 | 2020 | [PDF](https://dl.acm.org/doi/10.1145/3324884.3416580) | [Code](https://miner-ray.github.io/) |
| [MINOS: A Lightweight Real-Time Cryptojacking Detection System](https://www.researchgate.net/publication/349109071_MINOS_A_Lightweight_Real-Time_Cryptojacking_Detection_System) | Naseem et al. | NDSS 2021 | 2021 | [PDF](https://www.researchgate.net/publication/349109071_MINOS_A_Lightweight_Real-Time_Cryptojacking_Detection_System) | — |
| [WasmGuard: Enhancing Web Security through Robust Raw-Binary Detection of WebAssembly Malware](https://dl.acm.org/doi/10.1145/3696410.3714696) | Sun, Chen, Fu, Lv, Liu, Liu | WWW 2025 | 2025 | [PDF](https://dl.acm.org/doi/10.1145/3696410.3714696) | [Code](https://github.com/Yuxia-Sun/WasmGuard) |
| [POSTER: Detecting WebAssembly-based Cryptocurrency Mining](https://dl.acm.org/doi/10.1145/3319535.3363287) | Bian, Meng, Wang | ACM CCS 2019 | 2019 | [PDF](https://dl.acm.org/doi/10.1145/3319535.3363287) | — |
| [MineThrottle: Defending against Wasm In-Browser Cryptojacking](https://dl.acm.org/doi/10.1145/3366423.3380085) | Bian, Meng, Zhang | WWW 2020 | 2020 | [PDF](https://dl.acm.org/doi/10.1145/3366423.3380085) | [Code](https://github.com/cuhk-seclab/MineThrottle) |
| [Outguard: Detecting In-Browser Covert Cryptocurrency Mining in the Wild](https://dl.acm.org/doi/10.1145/3308558.3313665) | Kharraz et al. | WWW 2019 | 2019 | [PDF](https://dl.acm.org/doi/10.1145/3308558.3313665) | [Code](https://github.com/teamnsrg/outguard) |
| [JABBERWOCK: A Tool for WebAssembly Dataset Generation and Malicious Website Detection](https://www.jstage.jst.go.jp/article/ipsjjip/32/0/32_298/_pdf) | Komiya et al. | IPSJ JIP | 2024 | [PDF](https://www.jstage.jst.go.jp/article/ipsjjip/32/0/32_298/_pdf) | [Code](https://github.com/c-chocolate/Jabberwock) |
| [WASim: Understanding WebAssembly Applications through Classification](https://dl.acm.org/doi/10.1145/3324884.3415293) | Romano, Wang | ASE 2020 | 2020 | [PDF](https://dl.acm.org/doi/10.1145/3324884.3415293) | [Code](https://github.com/WASimilarity/WASim) |

---

### Obfuscation & Malware Evasion

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [Wobfuscator: Obfuscating JavaScript Malware via Opportunistic Translation to WebAssembly](https://ieeexplore.ieee.org/document/9833626) | Romano et al. | IEEE S&P 2022 | 2022 | [PDF](https://ieeexplore.ieee.org/document/9833626) | [Code](https://github.com/js2wasm-obfuscator/translator) |
| [WASMixer: Binary Obfuscation for WebAssembly](https://arxiv.org/abs/2308.03123) | Cao et al. | arXiv | 2023 | [PDF](https://arxiv.org/abs/2308.03123) | [Code](https://github.com/security-pride/WASMixer) |
| [A First Look at Code Obfuscation for WebAssembly](https://dl.acm.org/doi/pdf/10.1145/3507657.3528560) | Bhansali et al. | WiSec 2022 | 2022 | [PDF](https://dl.acm.org/doi/pdf/10.1145/3507657.3528560) | — |
| [Madvex: Instrumentation-based Adversarial Attacks on ML Malware Detection](https://arxiv.org/abs/2305.02559) | Loose et al. | DIMVA 2023 | 2023 | [PDF](https://arxiv.org/abs/2305.02559) | — |
| [WebAssembly Diversification for Malware Evasion](https://arxiv.org/abs/2212.08427) | Cabrera-Arteaga et al. | arXiv | 2022 | [PDF](https://arxiv.org/abs/2212.08427) | [Code](https://github.com/ASSERT-KTH/wasm_evasion) |
| [CROW: Code Diversification for WebAssembly](https://arxiv.org/pdf/2008.07185) | Cabrera Arteaga et al. | arXiv | 2021 | [PDF](https://arxiv.org/pdf/2008.07185) | — |
| [WASM-MUTATE: Fast and Effective Binary Diversification for WebAssembly](https://arxiv.org/abs/2309.07638) | Cabrera-Arteaga et al. | arXiv | 2023 | [PDF](https://arxiv.org/abs/2309.07638) | — |
| [Deceptive bytes: In-depth Evaluation of WebAssembly Obfuscation for Evading Crypto Mining Detection](https://nva.sikt.no/registration/0198eb542a7e-66fdfde1-1ff3-48de-9a47-38fd290d5819) | Harnes | NTNU Master's Thesis | 2023 | — | [Code](https://github.com/HakonHarnes/wasm-obf) |
| [CRYPTIC BYTES: WebAssembly Obfuscation for Evading Cryptojacking Detection](https://arxiv.org/abs/2403.15197) | Harnes, Morrison | arXiv | 2024 | [PDF](https://arxiv.org/abs/2403.15197) | — |
| [SELWasm: A Code Protection Mechanism for WebAssembly](https://ieeexplore.ieee.org/document/9047432) | Sun et al. | IEEE ISPA 2019 | 2019 | [PDF](https://ieeexplore.ieee.org/document/9047432) | — |
| [AndroWasm: Empirical Study on Android Malware Obfuscation through WebAssembly](https://arxiv.org/pdf/2602.18082) | Soi et al. | arXiv | 2026 | [PDF](https://arxiv.org/pdf/2602.18082) | — |
| [The WASM Cloak: Evaluating Browser Fingerprinting Defenses Under WebAssembly Obfuscation](https://arxiv.org/abs/2508.21219) | Sakib et al. | arXiv | 2025 | [PDF](https://arxiv.org/abs/2508.21219) | — |

---

### Side-Channel & Spectre Attacks

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [Swivel: Hardening WebAssembly against Spectre](https://www.usenix.org/system/files/sec21-narayan.pdf) | Narayan et al. | USENIX Security 2021 | 2021 | [PDF](https://www.usenix.org/system/files/sec21-narayan.pdf) | [Code](https://github.com/PLSysSec/swivel) |
| [Vivienne: Relational Verification of Cryptographic Implementations in WebAssembly](https://arxiv.org/abs/2109.01386) | Tsoupidi, Balliu, Baudry | arXiv | 2021 | [PDF](https://arxiv.org/abs/2109.01386) | [Code](https://github.com/romits800/Vivienne) |
| [Lurking Eyes: Detecting Side-Channel Attacks on JavaScript and WebAssembly](https://ieeexplore.ieee.org/document/9261920) | Mazaheri et al. | ISCISC 2020 | 2020 | [PDF](https://ieeexplore.ieee.org/document/9261920) | — |
| [Rapid Prototyping for Microarchitectural Attacks](https://www.usenix.org/system/files/sec22-easdon.pdf) | Easdon et al. | USENIX Security 2022 | 2022 | [PDF](https://www.usenix.org/system/files/sec22-easdon.pdf) | [Code](https://github.com/libtea/frameworks) |

---

### Trusted Execution Environments (TEE / SGX)

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [EDGEDANCER: Secure Mobile WebAssembly Services on the Edge](https://dl.acm.org/doi/10.1145/3434770.3459731) | Nieke, Almstedt, Kapitza | EdgeSys 2021 | 2021 | [PDF](https://dl.acm.org/doi/10.1145/3434770.3459731) | — |
| [WATZ: A Trusted WebAssembly Runtime Environment with Remote Attestation for TrustZone](https://arxiv.org/pdf/2206.08722) | Ménétrey et al. | ICDCS 2022 | 2022 | [PDF](https://arxiv.org/pdf/2206.08722) | [Code](https://github.com/jamesmenetrey/unine-watz) |
| [A Comprehensive Trusted Runtime for WebAssembly with Intel SGX (TWINE)](https://arxiv.org/pdf/2312.09087) | Ménétrey et al. | IEEE TDSC | 2023 | [PDF](https://arxiv.org/pdf/2312.09087) | — |
| [TWINE: An Embedded Trusted Runtime for WebAssembly](https://arxiv.org/abs/2103.15860) | Ménétrey et al. | IEEE ICDE 2021 | 2021 | [PDF](https://arxiv.org/abs/2103.15860) | [Code](https://github.com/jamesmenetrey/unine-twine) |
| [AccTEE: A WebAssembly-based Two-way Sandbox for Trusted Resource Accounting](https://dl.acm.org/doi/10.1145/3361525.3361541) | Goltzsche et al. | Middleware 2019 | 2019 | [PDF](https://dl.acm.org/doi/10.1145/3361525.3361541) | — |
| [SYMGX: Detecting Cross-boundary Pointer Vulnerabilities of SGX Applications](https://dl.acm.org/doi/10.1145/3576915.3623213) | Wang et al. | ACM CCS 2023 | 2023 | [PDF](https://dl.acm.org/doi/10.1145/3576915.3623213) | [Code](https://github.com/PKU-ASAL/WASEM) |
| [Fuzzing SGX Enclaves via Host Program Mutations](https://ieeexplore.ieee.org/document/10190488) | Khan et al. | IEEE EuroS&P 2023 | 2023 | [PDF](https://ieeexplore.ieee.org/document/10190488) | [Code](https://github.com/purseclab/FuzzSGX) |

---

### Smart Contracts & Blockchain

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [WASAI: Uncovering Vulnerabilities in Wasm Smart Contracts](https://dl.acm.org/doi/10.1145/3533767.3534218) | Chen et al. | ISSTA 2022 | 2022 | [PDF](https://dl.acm.org/doi/10.1145/3533767.3534218) | — |
| [WANA: Symbolic Execution of Wasm Bytecode for Cross-Platform Smart Contract Vulnerability Detection](https://arxiv.org/abs/2007.15510) | Wang, Jiang, Chan | arXiv | 2020 | [PDF](https://arxiv.org/abs/2007.15510) | [Code](https://github.com/gongbell/WANA) |
| [EVulHunter: Detecting Fake Transfer Vulnerabilities for EOSIO's Smart Contracts at Webassembly-level](https://arxiv.org/abs/1906.10362) | Quan, Wu, Wang | arXiv | 2019 | [PDF](https://arxiv.org/abs/1906.10362) | [Code](https://github.com/EVulHunter/EVulHunter) |

---

### Browser Security & Web Attacks

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [RØB: Ransomware over Modern Web Browsers](https://www.usenix.org/conference/usenixsecurity23/presentation/oz) | Oz et al. | USENIX Security 2023 | 2023 | [PDF](https://www.usenix.org/conference/usenixsecurity23/presentation/oz) | [Code](https://github.com/cslfiu/RoB_Ransomware_over_Modern_Web_Browsers) |
| [FP-tracer: Fine-grained Browser Fingerprinting Detection via Taint-tracking](https://petsymposium.org/popets/2024/popets-2024-0092.pdf) | Boussaha et al. | PoPETs 2024 | 2024 | [PDF](https://petsymposium.org/popets/2024/popets-2024-0092.pdf) | [Code](https://github.com/soumboussaha/FP-tracer) |
| [WasmView: Visual Testing for WebAssembly Applications](https://dl.acm.org/doi/10.1145/3377812.3382155) | Romano, Wang | ICSE-Companion 2020 | 2020 | [PDF](https://dl.acm.org/doi/10.1145/3377812.3382155) | [Code](https://github.com/wasmview/wasmview.github.io) |
| [WASMEYE: Language- and Platform-Independent Anomaly Detection for WebAssembly](https://dl.acm.org/doi/pdf/10.1145/3721462.3730957) | Vogel et al. | Middleware 2025 | 2025 | [PDF](https://dl.acm.org/doi/pdf/10.1145/3721462.3730957) | — |

---

### Taint Tracking & Information Flow

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [TaintAssembly: Taint-Based Information Flow Control Tracking for WebAssembly](https://arxiv.org/abs/1802.01050) | Fu, Lin, Inge | arXiv | 2018 | — | [Code](https://github.com/wfus/WebAssembly-Taint) |
| [Taint Tracking for WebAssembly](https://arxiv.org/abs/1807.08349) | Szanto, Tamm, Pagnoni | arXiv | 2018 | — | — |
| [SecWasm: Information Flow Control for WebAssembly](https://dl.acm.org/doi/10.1007/978-3-031-22308-2_5) | Bastys et al. | ESORICS 2022 | 2022 | [PDF](https://dl.acm.org/doi/10.1007/978-3-031-22308-2_5) | [Code](https://github.com/womeier/secwasm) |

---

### Reverse Engineering & Program Understanding

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [Finding the Dwarf: Recovering Precise Types from WebAssembly Binaries](https://dl.acm.org/doi/10.1145/3519939.3523449) | Lehmann, Pradel | PLDI 2022 | 2022 | [PDF](https://dl.acm.org/doi/10.1145/3519939.3523449) | — |
| [Multi-modal Learning for WebAssembly Reverse Engineering](https://dl.acm.org/doi/10.1145/3650212.3652141) | Huang, Zhao | ISSTA 2024 | 2024 | [PDF](https://dl.acm.org/doi/10.1145/3650212.3652141) | — |
| [WADEC: Decompiling WebAssembly Using Large Language Model](https://arxiv.org/abs/2406.11346) | She, Zhao | arXiv | 2024 | [PDF](https://arxiv.org/abs/2406.11346) | [Code](https://github.com/security-pride/WaDec) |
| [Automated WebAssembly Function Purpose Identification With Semantics-Aware Analysis](https://dl.acm.org/doi/pdf/10.1145/3543507.3583235) | Romano, Wang | WWW 2023 | 2023 | [PDF](https://dl.acm.org/doi/pdf/10.1145/3543507.3583235) | — |
| [WasmWalker: Path-based Code Representations for Improved WebAssembly Program Analysis](https://arxiv.org/abs/2410.08517) | Robati Shirzad, Lam | arXiv | 2024 | [PDF](https://arxiv.org/abs/2410.08517) | — |

---

### IoT & Embedded Systems

| Title | Authors | Venue | Year | Paper | Code |
|---|---|---|---|---|---|
| [WARDuino: A Dynamic WebAssembly Virtual Machine for Programming Microcontrollers](https://dl.acm.org/doi/10.1145/3357390.3361029) | Gurdeep Singh, Scholliers | MPLR 2019 | 2019 | [PDF](https://dl.acm.org/doi/10.1145/3357390.3361029) | — |
| [Aerogel: Lightweight Access Control for WebAssembly-Based Bare-Metal IoT Devices](https://pmc.ncbi.nlm.nih.gov/articles/PMC10512427/pdf/nihms-1839084.pdf) | Liu, Garcia, Srivastava | IEEE/ACM SEC 2021 | 2021 | [PDF](https://pmc.ncbi.nlm.nih.gov/articles/PMC10512427/pdf/nihms-1839084.pdf) | — |
| [WARD: Efficient Memory Protection for WebAssembly on Tiny Embedded Systems](https://doi.org/10.1109/ACCESS.2025.3650447) | Shin et al. | IEEE Access | 2026 | — | — |
| [eWASM: Practical Software Fault Isolation for Reliable Embedded Devices](https://ieeexplore.ieee.org/document/9211422) | Peach et al. | IEEE TCAD | 2020 | [PDF](https://ieeexplore.ieee.org/document/9211422) | [Code](https://github.com/gwsystems/awsm/) |
| [Exploring and Exploiting the Resource Isolation Attack Surface of WebAssembly Containers](https://www.usenix.org/conference/usenixsecurity25/presentation/yu-zhaofeng) | Yu et al. | USENIX Security 2025 | 2025 | [PDF](https://www.usenix.org/conference/usenixsecurity25/presentation/yu-zhaofeng) | [Code](https://zenodo.org/records/16594863) |
| [Towards Least-Privilege WebAssembly Applications](https://dl.acm.org/doi/10.1145/3801119.3801125) | Blaak, Van Cutsem | Programming 2026 | 2026 | [PDF](https://dl.acm.org/doi/10.1145/3801119.3801125) | — |

---

## Contributing

Found a paper missing? Spotted an error?

[Submit via our Google Form](https://docs.google.com/forms/d/e/1FAIpQLScWuBduYFmNyGv8NqLUIH5XRz3jSBn0V3YxNRINDyOUvRFIhg/viewform)

---

## Disclaimer

All paper entries were imported manually. I apologize if any paper has been misrepresented. Please raise an issue or use the form above to report mistakes.

---

## Maintained by

[@dhruthan](https://github.com/dhruthan)
