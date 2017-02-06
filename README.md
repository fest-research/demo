
## Demo
Simple demo application that represents the back-end of a web shop.
  



### Deploy to Kubernetes

```shell
$ https://raw.githubusercontent.com/fest-research/demo/master/assets/demo-deployment.yaml
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