# jfrog-artifactory

Get the 30 days free Trial License Key: \
https://jfrog.com/start-free/#hosted

Start artifactory:
```bash
docker run -d \
  -p 8081:8081 \
  -p 8082:8082 \
  --name artifactory \
  releases-docker.jfrog.io/jfrog/artifactory-pro
```
>  Use `releases-docker.jfrog.io/jfrog/artifactory-oss` docker image for Open Source version with limited features.

http://localhost:8082

ID: admin \
Pass: password


Debian Artifact | .
---|---
Distribution | focal
Component | main
Architecture | amd64



Remove artifactory:
```bash
docker rm -f artifactory
```
