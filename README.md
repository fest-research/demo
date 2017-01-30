
go install
cp $GOPATH/bin/demo ./bin

docker build docker build -t fest/demo .
docker push fest/demo
