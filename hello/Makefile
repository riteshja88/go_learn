all: run1

clean1:
	rm -f ./hello

clean2:
	go clean

build1: hello.go
	go build hello.go

build2: hello.go
	go build

run1: build1
	./hello

run2: hello.go
	go run hello.go

test1: hello.go hello_test.go
	go test hello.go hello_test.go

test2: hello.go hello_test.go
	go test

test: test1
