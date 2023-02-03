# AWSaC

AWS as code - better than landing zone or org-Formation

## Introduction
The AWSaC project is designing to be used as the first process taken after creating and activating a new AWS account.
(https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)

The AWS account activation must be complete before running the AWSaC project.

## Initialize a newly activated AWS account
The AWSaC tool will only work from an AWS account which is not a member account.
It is recommended to use the AWSaC tool on an unmodified, newly activated AWS account which has not had any further modifications or added resources.

To begin, log into the AWS consle with the account root user with the email address and password chosen during the AWS account creation.
(https://aws.amazon.com/)

Next, in the AWS console navigate to the root user security credentials page.
(https://console.aws.amazon.com/iam/home?#/security_credentials)

Create a new root access key and save the access key ID and secret access key in a secure temporary location on your local computer.

Execute the init-aws-org-root.yml workflow, replacing tmpID and tmpKey with the access key ID and secret access key created in the previous step:

```gh workflow run init-aws-org-root.yml -f AWS_ACCESS_KEY_ID=*** -f AWS_SECRET_ACCESS_KEY="***"```