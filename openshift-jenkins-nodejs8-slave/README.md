1. Create image
```
$ docker build -t openshift-jenkins-nodejs8-slave .
```
2. List images
```
$ docker image ls
```
3. Publish Image
```
$ docker login -u allenhwkim
Password:
Login Succeeded
$ docker tag <image-id> allenhwkim/openshift-jenkins-nodejs8-slave:latest
$ docker push allenhwkim/openshift-jenkins-nodejs8-slave
```
