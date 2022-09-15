# spaceapps-2022-public-mo-data-exploration


### Creating python Environments with conda 

* To create the python env using conda, execute this command from this directory 

```bash
conda env create --file requirement.yml
```

* Activate your environment using 

```bash
conda activate spaceapps-mo-data
```


* If you cannot see this environment from the kernels dropdown in your jupyter notebook, run the following command 

```bash
ipython kernel install --user --name=spaceapps-mo-data
```

* This allows jupyter to connect with your environment through the ipython kernel 