# wordpress-docker-compose
First ssh into the instance and update the machine using 
## sudo apt-get update
# Install docker
## sudo apt-get install docker.io
As the docker-compose tool is not inbuilt in docker, install the ### docker-compose
## sudo curl -L "https://github.com/docker/compose/releases/download/1.24.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
## sudo chmod +x /usr/local/bin/docker-compose
## docker-compose --version
# Create YAML file
## mkdir wordpress
## cd wordpress
## sudo nano docker-compose.yaml
copy the file from docker-compose.yaml and paste on sublime text and paste it in the docker-compose.yaml file.
save the file.
To build docker-compose file use 
## sudo docker-compose up -d
After sucessful execution go to browser and paste the ip address of instance and in yaml file we have mentioned port number 8000 so you need to use:
## master-ip-address:8000
You will get the wordpress installation page. thus, your deployment of wordpress using dockercompose file is done sucessfully. 
