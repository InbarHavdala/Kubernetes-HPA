Instructions
clone repo

git clone https://github.com/InbarHavdala/nodejs-sample-app-kubernetes.git
cd nodejs-sample-app-kubernetes/node_app
Build docker image

sudo docker build -t nodejs-v1 .
Verify app locally by running container

docker run -d --name <SOMENAME> -p 8080:3000 nodejs-v1:latest
Note: nodejs-v1:latest image has been pushed to dockerhub as well and its publically available. (docker pull tarun/nodejs-v1)


http://localhost:8080

http://localhost:8080/version
