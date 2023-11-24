# Introduction to Testing in Go (Golang)

This repo was created to add the files created while learning from the [Introduction to Testing in Go (Golang)](https://www.udemy.com/course/introduction-to-testing-in-go-golang) course.

## Applications

- [Simple testing](./01-simple-testing)
- [Testing web applications](./02-testing-web-applications/)

---

## Testing

### Run all the tests
`go test -v ./...`

### Run a single test
- `go test -v -run Test_isPrime`
- `go test -v -run ^Test_isPrime$`

### Run groups of tests (test suites)
- `go test -v -run Test_alpha`
- `go test -v -run ^Test_alpha.*$`

---

## Code coverage
### Show on the Terminal
`go test -cover .`

### Show on the Browser
```
go test -coverprofile=coverage.out
go tool cover -html=coverage.out
```