# Userguide_GPU_usage_at_IIITG

Step-by-step guide for Server's GPU acess at IIIT Guwahati.


# Account aquisation 

Scholars / Students of IIITG need to get an account / credentials for accessing the GPU from ICT section.

# Installations
 following are the list of tools to be downloaded for better user experience 


Configurations

Download WinSCP and install 
Login to the server using credentials 
Download putty and install it, if it is not installed
Open putty fro WinSCP
Then login using your credentials in PuTTY 
Inside PuTTY activate the anaconda using source ~/anaconda3/bin/activate
Now create a new environment for your personal use using conda create --name myenv
Activate the environment using 
conda activate myenv  for deactivation use conda deactivate myenv 
Install PyTorch using 
conda install pytorch==2.5.0 torchvision==0.20.0 torchaudio==2.5.0 pytorch-cuda=12.4 -c pytorch -c nvidia



Useful commands

nvidia-smi : to check the list of GPU CARDS

CUDA_VISIBLE_DEVICES=2 python check_GPU.py : To select the GPU card, here number 2 represents the available gpu card and check_GPU.py is the name of the program to execute 
top: to check the running processes and respective users
gpustat: to check the status of the GPU cards 
CUDA_VISIBLE_DEVICES=2 nohup python check_GPU.py & :: here nohup before the program file name and & after the program file name  helps to execute the programs in the server without continuos connection with local machine
It returns a process ID that we can check using top command, and it also create a nohup.out file where we can see the progress and output of the program executing in the background  


Tips

For PyTorch GPU CARD 3 is considered as card 1 




