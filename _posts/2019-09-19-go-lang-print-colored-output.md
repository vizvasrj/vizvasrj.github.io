# GO lang to print colored output

```go
package main

import (
	"fmt"
)

func Red(format string, args ...interface{}) {
	fmt.Printf("\033[31m"+format+"\033[0m", args...)
}

func Green(format string, args ...interface{}) {
	fmt.Printf("\033[32m"+format+"\033[0m", args...)
}

func Yellow(format string, args ...interface{}) {
	fmt.Printf("\033[33m"+format+"\033[0m", args...)
}

func Blue(format string, args ...interface{}) {
	fmt.Printf("\033[34m"+format+"\033[0m", args...)
}

func Magenta(format string, args ...interface{}) {
	fmt.Printf("\033[35m"+format+"\033[0m", args...)
}

func Cyan(format string, args ...interface{}) {
	fmt.Printf("\033[36m"+format+"\033[0m", args...)
}

func main() {
	// Set the foreground color to red
	Red("Hello, world!\n")
	Yellow("Hello, world!\n")
	Green("Hello, world!\n")
	Magenta("Hello, world!\n")
	Cyan("Hello, world!\n")
	Blue("Hello, world!\n")

}

```
