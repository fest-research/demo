
## Demo
Simple demo application that represents the back-end of a web shop.
  
Running instance [here](http://35.187.21.121:8080/api/v1/proxy/namespaces/default/services/demo/)



### Deploy to Kubernetes

```shell
$ kubectl create -f https://raw.githubusercontent.com/fest-research/demo/master/assets/demo-deployment.yaml
```

### Build

First set the GOPATH environment variable see [https://golang.org/doc/code.html]

```shell

# install dependencies
go install

# build binaries
go build -o bin/demo
```

Run the binary with ./bin/demo


### Build Container

```shell

# build
docker build docker build -t my-demo .

# run
docker run --net=host my-demo

# push
docker push my-demo

```

### Travis

Travis CI: [https://travis-ci.org/fest-research/demo]

### REST API


```
# add message to backend
/push/<value> 

# clear all messages
/clear
```
