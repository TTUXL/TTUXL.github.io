## HPC Guide
---
### Loading Miniconda module

     $ module load miniconda     % loading miniconda

     $ conda info  --envs        % list information of existed work environment
     or $ conda env list


### Creating Miniconda environment

    $ conda create --name tf-2.0 python=3.7   % create new environment name is tf-2.0 ,python version is 3.7
    or $ conda create -n tf-2.0 python=3.7   

    $ source activate tf-2.0                  % acivate environment or Simply understood as logging in to a windows account
    or conda activate tf-2.0                  % As of conda 4.4, conda activate is the preferred way to activate an environment.

    $ source deactivate                       % exit environment
    or conda deactivate

    $ conda remove -n tf-2.0 --all            $ delete tf-2.0 environment
    or $ conda env remove --name tf-2.0

###
