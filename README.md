# docker-howto-update-curl-utility
This article describes about how to install curl utility in running container

Step1 : Create docker centos container in interactive terminal mode.

```
docker container run --rm -it centos:7 bash

The above docker command prompts the bash shell then enter the following command

yum update curl

curl --version 

```

Step2 : Open the another terminal Crate the one more docker container.

```
docker container run --rm -it ubuntu:04 bash

Then enter the below command to 
apt-get update && apt-get install -y curl

curl --version 
```

Step 3: Verify the docker containers are running or not.

```
In Previous steps two containers are running in interactive terminal mode .Once we exit the terminal 
containers are not longer running

Start the both containers .Now we both the containers having the curl working 
```

