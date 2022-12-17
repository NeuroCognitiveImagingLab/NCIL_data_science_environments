# Create a NCIL data science environment
Create data science environment in python for NCIL

To use, download/clone the ncil.yml file to your computer (home directory is fine). Then in a terminal window, in the same directory where you saved the ncil.yml file, run:
```
mamba env create -f ncil.yml
```
This will install all the packages into a dedicated environment. When you want to use it, in a terminal run:
```
mamba activate ncil
```
Then proceed as usual (e.g., run `jupyter lab`). 

If you are using VS Code, you don't need to run `mamba activate`. Instead, when you open a Python file or notebook be sure to select the `ncil` environment in the upper right corner (rather than the default `base` environment).
