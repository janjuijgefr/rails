# **parallax-core**

![Go](https://img.shields.io/badge/go-1.22-blue)
![Redis](https://img.shields.io/badge/cache-redis-red)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

high-throughput async task processor for distributed Go services.

---

```bash
go install github.com/parallax/core@latest
```

### usage

```go
import "github.com/parallax/core"

task := parallax.New("email:send", payload)
parallax.Enqueue(task)
```

### features

* automatic deduplication
* configurable retry policies
* prometheus metrics `/metrics`
* redis + postgres backends

### roadmap

* [ ] kafka integration
* [ ] distributed tracing

MIT © [parallax.dev](https://parallax.dev)
