# docker-azure-template

## Description
This is a template to create a simple dockerized Nodejs "Hello world" server to azure web apps as a single container app.

## Prerequisites
- existing azure subscription
- az cli installed
- docker installed and running
- terraform installed

## Usage
1. Create a new project from this template
2. Run `az login`
3. In terraform directory rename the "terraform.tfvars.example" file to "terraform.tfvars" and fill in the correct variable values.
4. Cd into terraform directory and run `terraform init && terraform plan`
5. If everything looks fine run `terraform apply`
6. In Azure Portal go to your newly created app
7. Go to "Deployment Center" (left panel), fill in the the desired values and click "save"

Now, if you chose, for example, github actions as source, you can go to your github repo and see that the necessary secrets and github actions are automatically set and build and deploy is in process.
