# DEVOPS-DOCKER
DEVOPS DOCKER DRILL EXERCISE <br>
sudo docker build -t exe-img . <br>
sudo docker run -d -p 8080:80 exe-img <br>
sudo docker run -d -p 8082:80 -e web=website2 exe-img
