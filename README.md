# AWSaC

AWS as code - better than landing zone or org-Formation

## init aws org root account
Init the AWS org root account by triggering the init-aws-org-root.yml workflow.
gh workflow run init-aws-org-root.yml -f AWS_ACCESS_KEY_ID=scully -f AWS_SECRET_ACCESS_KEY=hello