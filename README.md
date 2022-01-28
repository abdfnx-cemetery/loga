# Loga

> Simple Golang logger.

```bash
# syntax
[LOG-LEVEL] [DATE] or [TIME] [FILE:LINE] [MESSAGE]

[error] 2019/05/08 20:04:57 file.go:141: error shows timestamp and line info
[warn]  2019/05/08 20:04:57 warn shows timestamp
[debug] 20:04:57 file.go:129: debug shows regular timestamp and line info
```

## Installation

```bash
go get github.com/abdfnx/loga
```

## Usage

```go
package main

import (
    "github.com/abdfnx/loga"
)

func main() {
    loga.Debug("debug message")
    loga.Info("info message")
    loga.Warn("warn message")
    loga.Error("error message")
}
```

## Log Levels

* debug
* trace
* info
* warn
* error
