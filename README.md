https://www.krakend.io/?

https://hub.docker.com/r/devopsfaith/krakend

## check
docker run -it -p 8080:8080 -v $PWD:/etc/krakend/ devopsfaith/krakend check --config krakend.json


## debug
docker run -p 8080:8080 -v "${PWD}:/etc/krakend/" devopsfaith/krakend run -d -c /etc/krakend/krakend.json


## health
curl HTTP://localhost:8080/__health



https://github.com/krakend/playground-community