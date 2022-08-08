
# Laravel Deploy

Github Action to deploy laravel on stagging or production server




## Generate SSH-Keygen
Menyiapkan private key dan public key di server
```bash
ssh-keygen -t rsa -f ci-laravel
cat ci-laravel.pub >> ~/.ssh/authorized_keys
```

## Installation
PRIVATE_KEY didapat dengan
```
cat ci-laravel
```

    
## Environment Variables

To run this project, you will need to add the following environment variables to your **secrets**

`PRODUCTION_PASSWORD`

`PRODUCTION_SSH_HOST`

`PRODUCTION_SSH_USERNAME`

`STAGGING_DOMAIN_NAME`

`STAGGING_SSH_HOST`

`STAGGING_SSH_PRIVATE_KEY`

`STAGGING_SSH_USERNAME`

## Commands

### Release Production
commit repository with message :
```
release-production: vX.XX.XXX
```
### Release Stagging
commit repository with message :
```
release-stagging: vX.XX.XXX
```

replace **vX.XX.XXX** with ur **VERSION**


