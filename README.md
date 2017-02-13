### Title of your forcefield

1. Fork this repo

2. Create your force field `.xml` file based on the [OpenMM](http://openmm.org/) [`.xml` format](http://docs.openmm.org/7.0.0/userguide/application.html#creating-force-fields)
and add [foyer](https://github.com/mosdef-hub/foyer) style SMARTS strings to define your atom types

3. Optionally, add example molecules with correct atomtypes defined as test cases. Execute the testing script using `py.test -v test_atomtyping`

4. Generate your own DOI via Zenodo
  * https://guides.github.com/activities/citable-code/

5. Update the link to the Zenodo DOI badge
  * [![DOI](https://zenodo.org/badge/XXX/USER_NAME/YOUR_FORCEFIELD_REPO.svg)](https://zenodo.org/badge/latestdoi/XXX/USER_NAME/YOUR_FORCEFIELD_REPO)
