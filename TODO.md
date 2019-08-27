## pyCFI To Do List

### Core Development

- Brodland approach
    - Go through FLAGs and see if some improvements can be made (only as necessary)


- Our approach
    - Go through FLAGs and see if some improvements can be made (only as necessary)


- Next steps
    - Convert the two notebooks into a python module
    - Implement scikit-learn-like API
    - Implement commandline interface


### Testing & Validation

- Brodland data
	- Parse out the data JV sent
	- Test our results vs. the paper's results
	- Iteratively make improvements to precision, robustness & performance


- Ventral furrow data
	- Look into the possibility of obtaining some segmented ventral furrow data
	- A lot is known about tensions in early Drosophila; could be a good benchmark!


- Read up on & implement quality control measures
- Code review HT!
- Add a test suite?!


### Extensions

- Implement the pure 2D version (should be straightforward) ->> HT/VT
	- First as a notebook
	- Then as an option in the module


- Add inference of cytoplasmic pressures
	- First do this in 2D, where it has been fully described in one of the CellFIT papers
	- Then also port it to 3D (should be possible)


- Develop some nice options for result visualization and analysis!


### Community & Publication Stuff

- Extend the README
- Write documentation
	- Purpose, principles, limitations
	- Quick-start guide
	- Installation & dependencies
	- Usage instructions
	- Detailed description of our implementation
	- FAQ & known issues
- Write a nice tutorial notebook?
- Add OSS community stuff (code of conduct, etc...)
- Look into packaging & releases (GitHub, PyPI, conda)


- Publication in JOSS
    - Check publication requirements
    - Implement requirements
    - Submit to JOSS

