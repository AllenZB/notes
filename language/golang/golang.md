# GoLang

## Build

```bash
env GOOS=linux GOARCH=amd64 go build $FILEPATH
```

## Basic

1. [Package](./package.md)
    - init & main
    - Execution Flow
1. [Slices](./slices.md)
    - Array vs Slice
    - Length & Capacity
    - Init, append and loop over
1. [Map](./map)
1. [Interface](./interface.md)

## Basic Questions

1. [String vs String Pointers](https://dhdersch.github.io/golang/2016/01/23/golang-when-to-use-string-pointers.html)

## Advanced

1. [Profiling with pprof](./pprof.md)
    - go-torch
1. [Go Routine](./goroutine.md)
1. [Mutex](./mutex.md)
1. [Reflection](./reflection.md)
1. [Embedding in Go](./embedding.md)

## Testing

- Fail vs Errorf vs Fatalf
- table of tests: slice of struct
  - Add name to tests
  - Sub Tests
- http handler test
  - http.NewRecorder(); rec.Result()
  - defer res.Body.Close()
  - ioutil.ReadAll(res.body())

## Blog/Tutorials

1. [Singleton Pattern in Go](http://marcio.io/2015/07/singleton-pattern-in-go/)
    - Check-Lock-Check Pattern
    - `sync.Once`
    - [Double-checked locking: Clever, but broken](https://www.javaworld.com/article/2074979/java-concurrency/double-checked-locking--clever--but-broken.html)
2. Just For Func #1: A Code Review
    1. Do not capitalize error codes.
    2. resp.Status vs resp.StatusCode.
    3. Close channels to avoid goroutine leak.