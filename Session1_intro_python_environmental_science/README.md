# Session 1 - Introduction to Python for Environmental Science

In this session, we will look at typical python tools for loading, analysing and visualising data for environmental science.

### Creating python Environments with conda 

[Conda](https://docs.conda.io/projects/conda/en/latest/) is Package, dependency and environment management for any language---Python, R, Ruby, Lua, Scala, Java, JavaScript, C/ C++, FORTRAN

If you don't already have Conda, [install miniconda here](https://docs.conda.io/en/latest/miniconda.html)

* To create the python env using conda, in the command line execute this command from this directory 

```bash
conda env create --file requirements.yml
```

* Activate your environment using 

```bash
conda activate spaceapps-mo-envsci
```

* Once your conda environment is activated, launch jupyter lab web interface by running the following command 

```bash
jupyter lab
```

### Downloading data

There is some data that it would be useful to have downloaded ahead of the start of the session. Please see the section titled <b>Getting the sample data</b> in the [03_gridded_data.ipynb](https://github.com/informatics-lab/spaceapps-2022-mo-bootcamp/blob/main/Session1_intro_python_environmental_science/03_gridded_data.ipynb) notebook for instructions on how to download the data from the Zenodo archive. 
