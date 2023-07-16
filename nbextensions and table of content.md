# Installing extensions in Jupyter

Reference https://stackoverflow.com/questions/49647705/jupyter-nbextensions-does-not-appear/59514338#59514338

Note python needed to be downgraded to Python version 3.8 using the command:
> conda create -n downgrade python=3.8 anaconda
> conda activate downgrade

Then, Jupyter was launched from anaconda navigator in the downgraded version where extensions were visible for the first time.

Table of content was simply ticked. 


The following were also tried at different times during previous attempts
Reference: 

1. https://stackoverflow.com/questions/21151450pip /how-can-i-add-a-table-of-contents-to-a-jupyter-jupyterlab-notebook

2. https://pythonbaba.com/install-nodejs-and-execute-javascript-in-jupyter-notebook-anaconda/#Step_3_Installing_Nodejs

# Install nodejs
conda install -c conda-forge nodejs

# Install npm
npm install -g npm@latest

# TOC as a panel
jupyter labextension install @jupyterlab/toc

# TOC as a cell
conda install -c conda-forge jupyter_contrib_nbextensions
