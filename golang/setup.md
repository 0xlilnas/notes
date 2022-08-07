# Setup

## How to clean up your go workspace

1.Open your terminal and type the command below:

```go
go env
```

2.In your terminal,there is a `GOMODCACHE` which show your pkg location in your local machine

3.`cd` into the path `/home/{username}/go/pkg/` and run

```go
go clean -modcache
```

4.`ls` in the path and check there is only one file left which is `sumdb`.Remove the file typing the command below

```go
rm -rf sumdb
```

5.Make new directory for your new project and initialize it with:

```go
mkdir new-project
go mod init github/{username}/new-project
```

6.Create `main.go` file and try add any 3rd party package and then run:

```go
go mod tidy
```

this command will download the package by finding it based on your import.
