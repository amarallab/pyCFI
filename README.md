# pyCFI

### python-based Cellular Force Inference

##### August 21, 2019

We are developing a python package for inferring cell interfacial tensions from segmented 3D image stacks, based on [a 2017 paper](https://www.ncbi.nlm.nih.gov/pubmed/28348259) from the lab of G. Wayne Brodland. The project will go fully Open Source once the first version is ready for release.

![contact Jonas Hartmann - email image](_images/email_JH.png)

----

### ++ WARNING: Work In Progress -- Do Not Use! ++

This project is under active development and is still in an early state. The current implementation may produce **incorrect results** and is likely **imprecise, unstable, and slow!** Over the next couple of months, we will clean, test, refactor, improve and validate this code, as well as provide APIs and documentation.

***++ Please check back later this year! ++***

----

### Background

Cellular mechanics are at the heart of spatial tissue self-organization during animal morphogenesis. Many common phenomena such as cluster formation and cell sorting can be explained by theoretical models based on force balance considerations of cell contractility and cell-cell adhesion, which jointly mediate effective interfacial tension [[Brodland, 2002]](https://www.ncbi.nlm.nih.gov/pubmed/12002128).

However, experimentally measuring interfacial tensions in developing tissues remains extremely challenging and existing methods have various limitations. For instance, micropipette aspiration requires the surfaces of interest to be freely exposed to the medium [[Guevorkian & Maître, 2016]](https://www.ncbi.nlm.nih.gov/pubmed/28215336), which is rarely the case in animal development. Methods based on laser nano-surgery sidestep this issue [[Smutny et al., 2015]](https://www.ncbi.nlm.nih.gov/pubmed/25245697) but are difficult to interpret in a 3D context and cause destruction in the tissue with every cut, limiting throughput.

In 2017, Veldhuis and colleagues presented a novel approach to meet this challenge: a method for computational inference of interfacial tensions directly from cell shapes as captured by 3D confocal microscopy [[Veldhuis et al., 2017]](https://www.ncbi.nlm.nih.gov/pubmed/28348259).

*Regrettably, they were unable to release their code for use by others.*


### The pyCFI Project

We aim to implement the interfacial tension inference approach described by Veldhuis and colleagues as a small, clean and efficient python package that can be used with a command-line interface or with a scikit-learn-style API.

Data from the study by Veldhuis and colleagues will be used to validate our implementation and to test possible improvements. The resulting code will be made available to the community and further improved, extended and maintained as Open Source Software.


### Authors & Acknowledgements

- Authors: Jonas M. Hartmann, Harsh Thakkar, Vivek Thatte, and Luís A. N. Amaral
- We thank G. Wayne Brodland and Jim Veldhuis for responding to our inquiries regarding cellFIT3D and for providing us with data from their publication so we can validate our implementation
- We thank Helio Tejedor for his help on various coding and geometry issues and Martin Gerlach for his input on Gram-Schmidt orthogonalization