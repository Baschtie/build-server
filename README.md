# Jenkins behind a reverse proxy in docker

### Setup
These environment variables need to be set:
```
DEFAULT_HOST
JENKINS_HOST
```

You need you certs in the folder nginx/certs/
if you used certbot to optain some you will find these in /etc/letsencrypt/live/domain.tld-001/privkey.pem & /etc/letsencrypt/live/domain.tld/fullchain.pem

_copy_ them & rename them as follows
```
fullchain.pem --> jenkins.domain.tld.crt
```

```
privkey.pem --> jenkins.domain.tld.key
```
