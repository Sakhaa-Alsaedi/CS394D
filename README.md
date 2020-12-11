# CS394D
The Final project of CS394D:Using Efficient Deep Learning to Classifying Disease Severity of COVID-19 Patients by using X-ray Chest Images

To run the code follow the the following steps:

Step 1: alocate a node on KAUST ibex with 150Gb memory, gpu:v100:1 GPU srun --time=15:00:00 --mem=150Gb --gres=gpu:v100:1 --resv-port=1 --pty bash -l

Step 2: load the following packges module load cuda module load anaconda3

Step 3: Crate an enviroments conda create -p env source activate ./env

Step 4: Run Jupyter notebook on ibex, copy the link and add ibex.kaust.edu.sa after the node name module load anaconda3 export JUPYTER_RUNTIME_DIR=/tmp jupyter notebook --no-browser --ip=0.0.0.0 --port=$SLURM_STEP_RESV_PORTS

Important notes: The main experiment in the Main Models folder, which contains the transfer learning approach and pre-trained model on the augmented dataset. The code implemented on jupyter notebook, you just need to load the attached dataset and run blocks.
