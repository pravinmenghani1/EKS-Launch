# EKS-Launch
This section outlines how to set up the environment to run the labs in your own AWS account.

The first step is to create an IDE with the provided CloudFormation template. The easiest way to do this is using the quick launch links below:

Region	Link
us-west2	Launch
eu-west-1	Launch
ap-southeast-1	Launch
tip
These instructions have been tested in the AWS regions listed above and are not guaranteed to work in others without modification.

Scroll to the bottom of the screen and acknowledge the IAM notice:

acknowledge IAM

Then click the Create stack button:

Create Stack

The CloudFormation stack will take roughly 5 minutes to deploy, and once completed you can retrieve the URL for the Cloud9 IDE from the Outputs tab:

cloudformation outputs

Open this URL in a web browser to access the IDE.

cloud9-splash

You can now close CloudShell, all further commands will be run in the terminal section at the bottom of the Cloud9 IDE. The AWS CLI is already installed and will assume the credentials attached to the Cloud9 IDE:

~
$
aws sts get-caller-identity
The next step is to create an EKS cluster to perform the lab exercises in. Please follow one of the guides below to provision a cluster that meets the requirements for these labs:

(Recommended) eksctl
Terraform
(Coming soon!) CDK
