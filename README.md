### Getting Started

Installation of Foyer and required tools
```bash
conda install -c omnia -c mosdef parmed foyer pytest
```

Creating a new force field
1. Duplicate the force field template.  This can be done in various ways:
 * Use the "Import repository" function on github.com (in the "+" at top right) to import the template  https://github.com/mosdef-hub/forcefield_template 
 * Follow the documentation on this page: https://help.github.com/articles/duplicating-a-repository/

2. Create your force field `.xml` file based on the [OpenMM](http://openmm.org/) [`.xml` format](http://docs.openmm.org/7.0.0/userguide/application.html#creating-force-fields)
and add [foyer](https://github.com/mosdef-hub/foyer) style SMARTS strings to define your atom types. 
 * Example force field files:
  * https://github.com/chrisiacovella/OPLSaa_perfluoroalkanes

3. Optionally, add example molecules with correct atomtypes defined as test cases. Execute the testing script using `py.test -v --tb=line`
 * Note, even if test molecules are not created, running py.test is recommended, as this will perform checking of your data file for proper syntax and ensure that all atom types references are defined.

4. Generate your own DOI via Zenodo
  * https://guides.github.com/activities/citable-code/

5. Update the link to the Zenodo DOI badge
  * [![DOI](https://zenodo.org/badge/XXX/USER_NAME/YOUR_FORCEFIELD_REPO.svg)](https://zenodo.org/badge/latestdoi/XXX/USER_NAME/YOUR_FORCEFIELD_REPO)

The text above can be removed upon publishing a forcefield, but please be sure to include the following, 

### [Title of your forcefield]

 * Source: [Journal reference(s) if parameters are published (include DOI link)]

 * Forcefield file initially created [DATE] by [Creator(s)]

#### Source Notes:
< Add specific notes about parameters, e.g., if a set of parameters come verbatim from prior work, provide details and a DOI >

#### Additional Notes:
< Add any other relevant information. Also For consistency, please define conversion factors used. Note that we strongly suggest follow unit conversions defined in openMM, as detailed below. >
 * PI is defined as 3.141592653589 for conversion to radians, consistent with openMM.
 * kcal/mol to kJ/mol conversion factor of 4.184, consistent with openMM.
 
### Force field DOI
  * [![DOI](https://zenodo.org/badge/XXX/USER_NAME/YOUR_FORCEFIELD_REPO.svg)](https://zenodo.org/badge/latestdoi/XXX/USER_NAME/YOUR_FORCEFIELD_REPO)

