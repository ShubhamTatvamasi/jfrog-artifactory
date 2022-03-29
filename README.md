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

### Debian Artifact

Property | Value
---|---
Distribution | focal
Component | main
Architecture | amd64

---

### Repo

Add public GPG key to ubuntu:
```bash
curl -fsSL https://artifactory.shubhamtatvamasi.com/artifactory/api/security/keypair/artifactory-gpg/public | \
  sudo gpg --dearmor -o /usr/share/keyrings/artifactory-shubhamtatvamasi-keyring.gpg
```

Add repo link:
```bash
sudo echo "deb [arch=amd64 signed-by=/usr/share/keyrings/artifactory-shubhamtatvamasi-keyring.gpg] \
  https://artifactory.shubhamtatvamasi.com/artifactory/ubuntu/ \
  focal main" > /etc/apt/sources.list.d/artifactory.shubhamtatvamasi.list
```


### Uninstall

Remove artifactory:
```bash
docker rm -f artifactory
```
