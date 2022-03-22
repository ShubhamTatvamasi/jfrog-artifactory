# jfrog-artifactory

Get the Trial License Key: \
https://jfrog.com/start-free/#hosted

Start artifactory:
```bash
docker run -d \
  -p 8081:8081 \
  -p 8082:8082 \
  --name artifactory \
  releases-docker.jfrog.io/jfrog/artifactory-pro
  # releases-docker.jfrog.io/jfrog/artifactory-oss # Open Source image (limited features)
```

http://localhost:8082

ID: admin \
Pass: password \
New Pass: Password1

Remove artifactory:
```bash
docker rm -f artifactory
```
