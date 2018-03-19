# goldfish-docker
Plain and simple goldfish Docker image

Note that this image does NOT contain a goldfish config file.
You need to provide one, for example using volume mount:
```bash
docker run -d -v $PWD/config.hcl:/app/config.hcl --cap-add IPC_LOCK gold1 -config=config.hcl
```
