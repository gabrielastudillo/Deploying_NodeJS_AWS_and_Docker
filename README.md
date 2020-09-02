# Deploying NodeJS in AWS with Docker (ERS and EKS)
In this guide, I present the steps on how to dockerize a Node.js application and then deploy it to Amazon Web Services (AWS) using Amazon Elastic Container Registry (ECR) and Amazon Elastic Container Service (ECS).

# Setup
I am using the Cloud9 envirnment in AWS as its provides an IDE and most of the required compnents are already preinstalled. Follow this steps:
 #1. Update system
 sudo yum update
 #2. Install Node and NVM
  To install Node.js, begin by running this command to download Node Version Manager (nvm). (nvm is a simple Bash shell script that is useful for installing and managing Node.js     versions. For more information, see Node Version Manager on the GitHub website.)

    curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
    To start using nvm, either close the terminal session and start it again, or source the ~/.bashrc file that contains the commands to load nvm.

    . ~/.bashrc
    Run this command to install the latest version of Node.js.

    nvm install node
    
    
 #3. Check Docker
 Chek if Docker is installed on your system (including Docker Engine and Docker CLI Client). To check if the installation worked, run this command in the terminal:
 
 $ docker --version
 
