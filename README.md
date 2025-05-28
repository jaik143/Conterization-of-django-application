
#  Containerization of Django Application with Docker

This project demonstrates how to containerize a Django web application using Docker. It includes all the necessary files to build and instructions to run the app inside a container.


## Install docker



```fffff
sudo apt update
sudo apt install docker.io -y
```
## Start Docker daemon
```bash
sudo systemctl status docker
sudo systemctl start docker
```
Grant Access to your user to run docker commands
## Grant Access to your user to run docker commands
```bash
sudo usermod -aG docker ubuntu
```
## Docker is Installed, up and running 
```bash
docker run hello-world
```
Output should look like:

```bash
....
....
Hello from Docker!
This message shows that your installation appears to be working correctly.
...
...
```
 
```

```
## Login to Docker [Create an account with https://hub.docker.com/]
```
docker login
```
```
Login with your Docker ID to push and pull images from Docker Hub. If you don't have a Docker ID, head over to https://hub.docker.com to create one.
Username: jaik468
Password:
WARNING! Your password will be stored unencrypted in /home/ubuntu/.docker/config.json.
Configure a credential helper to remove this warning. See
https://docs.docker.com/engine/reference/commandline/login/#credentials-store

Login Succeeded
```

## Now clone the repository 
```  
git clone https://github.com/jaik143/Conterization-of-django-application.git

cd Conterization-of-django-application/python-web-app

```
## Build the Docker Image
```
docker build -t django-app .
```
## Run the Docker Container
```
docker run -d -p 8000:8000 django-app
```
## Access the Application
```
http://<your-server-ip>:8000
```
## if your running locally please use 

```
http://localhost:8000
```


![Screenshot 2025-05-28 163749](https://github.com/user-attachments/assets/7e099517-a398-4de0-b1f3-2b6ef6a6bc4a)



