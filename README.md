# NCIL Data Science Environments

These configuration files will allow you to create dedicated environments (sets of Python and R packages) for typical NCIL use cases. 

The environments:
- `ncil.yml`: Python environment for data science, including Jupyter Lab, pandas, numpy, matplotlib, seaborn, scikit-learn, and more.
- neural_data_science.yml: Python environment for the NESC 3505 neural data science course. Includes all of the packages necessary to work through the textbook chapters, as well as packages for publishing the book (`jupyter-book` and helpers)
- psychopy.yml: Python environment for running PsychoPy experiments. Includes PsychoPy, as well as basic packages for data analysis (pandas, numpy, matplotlib, seaborn, scikit-learn, and more). Adapted from the one provided by PsychoPy, with additions including jupyter notebooks (so you can create and run PsychoPy experiments or code snippets in Jupyter notebooks).


To use, fork this repository to your computer, or just download the individual file you want. Then in a terminal window, `cd` to the folder containing this repository and run:
```
mamba env create -f ncil.yml
```

(or whatever the name of the file is).

This will install all the packages into a dedicated environment. When you want to use it, in a terminal run:
```
mamba activate ncil
```
Then proceed as usual (e.g., run `jupyter lab`). 

If you are using VS Code, you don't need to run `mamba activate`. Instead, when you open a Python file or notebook be sure to select the `ncil` environment in the upper right corner (rather than the default `base` environment).
