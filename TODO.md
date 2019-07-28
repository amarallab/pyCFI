## pyCFI To Do List

### Core Development

- Brodland approach
    - Fix the orthogonal plane projection
    - Add registration of the vectors and a better way of getting a consensus
    - Clean & comment the notebook
    - Re-implement the notebook with streamlining, fixes, improvements
    	- Clean nomenclature (TE -> TN)


- Our approach
    - Finish vector extraction
    - Add the equations
    - Clean & comment the notebook
    - Re-implement the notebook with streamlining, fixes, improvements
    	- Clean nomenclature (TE -> TN)


- Next steps
    - Convert the two notebooks into a python module
    - Implement scikit-learn-like API
    - Implement commandline interface


### Testing & Validation

- Brodland data
	- Parse out the data Jim Veldhuis sent
	- Test our results vs. the paper's results
	- Iteratively make improvements to precision, robustness & performance


- Lateral line data
    - Also test on some lateral line data to further improve robustness & performance


- Read up on & implement quality control measures
- Develop some nice visualization options
- Code review Helio!


### Extensions

- Implement the 2D version (should be straightforward)
	- First as a notebook
	- Then as an option in the module


- Add inference of cytoplasmic pressures
	- Best to first do this in 2D, where it has been fully described
	- Then also port it to 3D


### Community & Publication Stuff

- Write proper README
- Write documentations
	- Purpose, principles, limitations
	- Quick-start guide
	- Installation & dependencies
	- Usage instructions
	- FAQ & known issues
- Add license, community guidelines, ...
- Maybe: add a test suite
- Look into packaging & releases (GitHub, PyPI, conda)


- Publication in JOSS
    - Check publication requirements
    - Implement requirements
    - Submit to JOSS



