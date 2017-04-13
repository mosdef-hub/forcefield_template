# Create your custom forcefield

The goal of this repositiory is to provide the templates and examples necessary for you to quickly
set up a custom forcefield of your own for atomtyping, and to quickly validate your results as
well.


### Hierarchy
* `tutorial/` - example custom forcefield and validation script
* `forcefield_template.xml` - empty `.xml` file to add a custom forcefield
___

### Installation Requirements
The following packages and their dependencies are necessary for a usable `foyer` environment.
Continuum's [`Anaconda`](https://www.continuum.io/downloads) python package manager is
recommended.

#### Installation (using `Anaconda`):
```bash
conda install -c omnia -c mosdef parmed foyer pytest
```
___

### Implement own forcefield
1. Fork this repository
    * More information about forking through GitHub can be found [here.](https://guides.github.com/activities/forking)

2. Create your force field `.xml` file based on the [OpenMM](http://openmm.org/) [`.xml` format](http://docs.openmm.org/7.0.0/userguide/application.html#creating-force-fields)
and add [foyer](https://github.com/mosdef-hub/foyer) style SMARTS strings to define your atom types
    - A **template** forcefield `.xml` file is located here with the name
    - An **example** forcefield `.xml` file can be found in the `tutorial/` directory.
    `forcefield_template.xml`

3. Optionally, add example molecules with correct atomtypes defined as test cases. Execute the testing script using `py.test -v --tb=line`

___

### Giving back to the community
Once you have successfully generated a custom forcefield for your system of interest, making the
code easily testable and citable by others is highly recommended. An optimal way to make this
forcefield readily citable is through a custom DOI. Zenodo provides a simple way to develop
a DOI for your forked repository.

1. Generate your own DOI via Zenodo
  * https://guides.github.com/activities/citable-code/

2. Update the link to the Zenodo DOI badge
  * [![DOI](https://zenodo.org/badge/XXX/USER_NAME/YOUR_FORCEFIELD_REPO.svg)](https://zenodo.org/badge/latestdoi/XXX/USER_NAME/YOUR_FORCEFIELD_REPO)

