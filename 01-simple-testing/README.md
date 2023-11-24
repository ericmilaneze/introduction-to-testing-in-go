# Simple Testing

## Running the program
`go run .`

---

## Testing it
`go test -v .`

### Running a single test
- `go test -v -run Test_isPrime`
- `go test -v -run ^Test_isPrime$`

### Running groups of tests (test suites)
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

---
