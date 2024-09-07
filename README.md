# assignment3-5
Submission of assignment3-5

## 1. Retrieve an authentication token and authenticate your Docker client to your registry using the AWS CLI:

`aws ecr get-login-password --region ap-southeast-1 | docker login --username AWS --password-stdin 637423510314.dkr.ecr.ap-northeast-1.amazonaws.com`

Note: If you receive an error using the AWS CLI, make sure that you have the latest version of the AWS CLI and Docker installed.

## 2. Build your Docker image using the following command. You can skip this step if your image is already built:

`docker build -t kerenp/assignment3-5 .`

## 3. After the build completes, tag your image so you can push it to this repository:

`docker tag kerenp/assignment3-5:latest 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com/kerenp/assignment3-5:latest`

## 4. Run the following command to push this image to your newly created AWS repository:

`docker push 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com/kerenp/assignment3-5:latest`