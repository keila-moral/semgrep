## Quickstart guide using Docker

Initialise Docker

```
open -a Docker
```

Test the local Semgrep Docker image is actually responsive:

```
docker run -it -v "${PWD}:/src" semgrep-local semgrep
```

After implementing the new changes, build the Docker image again:

```
docker build --target semgrep-oss -t semgrep-local . 
``` 
