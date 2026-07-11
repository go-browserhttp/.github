<p align="center"><img src="https://raw.githubusercontent.com/go-browserhttp/brand/main/social/go-browserhttp.png" alt="go-browserhttp" width="720"></p>

<h1 align="center">go-browserhttp</h1>
<p align="center">A pure-Go http.Client with a Chrome TLS fingerprint (uTLS) — bypass anti-bot 403s, no host web view.</p>
<p align="center">[![docs](https://img.shields.io/badge/docs-mkdocs--material-0A6E96?style=flat-square&logo=materialformkdocs&logoColor=white)](https://go-browserhttp.github.io/docs/) ![repos](https://img.shields.io/badge/repos-1-0079A8?style=flat-square) ![Go](https://img.shields.io/badge/Go-1.26-00ADD8?style=flat-square&logo=go&logoColor=white) ![license](https://img.shields.io/badge/license-BSD--3--Clause-0A6E96?style=flat-square)</p>

---

## What is this?

`go-browserhttp` is a pure-Go (**CGO=0**) `http.Client` that presents a real **Chrome TLS fingerprint** via [uTLS](https://github.com/refraction-networking/utls). Many sites 403 non-browser clients based largely on the TLS ClientHello; mimicking Chrome's ciphers/extensions/curves — plus a browser User-Agent and a warmed cookie jar — lets a plain Go client reach public endpoints with **no host web view**. Identical on macOS, Linux and Windows.

```go
c := browserhttp.NewClient(30 * time.Second)
resp, err := c.Get("https://www.reddit.com/r/golang/hot.json")
```

Extracted from `go-news-reader/reader`; shared by any fetcher that must look like a browser.

## Repositories (1)

| Module | Kind | What it is | API |
|---|---|---|:--:|
| [`browserhttp`](https://github.com/go-browserhttp/browserhttp) | client | Pure-Go `http.Client` presenting a Chrome TLS fingerprint via uTLS. CGO=0. | [ref](https://pkg.go.dev/github.com/go-browserhttp/browserhttp) |

> This list reflects the repos that actually exist in the org.

## Links

- 📖 Docs — <https://go-browserhttp.github.io/docs/>
- 🌐 Site — <https://go-browserhttp.github.io/>
- 🎨 Brand assets — <https://github.com/go-browserhttp/brand>

---
<p align="center"><sub>Branding in <a href="https://github.com/go-browserhttp/brand">go-browserhttp/brand</a>.</sub></p>
