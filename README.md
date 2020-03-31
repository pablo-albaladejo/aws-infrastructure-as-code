https://review.udacity.com/#!/rubrics/2556/view

# Network
`./create.sh AWS-IaC-Network ./network/infra.yml ./network/parameters.json`

`./update.sh AWS-IaC-Network ./network/infra.yml ./network/parameters.json`

`./delete.sh AWS-IaC-Network`

# Servers
`./create.sh AWS-IaC-Servers ./servers/infra.yml ./servers/parameters.json`

`./update.sh AWS-IaC-Servers ./servers/infra.yml ./servers/parameters.json`

`./delete.sh AWS-IaC-Servers`

# Bastion
`./create.sh AWS-IaC-Bastion ./bastion/infra.yml ./bastion/parameters.json`

`./update.sh AWS-IaC-Bastion ./bastion/infra.yml ./bastion/parameters.json`

`./delete.sh AWS-IaC-Bastion`

# ssh
`chmod 400 ./AWS-IaC-BastionHost.pem`

`scp -i ./AWS-IaC-BastionHost.pem ./AWS-IaC-WebServer.pem ubuntu@<bastion-public-ip>:/home/ubuntu`

`ssh -i ./AWS-IaC-BastionHost.pem ubuntu@<bastion-public-ip>`

`ssh i ./AWS-IaC-WebServer.pem ubuntu@<server-private-ip>`
