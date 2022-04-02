# MAHGNN
## Install
To use MAHGNN you must make sure that your python version is greater than 3.7. If you don’t know the version of python you can check it by:
```python
python
>>> import platform
>>> platform.python_version()
'3.7.13'
```
### Environment Requirement
The required packages are as follows:
- PyTorch==1.7.0
- PyTorch-Geometric==1.5.0
- numpy==1.19.2
- scikit-learn==0.21.3

## Data availability
In the "datasets" folder, we provide the compressed format of the datasets T1,T2 used in the paper. If you want to use them, please download and unzip them first. 
- T1
- drug-disease associations in the T1 dataset were selected from ZhangDDA
- sim_path.txt: pathway similarity matrix
- sim_structure.txt: target similarity matrix
- sim_drug_interaction.txt:drug-drug interactions similarity matrix
- sim_enzyme_sim.txt:drug enzymes similarity matrix
- spilt_x.mat:10 cross validation index
- p_r.pt:protein-drug associations
- p_d.pt:protein-disease associations
- p_p.pt:protein-protein associations
- T2
- drug-disease associations in the T2 dataset were selected from repoDB
- sim_path.txt: pathway similarity matrix
- sim_structure.txt: target similarity matrix
- sim_drug_interaction.txt:drug-drug interactions similarity matrix
- spilt_x.mat:10 cross validation index
- p_r.pt:protein-drug associations
- p_d.pt:protein-disease associations
- p_p.pt:protein-protein associations
## Usage
### Quick start
We use the dataset T1 to illustrate an example. You should first enter the "datasets" folder and unzip the "T1.zip" file. Then you just need to go back to the MAHGNN file directory and run the following code:

```bash
python main.py --dataset T1
```
###T2 Datesets

```bash
python main.py --dataset folder_name
```
