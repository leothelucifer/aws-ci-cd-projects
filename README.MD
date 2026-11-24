## End to End MAchine Learning Project

1. Docker Build checked
2. Github Workflow
3. Iam User In AWS
create user and execute below command in cloud shell or add permissions policy from console
  ~ $ aws iam attach-user-policy \
     --user-name cicd-user-prml \
     --policy-arn arn:aws:iam::aws:policy/AmazonEC2ContainerRegistryPowerUser

## Docker Setup In EC2 commands to be Executed

#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

## Configure EC2 as self-hosted runner:

## Setup github secrets:

AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = ap-southeast-1

AWS_ECR_LOGIN_URI = demo>>  548597179073.dkr.ecr.ap-southeast-1.amazonaws.com

ECR_REPOSITORY_NAME = studentperformance

--------------------------------------
