all: run1

#############################################
clean: clean2
clean1:
	rm -f ./hello

clean2:
	go clean

#############################################
build:  build2
build1: hello.go
	go build hello.go

build2: hello.go
	go build

run: run2
run1: build1
	./hello

run2: hello.go
	go run hello.go

debug: debug1
debug1: build1
	gdb ./hello

debug2: build1
	/home/http/go_workspace/bin/dlv exec ./hello --check-go-version=false

#############################################
test:test2
test1: hello.go hello_test.go
	go test hello.go hello_test.go

test2: hello.go hello_test.go
	go test

build_test: hello.go hello_test.go
	go test -c

test3: build_test
	./hello.test

debug_test: debug_test1
debug_test1: build_test
	gdb ./hello.test

debug_test2: build_test
	/home/http/go_workspace/bin/dlv exec ./hello.test --check-go-version=false
