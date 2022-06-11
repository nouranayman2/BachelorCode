# To Run the test files
1. install miniconda,
2. download the data-set
3.store unzipped data into folder  --data_root parameter accordingly)
4. change dir to root of this project
5. run conda env create -f environment.yml to install the conda environment
6. activate the conda environment with conda sess1
7. Install all the required packages such as Pytorch,Pytorch lightning,librosa
## To train the first machine run the below command:For MADE model
8.python -m experiments.train density --version made --architecture made --n_gaussians 1 --proxy_outliers other_sections --proxy_outlier_lambda 1.0 --margin 0.5 --consistent_with_librosa --machine_type fan
