# ZigZag [Documentation](https://kuleuven-micas.github.io/zigzag/) [Tutorial](https://www.youtube.com/watch?v=VgUuG4QaSQQ&list=PLUi74Rw4uFDIuK_6FCF9Bv7SMJlHfG4l3&index=1)
This repository presents the novel version of our tried-and-tested HW Architecture-Mapping Design Space Exploration (DSE) Framework for Deep Learning (DL) accelerators. ZigZag bridges the gap between algorithmic DL decisions and their acceleration cost on specialized accelerators through a fast and accurate HW cost estimation. 

A crucial part in this is the mapping of the algorithmic computations onto the computational HW resources and memories. In the framework, multiple engines are provided that can automatically find optimal mapping points in this search space.

## Installation

Please take a look at the [Installation](https://zigzag-project.github.io/zigzag/installation.html) page of our documentation.

## Getting Started

Please take a look at the [Getting Started](https://kuleuven-micas.github.io/zigzag/getting-started.html) page on how to get started using ZigZag.

Also, a Jupyter Notebook based demo is prepared for new users [here](https://github.com/ZigZag-Project/zigzag-demo).

## Recent changes

In this novel version, we have: 
- Added an interface with ONNX to directly parse ONNX models
- Overhauled our HW architecture definition to:
    - include multi-dimensional (>2D) MAC arrays.
    - include accurate interconnection patterns.
    - include multiple flexible accelerator cores.
- Enhanced the cost model to support complex memories with variable port structures.
- Revamped the whole project structure to be more modular.
- Written the project with OOP paradigms to facilitate user-friendly extensions and interfaces.


## Publication pointers

#### The general idea of ZigZag
L. Mei, P. Houshmand, V. Jain, S. Giraldo and M. Verhelst, "ZigZag: Enlarging Joint Architecture-Mapping Design Space Exploration for DNN Accelerators," in IEEE Transactions on Computers, vol. 70, no. 8, pp. 1160-1174, 1 Aug. 2021, doi: 10.1109/TC.2021.3059962. [paper](https://ieeexplore.ieee.org/document/9360462)

#### Detailed latency model explanation
L. Mei, H. Liu, T. Wu, H. E. Sumbul, M. Verhelst and E. Beigne, "A Uniform Latency Model for DNN Accelerators with Diverse Architectures and Dataflows," 2022 Design, Automation & Test in Europe Conference & Exhibition (DATE), Antwerp, Belgium, 2022, pp. 220-225, doi: 10.23919/DATE54114.2022.9774728. [paper](https://lirias.kuleuven.be/retrieve/661303), [slides](https://docs.google.com/presentation/d/1mPdzEvuhu4923L0qYfEXGqRH7jtnHDlm/edit?usp=sharing&ouid=117150865143314519834&rtpof=true&sd=true), [video](https://drive.google.com/file/d/1o1ZY_rPsR5d8ZNpxxO7be0Tc2KUQIfX_/view?usp=sharing)

#### The new temporal mapping search engine
A. Symons, L. Mei and M. Verhelst, "LOMA: Fast Auto-Scheduling on DNN Accelerators through Loop-Order-based Memory Allocation," 2021 IEEE 3rd International Conference on Artificial Intelligence Circuits and Systems (AICAS), Washington DC, DC, USA, 2021, pp. 1-4, doi: 10.1109/AICAS51828.2021.9458493. [paper](https://ieeexplore.ieee.org/document/9458493), [slides](https://drive.google.com/file/d/1m_4YznH67mxngP3Mlmoj_c8ruRqrjdbq/view?usp=share_link), [video](https://drive.google.com/file/d/1pK3hoy3znto7JfXHj3V_sWv4FdrcTgzA/view?usp=share_link)

#### Apply ZigZag for different design space exploration case studies
P. Houshmand, S. Cosemans, L. Mei, I. Papistas, D. Bhattacharjee, P. Debacker, A. Mallik, D. Verkest, M. Verhelst, "Opportunities and Limitations of Emerging Analog in-Memory Compute DNN Architectures," 2020 IEEE International Electron Devices Meeting (IEDM), San Francisco, CA, USA, 2020, pp. 29.1.1-29.1.4, doi: 10.1109/IEDM13553.2020.9372006. [paper](https://ieeexplore.ieee.org/abstract/document/9372006), [slides](https://docs.google.com/presentation/d/e/2PACX-1vRTB-KJemyLhrBmiZ9c7fL8gpnIevJzB2feNHeAGfcKchkFR698Df2_Wh0CXu8Qrg/pub?start=false&loop=false&delayms=30000), [video](https://drive.google.com/file/d/1tfz9NJKDECWgkYCK_vtir8hf2-Dz5ISh/view?usp=sharing)

V. Jain, L. Mei and M. Verhelst, "Analyzing the Energy-Latency-Area-Accuracy Trade-off Across Contemporary Neural Networks," 2021 IEEE 3rd International Conference on Artificial Intelligence Circuits and Systems (AICAS), Washington DC, DC, USA, 2021, pp. 1-4, doi: 10.1109/AICAS51828.2021.9458553. [paper](https://ieeexplore.ieee.org/abstract/document/9458553), [slides](https://docs.google.com/presentation/d/1IIeNwIfunKE409SmlS3JEIAF-5GyhbCN/edit?usp=sharing&ouid=100287940751782809199&rtpof=true&sd=true), [video](https://drive.google.com/file/d/1SssJKLt89H1SCAeCOUX4ibsZ15ewLKPb/view?usp=sharing)

S. Colleman, T. Verelst, L. Mei, T. Tuytelaars and M. Verhelst, "Processor Architecture Optimization for Spatially Dynamic Neural Networks," 2021 IFIP/IEEE 29th International Conference on Very Large Scale Integration (VLSI-SoC), Singapore, Singapore, 2021, pp. 1-6, doi: 10.1109/VLSI-SoC53125.2021.9607013. [paper](https://ieeexplore.ieee.org/abstract/document/9607013), [slides](https://drive.google.com/file/d/1to0IHQP30CUbjh37LrT_g4Tfjo6VhVx7/view?usp=sharing), [video](https://drive.google.com/file/d/1tjp_0OBiXSFOOF_u3cw9Zr-u4fcJRy9_/view?usp=sharing)

S. Colleman, P. Zhu, W. Sun and M. Verhelst, "Optimizing Accelerator Configurability for Mobile Transformer Networks," 2022 IEEE 4th International Conference on Artificial Intelligence Circuits and Systems (AICAS), Incheon, Korea, Republic of, 2022, pp. 142-145, doi: 10.1109/AICAS54282.2022.9869945. [paper](https://ieeexplore.ieee.org/document/9869945), [slides](https://docs.google.com/presentation/d/1tp11akyAVGg3Y20Aupp2wlTRSgg9nKAQ/edit?usp=sharing&ouid=117150865143314519834&rtpof=true&sd=true), [video](https://drive.google.com/file/d/1tglc-BCGVclrWT-kNhWy02Vms5sjk1zt/view?usp=sharing)

#### Extend ZigZag to support cross-layer depth-first scheduling
L. Mei, K. Goetschalckx, A. Symons and M. Verhelst, " DeFiNES: Enabling Fast Exploration of the Depth-first Scheduling Space for DNN Accelerators through Analytical Modeling," 2023 IEEE International Symposium on High-Performance Computer Architecture (HPCA), 2023 [paper](https://arxiv.org/abs/2212.05344), [slides](https://drive.google.com/file/d/1u_PG9ZhjUZVrH2wnMLDe-PYJeO0RUGLd/view?usp=sharing), [github](https://github.com/ZigZag-Project/DeFiNES)

#### Extend ZigZag to support multi-core layer-fused scheduling
A. Symons, L. Mei, S. Colleman, P. Houshmand, S. Karl and M. Verhelst, “Towards Heterogeneous Multi-core Accelerators Exploiting Fine-grained Scheduling of Layer-Fused Deep Neural Networks”, <i>arXiv e-prints</i>, 2022. doi:10.48550/arXiv.2212.10612. [paper](https://arxiv.org/abs/2212.10612), [github](https://github.com/ZigZag-Project/stream)

S. Karl, A. Symons, N. Fasfous and M. Verhelst, "Genetic Algorithm-based Framework for Layer-Fused Scheduling of Multiple DNNs on Multi-core Systems," 2023 Design, Automation & Test in Europe Conference & Exhibition (DATE), Antwerp, Belgium, 2023, pp. 1-6, doi: 10.23919/DATE56975.2023.10137070. [paper](https://ieeexplore.ieee.org/document/10137070), [slides](https://www.dropbox.com/s/rv8qiko59h4pp0s/Genetic%20Algorithm-based%20Framework%20for.pptx?dl=0), [video](https://www.dropbox.com/s/12v94stvevj9xns/Genetic%20Algorithm-based%20Framework%20for.mp4?dl=0)
