Django Pipeline

Secrets
DOCKER_USERNAME
DOCKER_PASSWORD
HOST = ssh host
USERNAME = ssh username
KEY ssh private key

Edit `.github/workflow/push.yml`

image: docker-user/docker-repo


## Deploy infrastructure
```sh
./deploy.sh
```

### Connecting to your Linux instance using SSH
```sh
ssh -i ./tf/private/key_access.pem -A ubuntu@[instance IP]
```

## Destroy infrastructure
```sh
./down.sh
```

## Deploy CI/CD
On main branch...
```sh
git push
```
