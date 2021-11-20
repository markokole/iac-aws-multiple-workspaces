# Working with Terraform workspace

There are three workspaces:

- dev
- test
- prod

## Start the container

```bash
docker run -itd --name aws-workspace --env-file "aws/credentials" --volume $PWD/terraform:/local-git markokole/terraformer:1.0.3
```

## Step into container

```bash
docker exec -it aws-workspace /bin/sh
```
