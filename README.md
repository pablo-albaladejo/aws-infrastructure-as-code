# udacity-aws-infrastructure-as-code
https://review.udacity.com/#!/rubrics/2556/view

#Network
./create.sh udagram-network network.yml network-parameters.json
./update.sh udagram-network network.yml network-parameters.json

#Servers
./create.sh udagram servers.yml servers-parameters.json
./update.sh udagram servers.yml servers-parameters.json8