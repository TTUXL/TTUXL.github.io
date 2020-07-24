## HPC Guide
---
### Loading Miniconda module

     $ module load miniconda                 % loading miniconda

     $ conda info  --envs                    % list information of existed work environment
     or $ conda env list


### Creating Miniconda environment

    $ conda create --name tf-2.0 python=3.7   % create new environment name is tf-2.0 ,python version is 3.7
    or $ conda create -n tf-2.0 python=3.7   

    $ source activate tf-2.0                  % acivate environment or Simply understood as logging in to a windows account
    or conda activate tf-2.0                  % As of conda 4.4, conda activate is the preferred way to activate an environment.

    $ source deactivate                       % exit environment
    or conda deactivate

    $ conda remove -n tf-2.0 --all            % delete tf-2.0 environment
    or $ conda env remove --name tf-2.0

### login GPU node(First install)

    $ hpcshell --gres=gpu --mem=16G           % Apply for GPU node
    $ source activate tf-2.0                  % Activate this environment on the GPU Node
    $ pip install --upgrade tensorflow-gpu    % TF-GPU can only be installed on GPU nodes
    $ module load cuda10.0 cudnn              % Load the CUDA driver
    $ Python helloworld.py                    % run demo code
    $ exit                                    % exist

---
### Quick to use

    $ module load miniconda
    $ source activate tf-2.0-test
    $ hpcshell --gres=gpu --mem=8G
    $ python xxx.py
    $ exit
---
### Submitting jobs using script
    1. create a new txt and name xx.sh
>#!/bin/bash  
>#SBATCH --gres=gpu:1 --mem=4G  
>#SBATCH --time=1:00:00  
>module load miniconda  
>module load cuda10.0 cudnn  
>source activate tf-2.0-test
>python xxx.py

    2. $ scp /home/xx.sh xli44@shell.hpc.tntech.edu:   % cope File to server.File directory is set according to personal computer

    3. $ sbatch xx.sh
