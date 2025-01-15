## This is step by step running spring boot application

# Test build using maven
`mvn clean package`

# start minikube cluster
`minikube start`

# run jenkins using docker port 8080
`docker run -d --name jenkins -p 8080:8080 -p 50000:50000 -v /var/run/docker.sock:/var/run/docker.sock -v $(which docker):/usr/bin/docker -v /home/jenkins_home:/var/jenkins_home --network minikube jenkins/jenkins:lts`

# Test Apps in local
_*syntax*_:
```
docker build -t spring-boot-hello-world .
```