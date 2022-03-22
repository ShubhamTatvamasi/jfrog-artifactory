# jfrog-artifactory

Start artifactory:
```bash
docker run -d \
  -p 8081:8081 \
  -p 8082:8082 \
  --name artifactory \
  releases-docker.jfrog.io/jfrog/artifactory-oss
```

Stop artifactory:
```bash
docker rm -f artifactory
```

http://localhost:8081

ID: admin \
Pass: password \
New Pass: Password1
