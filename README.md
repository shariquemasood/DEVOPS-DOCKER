# DEVOPS-DOCKER
DEVOPS DOCKER DRILL EXERCISE
sudo docker build -t exe-img .
sudo docker run -d -p 8080:80 exe-img
sudo docker run -d -p 8082:80 -e web=website2 exe-img
