### *WARNING: PROJECT UNFINISHED AND ABANDONED - DO NOT USE!*

Due to lack of time, I regrettably had to abandon this project while it was still in an early state. The current prototype on the `master` branch works only *qualitatively* and only on a *toy example*. Attempts at validating it with real data **did _not_ succeed** and further work to fix/improve the pipeline turned into an endless rabbit hole (see branch `Jonas`).

**I strongly caution anyone who wishes to use or build on this work;** the current implementation may produce **incorrect results** and is likely **highly imprecise, unstable, and slow!** It would require extensive cleaning, testing, iteration, refactoring, and validation against baseline data in order to become functional and trustworthy.

![contact_email_image_JH](_images/email_JH.png)

----

# pyCFI

### python-based Cellular Force Inference

A python package for inferring cell interfacial tensions from segmented 3D image stacks, based on [a 2017 paper](https://www.ncbi.nlm.nih.gov/pubmed/28348259) from the lab of G. Wayne Brodland.


### Background

Cellular mechanics are at the heart of tissue self-organization during animal morphogenesis. Many common phenomena such as cluster formation and cell sorting can be explained by theoretical models based on force balance considerations of cell contractility and cell-cell adhesion, which jointly mediate effective interfacial tension [[Brodland, 2002]](https://www.ncbi.nlm.nih.gov/pubmed/12002128).

However, experimentally measuring interfacial tensions in developing tissues remains extremely challenging and existing methods have various limitations. For instance, micropipette aspiration requires the surfaces of interest to be freely exposed to the medium [[Guevorkian & Maître, 2016]](https://www.ncbi.nlm.nih.gov/pubmed/28215336), which is rarely the case in animal development. Methods based on laser nano-surgery sidestep this issue [[Smutny et al., 2015]](https://www.ncbi.nlm.nih.gov/pubmed/25245697) but are difficult to interpret in a 3D context and cause destruction in the tissue with every cut, limiting throughput.

In 2017, Veldhuis and colleagues presented a novel approach to meet this challenge: a method for computational inference of interfacial tensions directly from cell shapes as captured by 3D confocal microscopy [[Veldhuis et al., 2017]](https://www.ncbi.nlm.nih.gov/pubmed/28348259). Regrettably, they were unable to release their code for use by others.


### Project aims

We aim to implement the interfacial tension inference approach described by Veldhuis and colleagues as a small, clean and efficient python package that can be used with a command-line interface or with a scikit-learn-style API.

Data from the study by Veldhuis and colleagues will be used to validate our implementation and to test possible improvements. The resulting code will be made available to the community and further improved, extended and maintained as Open Source Software.


### Authors & acknowledgements

- Authors: Jonas M. Hartmann, Harsh Thakkar, Vivek Thatte, and Luís A. N. Amaral
- We thank G. Wayne Brodland and Jim Veldhuis for responding to our inquiries regarding cellFIT3D and for providing us with data from their publication for validation of our implementation
- We thank Helio Tejedor for his help on various coding and geometry issues and Martin Gerlach for his input on Gram-Schmidt orthogonalization
