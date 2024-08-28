<a href="https://www.gnu.org/licenses/gpl-3.0">
  <img src="https://img.shields.io/badge/License-GPLv3-blue.svg" align="left" height="20"/>
</a> 

<a href="https://gitpod.io/#https://github.com/Adamtaranto/python-novice-dataframes">
  <img src="https://gitpod.io/button/open-in-gitpod.svg" align="right" height="35"/>
</a>

<br>

# Working locally

## On Mac or Linux machine


Clone this repo and navigate into the dir:

```bash
git clone https://github.com/Adamtaranto/python-novice-dataframes.git
cd python-novice-dataframes
``

Set up a python environment with the packages we will be using:

### Micromamba

Setup new micromamba environment.

```bash
# Create env and install packages from yml
micromamba env create --name pandas-workshop --file environment.yml

# Activate the environment
micromamba activate pandas-workshop
```

### Or using Conda

```bash
# Create env and install packages from yml
conda env create --name pandas-workshop --file environment.yml

# Activate the environment
conda activate pandas-workshop
```

### Or using pip

```bash
pip install matplotlib numpy pandas scipy seaborn jupyterlab
```

Now you can launch Jupyter Lab.

```bash
jupyter lab
```

## Setup for Windows

1. [Install GitBash](https://wehi-education.github.io/git-novice/#installing-git)
2. [Install VS Code](https://code.visualstudio.com/download)
    If you are using VS Code on a windows machine you will also need to [set your default shell as "GitBash"](https://code.visualstudio.com/docs/sourcecontrol/intro-to-git#_git-bash-on-windows).
3. Install [miniforge3](https://conda-forge.org/miniforge/)
4. Open a GitBash shell and run this command to enable Conda: `~/miniforge3/Scripts/conda.exe init bash` 
5. From a new GitBash shell use `conda` to install packages:
`conda install -c conda-forge jupyterlab pandas numpy matplotlib seaborn scipy`


# Working in Gitpod

Click the Gitpod button at the top of this README to launch a gitpod workspace with all the required software pre-installed. 

If you have a paid Gitpod account you can increase the timout limit on your workspace. 
Otherwise you will need to restart the workspace periodically.

```bash
# Increase gitpod timeout setting
gp timeout set 6h
```

Manually start Jupyter session

```bash
# Launch jupyter-lab
jupyter lab --NotebookApp.allow_origin='*' --NotebookApp.allow_remote_access=True --NotebookApp.token='' --NotebookApp.password='' --no-browser --port=8888
```

**Note:** See other [gitpod settings](https://www.gitpod.io/docs/references/gitpod-cli#set) here.


