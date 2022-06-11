# BachelorCode
## To run the code install miniconda
### download the data-set
#### store unzipped data into folder ~/shared/DCASE2021/task2 (or set --data_root parameter accordingly)
##### change dir to root of this project
###### run conda env create -f environment.yml to install the conda environment
####### activate the conda environment with conda activate dcase2021_task2
######### Install all the required packages such as Pytorch,Pytorch lightning,librosa
########## To train the first machine run the below command:For MADE model
python -m experiments.train density --version made --architecture made --n_gaussians 1 --proxy_outliers other_sections --proxy_outlier_lambda 1.0 --margin 0.5 --consistent_with_librosa --machine_type fan
