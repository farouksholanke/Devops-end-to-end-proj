
## 🚀 COMPREHENSIVE CI/CD PIPELINE FOR DEPLOYMENT OF A WEB APPLICATION USING


In this project I will set up a comprehensive CI/CD pipeline that automates the integration and
delivery process from when updates to the source code for a web application are committed to
GitHub repository
- Jenkins automatically pulls the code from the GitHub repository with the help of poll SCM enabled
to detect changes to the source and builds the code with the help of Maven which generates a
(.war) artifact and pushes onto an Ansible server
- Jenkins also automatically executes my Ansible playbook which creates and image with the
artifact and commits it into my Docker hub repository
- in Jenkins, the successful build of the continuous integration job will trigger the continuous
deployment job
- In the CD job, Jenkins will initialize and Ansible playbook that will execute a deployment and
service file for a Kubernetes cluster with the image and finally the application is up and running with
the latest code
![image](https://github.com/user-attachments/assets/2ac862d7-2133-485c-8903-215edf4262d8)


I am going to demonstrate this step by step, first manually on a virtual machine then automate the
integration and deployment process with Jenkins on a Docker container, then Ansible (as a
deployment tool to execute commands and configure my target environment in a more efficient
way) and then Kubernetes container management system for high availability and fault tolerance
using Amazon EKS


## TOOLS
Git, GitHub, Jenkins, Maven, Ansible, Docker, AWS(EC2, CloudFormation,), Ansible, Kubernetes
(AWS EKS)
