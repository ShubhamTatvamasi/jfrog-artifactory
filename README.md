# jfrog-artifactory

Start artifactory:
```bash
docker run -d \
  --name artifactory \
  -p 8081:8081 \
  -p 8082:8082 \
  releases-docker.jfrog.io/jfrog/artifactory-oss
```
