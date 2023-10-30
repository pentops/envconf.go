Env Conf
========

Environment Variable config loader for go

## Simple Usage

```

import "github.com/pentops/envconf.go/envconf"

var config struct {
	Bind string `env:"BIND" default:":8080"`
}

func main() {
	if err := envconf.Parse(&config); err != nil {
		log.Fatal(err.Error())
	}
}
```
