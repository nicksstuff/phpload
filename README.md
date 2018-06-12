# Docker Load Example

from here: https://kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale-walkthrough/

This project contains a simple application that generates load.


## Build Docker Images

```bash

sudo rm -r phpload/
git clone https://github.com/niklaushirt/phpload.git
cd phpload/
docker build -t phpload:1.0.0 docker

docker run --rm -p 9080:9080 phpload:1.0.0
```

## Add HELM repository

```
https://raw.githubusercontent.com/niklaushirt/phpload/master/charts/stable/repo/stable/
```
