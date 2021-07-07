# cfncross

**#1 sample ansible code to create codepipeline using cloudformation**
cloudform-codepipeline1.yml**  is used to create codepiple using cloudformations and it is referncing  codepipeline-cfn-custom.yml ( where actual code for deployment writtern)
execution command : ansible-playbook cloudform-codepipeline1.yml

**#2sample ansible code to create vpc using cloudformation

cloudform-vpc.yml  is used to create codepiple using cloudformations and it is referncing  SampleNetworkCrossStack.template
execution command : ansible-playbook cloudform-codepipeline1.yml


**#3sample ansible code to create ec2 by crossrefer vpc in above stack using cloudformation**
cloudform-ec2.yml  is used to create codepiple using cloudformations and it is referncing  SampleWebAppCrossStack.template 
execution command : ansible-playbook cloudform-ec2.yml

#aws-ssm-read.yml and aws-ssm-text.yml is working code for ssm parameter lookup

**#4sample ansible code to create pipeline using aws ssm parameter lookup.**
new-code-pipeline-cloudform2.yml is used to create codepiple using cloudformations and it is referncing  new-code-pipeline2.yml 

#5 sample ansible code for to deploy jinja template to deploy ec2.
#6 sample ansible code to deploy ec2 using assume role and cross account deployment
#7 sample ansible code to read inventory and create cloud formation stack for each changed hostfile parameter.
# adhoc practical
create new account using step functions.
Create EC2 Key Pairs
Create Security Groups
Create IAM Roles
deploy a custom IAM role:
Terminating Instances
Troubleshooting 
#### Validation tool

This tool allow to detect any issue above without deploy the pipeline. Allow you to get faster feedback from your configuration.

run `make validate`
Source failure in the AWS CodePipeline
Dynamic inventory creation using python script
Host inventory reading and create stack for ec2
