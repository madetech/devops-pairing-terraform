# devops-pairing-terraform
Create a temporary user for use in devops pairing interviews

**We do not expect the interviewee to use this project**

## How to use
1. Clone this repo
2. Ensure [aws-vault](https://github.com/madetech/handbook/blob/main/guides/cloud/aws_sandbox.md#cli-usage-1) is installed
3. Ensure [tfenv](https://github.com/tfutils/tfenv) is installed
4. Run `terraform init`
5. Run `aws-vault exec mt-devops -- terraform apply` in the DevOps pairing account (the regular sandbox playground account will not work for this)
6. Enter the first name of the interviewee when prompted
7. Don't forget to run `aws-vault exec mt-devops -- terraform destroy` after the candidate has destroyed what they have made

## Credits
Based of https://github.com/cob16/terraform-learning/tree/master/pairing
