# Installing golang compiler in linux machine

Download the Go 1.12.1 binary archive suitable for your operating system from the official Go website ([https://golang.org/dl/](https://golang.org/dl/)).

```bash
wget https://dl.google.com/go/go1.12.1.linux-amd64.tar.gz
```

Extract the downloaded archive to the /usr/local directory:

```bash
sudo tar -C /usr/local -xzf go1.12.1.linux-amd64.tar.gz
```

Add the Go binary directory to your system's PATH environment variable by editing your shell profile file (e.g. ~/.bashrc or ~/.zshrc) and adding the following lines:

```ruby
export PATH=$PATH:/usr/local/go/bin
```

Reload your shell profile to apply the changes:

```bash
source ~/.bashrc
```

```bash
go version
```

**output:**

go version go1.12.1 linux/amd64


###### lets print HelloWorld! from go

```go
package main

import "fmt"

func main() {
	fmt.Printf("HelloWorld!")
}

```

**Output:** 

HelloWorld!
