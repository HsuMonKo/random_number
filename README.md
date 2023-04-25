# DipSA CICD Workshop

##  Assignment

In this assignment, you will be writing a CICI pipeline to build and push a Docker 
image for the provided Golang application. Your pipeline must perform the 
following tasks

1.  The pipeline should be triggered when a release is published

2.  Check out the correct branch (tag). Use the ref parameter to specify the 
release tag

3.  The pipeline should build the source as a Docker container image where the 
format of the name of the image (image tag) is as follows \
<b>&lt;account name>/&lt;image name>:&lt;tag></b> \
where <b>&lt;account name></b> is the name of your Docker hub account, <b>&lt;image 
name></b> is the image name and <b>&lt;tag></b> is the name of tag that triggered this 
release. Example, if your Docker hub account name is <b>fred</b> , the image name 
is called <b>random_numbers</b>, and the release git tag is <b>v1.1</b>, then the image 
should be called \
<b>fred/random_numbers:v1.1</b>

4.  Push the image to your Docker hub after successfully building the image
Version 1.1.1 Page 2 of 4

5. Send a notification to Slack. The notification should include all the following information in the following order:  
   a. Name - as per your NRIC or passport. This should be your official name  
   b. Matriculation number – the exact format that you use when you sit for your NUS ISS examination  
   c. Email – you can be your NUS or your personal email  
   d. Repository – this is the repository of your work; the URL should be derived from github context  
   e. Image name – the name of the Docker image that you pushed to Docker hub  
   f. Image URL – URL of your image in Docker hub
