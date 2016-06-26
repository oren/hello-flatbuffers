# Tutorial: Use FlatBuffers in Go

The code for https://rwinslow.com/posts/use-flatbuffers-in-golang/

## Install the FlatBuffers compiler (Linux)

For other OSX/Windows [go here](https://rwinslow.com/posts/how-to-install-flatbuffers/).

```
git clone https://github.com/google/flatbuffers.git
cd flatbuffers
cmake -G "Unix Makefiles"
make
./flattests
sudo cp flatc /usr/local/bin/
```

## Install the FlatBuffers Go runtime library

```
GOPATH=$(pwd) go get github.com/google/flatbuffers/go
```

# Run

```
GOPATH=$(pwd) go run main.go
```

# Test

```
GOPATH=$(pwd) go test -test.bench .
```
