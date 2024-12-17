# Uninitialized Integer Variable in Go

This repository demonstrates a common error in Go: using uninitialized integer variables.  Go's default zero value for integers might not always be the intended starting value, leading to subtle bugs.

The `bug.go` file shows the problem. The integer variable `i` is not explicitly initialized; therefore it defaults to 0. However, this default value might not be obvious to all developers, which could lead to unexpected behavior. 

The `bugSolution.go` shows how to fix this by initializing the variable explicitly.

## How to reproduce

1. Clone this repository.
2. Run `go run bug.go` to see the unintended behavior.
3. Run `go run bugSolution.go` to see the corrected version.
