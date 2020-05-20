# Hello.go

Build only (dont run)
```
#Method 1
make build1
go build hello.go

#Method 2
make build2
go build
```

Build and Run
```
#Method 1
make run1
go build hello.go
./hello

#Method2
Hello, world
make run2
go run hello.go
Hello, world
```

Run test
```
#Method 1
make test1
go test hello.go hello_test.go
ok      command-line-arguments  (cached)

#Method 2
make test2
go test
PASS
ok      _/home/ritesh/go_learn/hello    0.002s
```

General use (Method 1)
```
make
go build hello.go
./hello

Hello, world
make test
go test hello.go hello_test.go
ok      command-line-arguments  (cached)
```

Clean
```
#Method 1
make clean1
rm -f ./hello

#Method 1
make clean2
go clean
```
