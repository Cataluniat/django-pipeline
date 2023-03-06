Django Pipeline

## Setup Secrets
```sh 
DOCKER_USERNAME
DOCKER_PASSWORD
HOST = ssh host
USERNAME = ssh username
KEY ssh private key
```
## Setup Secrets
Edit `.github/workflow/push.yml`

```sh 
image: docker-user/docker-repo
```

## Deploy
```sh
./deploy.sh
```

### SSH login in instance
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
