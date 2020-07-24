## HPC Guide
---
### Loading Miniconda module

     module load miniconda     % loading miniconda
     conda info  --envs        % list information of existed work environment


### Creating Miniconda environment
>conda create --name tf-2.0 python=3.7   % create new environment name is tf-2.0 ,python version is 3.7
>source activate tf-2.0                  % acivate environment
>do somethings
>source deactivate
