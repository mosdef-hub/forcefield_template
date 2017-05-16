# Create your custom force field

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

### Staying up to date with our template `XML` file
As we continue to increase our support for many `SMARTS` features within
`Foyer`, we will be updating our testing suite to also reflect these changes.
To keep you up to date with these changes, we have included `FEATURE`.
 
To stay up to date with these changes, simply run in your `master` branch:
```bash
    ./FEATURE update_xml_template
```

---

### Implement own forcefield
1. Fork this repository
    * More information about forking through GitHub can be found [here.](https://guides.github.com/activities/forking)

2. Follow [this](tutorial/README.md) tutorial for developing own force field and `XML`
format for `Foyer`.

___

### Giving back to the community
Once you have successfully generated a custom forcefield for your system of interest, making this
information easily testable and citable by others is highly recommended. An optimal way to make this
forcefield readily citable is through a custom DOI. Zenodo provides a simple way to develop
a DOI for your forked repository.

1. Generate your own DOI via Zenodo
  * https://guides.github.com/activities/citable-code/

2. Update the link to the Zenodo DOI badge
  * [![DOI](https://zenodo.org/badge/XXX/USER_NAME/YOUR_FORCEFIELD_REPO.svg)](https://zenodo.org/badge/latestdoi/XXX/USER_NAME/YOUR_FORCEFIELD_REPO)

