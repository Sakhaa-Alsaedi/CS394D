# CS394D
The Final project of CS394D:Using Efficient Deep Learning to Classifying Disease Severity of COVID-19 Patients by using X-ray Chest Images

To run the code follow the the following steps:

Step 1: alocate a node on KAUST ibex with 150Gb memory, gpu:v100:1 GPU srun --time=15:00:00 --mem=150Gb --gres=gpu:v100:1 --resv-port=1 --pty bash -l

Step 2: load the following packges module load cuda module load anaconda3

Step 3: Crate an enviroments conda create -p env source activate ./env

Step 4: Run Jupyter notebook on ibex, copy the link and add ibex.kaust.edu.sa after the node name module load anaconda3 export JUPYTER_RUNTIME_DIR=/tmp jupyter notebook --no-browser --ip=0.0.0.0 --port=$SLURM_STEP_RESV_PORTS

Important notes: The main experiment in the Main Models folder, which contains the transfer learning approach and pre-trained model on the augmented dataset. The code implemented on jupyter notebook, you just need to load the attached dataset and run blocks.


DATASET:
1- The public chest X-ray images available on https://www.kaggle.com/tawsifurrahman/covid19-radiography-database

Note:
load data and change directories to your directory.
since the size of data massive, only a very small part from augmented images generated from the GAN and transformation part is available on the following:
https://drive.google.com/file/d/14hfHZCijMiE5m1G1VJ-9L_z66_Hl3F8H/view?usp=sharing
