# ✨ Awesome Fiber [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Discord](https://img.shields.io/badge/discord-join%20channel-7289DA)](https://gofiber.io/discord)

<a href="https://gofiber.io">
  <img src="https://raw.githubusercontent.com/gofiber/docs/master/static/fiber_v2_logo.svg" alt="Fiber Logo" align="left" style="margin-right: 25px" height=150>
</a>

> **Fiber** is an [Express](https://github.com/expressjs/express) inspired **web framework** built on top of [Fasthttp](https://github.com/valyala/fasthttp), the **fastest** HTTP engine for [Go](https://golang.org/doc/). Designed to **ease** things up for **fast** development with **zero memory allocation** and **performance** in mind.

A curated list of awesome Fiber middlewares, boilerplates, recipes, articles and tools.
<br>

## Contents
- [⚙️ Middlewares](#%EF%B8%8F-middlewares)
  - [🧬 Core](#-core)
  - [🔗 External](#-external)
  - [💻 Contrib](#-contrib)
  - [🌱 Third Party](#-third-party)
- [🚧 Boilerplates](#-boilerplates)
- [📁 Recipes](#-recipes)
- [🛠️ Tools](#%EF%B8%8F-tools)
- [📖 Articles](#-articles)
- [🤖 Benchmarks](#-benchmarks)

## ⚙️ Middlewares
Where to discover Fiber middlewares.

### 🧬 Core
List of middlewares that are included within the Fiber framework.
- [BasicAuth](https://github.com/gofiber/fiber/tree/master/middleware/basicauth) - Basic auth middleware provides an HTTP basic authentication. It calls the next handler for valid credentials and 401 Unauthorized for missing or invalid credentials.
- [Cache](https://github.com/gofiber/fiber/tree/master/middleware/cache) - Intercept and cache responses.
- [Compress](https://github.com/gofiber/fiber/tree/master/middleware/compress) - 	Compression middleware for Fiber, it supports `deflate`, `gzip` and `brotli` by default.
- [CORS](https://github.com/gofiber/fiber/tree/master/middleware/cors) - Enable cross-origin resource sharing (CORS) with various options.
- [CSRF](https://github.com/gofiber/fiber/tree/master/middleware/csrf) - Protect from CSRF exploits.
- [Encrypt Cookie](https://github.com/gofiber/fiber/tree/master/middleware/encryptcookie) - Encrypt middleware which encrypts cookie values.
- [ETag](https://github.com/gofiber/fiber/tree/master/middleware/etag) - ETag middleware that lets caches be more efficient and save bandwidth, as a web server does not need to resend a full response if the content has not changed.
- [Expvar](https://github.com/gofiber/fiber/tree/master/middleware/expvar) - Expvar middleware that serves via its HTTP server runtime exposed variants in the JSON format.
- [Favicon](https://github.com/gofiber/fiber/tree/master/middleware/favicon) - Ignore favicon from logs or serve from memory if a file path is provided.
- [FileSystem](https://github.com/gofiber/fiber/tree/master/middleware/filesystem) - FileSystem middleware for Fiber, special thanks and credits to Alireza Salary.
- [Limiter](https://github.com/gofiber/fiber/tree/master/middleware/limiter) - Rate-limiting middleware. Use to limit repeated requests to public APIs and/or endpoints such as password reset.
- [Logger](https://github.com/gofiber/fiber/tree/master/middleware/logger) - HTTP request/response logger.
- [Monitor](https://github.com/gofiber/fiber/tree/master/middleware/monitor) - Monitor middleware that reports server metrics, inspired by express-status-monitor.
- [Pprof](https://github.com/gofiber/fiber/tree/master/middleware/pprof) - Pprof middleware that serves via its HTTP server runtime profiling data in the format expected by the pprof visualization tool.
- [Proxy](https://github.com/gofiber/fiber/tree/master/middleware/proxy) - Allows you to proxy requests to a multiple servers.
- [Recover](https://github.com/gofiber/fiber/tree/master/middleware/recover) - Recover middleware recovers from panics anywhere in the stack chain and handles the control to the centralized ErrorHandler.
- [RequestID](https://github.com/gofiber/fiber/tree/master/middleware/requestid) - Adds a requestid to every request.
- [Session](https://github.com/gofiber/fiber/tree/master/middleware/session) - Session middleware. NOTE: This middleware uses our Storage package.
- [Skip](https://github.com/gofiber/fiber/tree/master/middleware/skip) - Skip middleware that skips a wrapped handler is a predicate is true.
- [Timeout](https://github.com/gofiber/fiber/tree/master/middleware/timeout) - Adds a max time for a request and forwards to ErrorHandler if it is exceeded.

### 🔗 External
List of externally hosted middleware modules and maintained by the [Fiber team](https://github.com/orgs/gofiber/people).
- [adaptor](https://github.com/gofiber/adaptor) - Converter for net/http handlers to/from Fiber request handlers.
- [helmet](https://github.com/gofiber/helmet) - Helps secure your apps by setting various HTTP headers.
- [jwt](https://github.com/gofiber/jwt) - JWT returns a JSON Web Token (JWT) auth middleware.
- [keyauth](https://github.com/gofiber/keyauth) - Key auth middleware provides a key based authentication.
- [redirect](https://github.com/gofiber/redirect) - Redirect middleware for Fiber.
- [rewrite](https://github.com/gofiber/rewrite) - Rewrite middleware rewrites the URL path based on provided rules. It can be helpful for backward compatibility or just creating cleaner and more descriptive links.
- [storage](https://github.com/gofiber/storage) - Premade storage drivers that implement the Storage interface, designed to be used with various Fiber middlewares.
- [template](https://github.com/gofiber/template) - This package contains 8 template engines that can be used with Fiber v1.10.x Go version 1.13 or higher is required.
- [websocket](https://github.com/gofiber/websocket) - Based on Fasthttp WebSocket for Fiber with Locals support!

### ‍💻 Contrib
List of third party middlewares and maintained by the Fiber team and community.
- [fibersentry](https://github.com/gofiber/contrib/tree/main/fibersentry) - Sentry support for Fiber.
- [fiberzap](https://github.com/gofiber/contrib/tree/main/fiberzap) - Zap logging support for Fiber.
- [otelfiber](https://github.com/gofiber/contrib/tree/main/otelfiber) - OpenTelemetry support for Fiber.
- [paseto](https://github.com/gofiber/contrib/tree/main/paseto) - PASETO returns a Web Token (PASETO) auth middleware.
- [swagger](https://github.com/gofiber/contrib/tree/main/swagger) - Swagger middleware for Fiber. The middleware handles Swagger UI.

### 🌱 Third Party
List of middlewares that are created by the Fiber community. **(WIP)**
- [arsmn/fiber-swagger](https://github.com/arsmn/fiber-swagger)
- [arsmn/fiber-casbin](https://github.com/arsmn/fiber-casbin)
- [arsmn/fiber-introspect](https://github.com/arsmn/fiber-introspect)
- [shareed2k/fiber_tracing](https://github.com/shareed2k/fiber_tracing)
- [shareed2k/fiber_limiter](https://github.com/shareed2k/fiber_limiter)
- [arsmn/gqlgen](https://github.com/arsmn/gqlgen)
- [kiyonlin/fiber_limiter](https://github.com/kiyonlin/fiber_limiter)
- [juandiii/go-jwk-security](https://github.com/juandiii/go-jwk-security)
- [ansrivas/fiberprometheus](https://github.com/ansrivas/fiberprometheus)
- [LdDl/fiber-long-poll](https://github.com/LdDl/fiber-long-poll)
- [K0enM/fiber_vhost](https://github.com/K0enM/fiber_vhost)
- [sacsand/gofiber-firebaseauth](https://github.com/sacsand/gofiber-firebaseauth)
- [theArtechnology/fiber-inertia](https://github.com/theArtechnology/fiber-inertia)
- [aschenmaker/fiber-health-check](https://github.com/aschenmaker/fiber-health-check)
- [elastic/apmfiber](https://github.com/elastic/apm-agent-go/tree/master/module/apmfiber)
- [eozer/fiber_ldapauth](https://github.com/eozer/fiber_ldapauth)


## 🚧 Boilerplates
Premade boilerplates for Fiber. **(WIP)**
- [gofiber/boilerplate](https://github.com/gofiber/boilerplate)
- [fiber-boilerplate](https://github.com/thomasvvugt/fiber-boilerplate)
- [sujit-baniya/fiber-boilerplate](https://github.com/sujit-baniya/fiber-boilerplate)
- [create-go-app/fiber-go-template](https://github.com/create-go-app/fiber-go-template)
- [embedmode/fiberseed](https://github.com/embedmode/fiberseed)


## 📁 Recipes
Recipes for Fiber. **(WIP)**
- [gofiber/recipes](https://github.com/gofiber/recipes) - Official Fiber cookbook.
- https://github.com/kiyonlin/fiblar-demo
- https://github.com/koddr/tutorial-go-fiber-rest-api
- https://github.com/firebase007/go-rest-api-with-fiber
- https://github.com/embedmode/fiberseed
- https://github.com/chawk/go_fiber_quickstart
- https://github.com/EricLau1/go-fiber-auth-api

## 🛠️ Tools
Several tools to make Fiber usage easier. **(WIP)**
- [gofiber/cli](https://github.com/gofiber/cli) - Fiber Command Line Interface.
- [go-dawn/dawn](https://github.com/go-dawn/dawn) - Dawn is an opinionated web framework that provides rapid development capabilities which on top of Fiber.
- [tompston/gomakeme](https://github.com/tompston/gomakeme) - Generate boilerplate + endpoints for Fiber or Gin REST APIs.

## 📖 Articles
Articles about Fiber written by the community.

- [Working with middlewares and boilerplates](https://dev.to/koddr/go-fiber-by-examples-working-with-middlewares-and-boilerplates-3p0m)
- [Testing the application](https://dev.to/koddr/go-fiber-by-examples-testing-the-application-1ldf)
- [Delving into built-in functions](https://dev.to/koddr/go-fiber-by-examples-delving-into-built-in-functions-1p3k)
- [Go Fiber by Examples: How can the Fiber Web Framework be useful?](https://dev.to/koddr/go-fiber-by-examples-how-can-the-fiber-web-framework-be-useful-487a)
- [Build a RESTful API on Go: Fiber, PostgreSQL, JWT and Swagger docs in isolated Docker containers](https://dev.to/koddr/build-a-restful-api-on-go-fiber-postgresql-jwt-and-swagger-docs-in-isolated-docker-containers-475j)
- [Getting started with Fiber](https://dev.to/fenny/getting-started-with-fiber-36b6)
- [Building an Express-style API in Go with Fiber](https://blog.logrocket.com/express-style-api-go-fiber/)
- [The road to web-based authentication with Fiber](https://vugt.me/the-road-to-web-based-authentication-with-fiber/)
- [Fiber v1.9.6 How to improve performance by 817% and stay fast, flexible and friendly?](https://dev.to/koddr/fiber-v1-9-5-how-to-improve-performance-by-817-and-stay-fast-flexible-and-friendly-2dp6)
- [Create a travel list app with Go, Fiber, Angular, MongoDB and Google Cloud Secret Manager](https://blog.yongweilun.me/create-a-travel-list-app-with-go-fiber-angular-mongodb-and-google-cloud-secret-manager-ck9fgxy0p061pcss1xt1ubu8t)
- [Building a Basic REST API in Go using Fiber](https://tutorialedge.net/golang/basic-rest-api-go-fiber/)
- [Creating Fast APIs In Go Using Fiber](https://dev.to/jozsefsallai/creating-fast-apis-in-go-using-fiber-59m9)
- [Is switching from Express to Fiber worth it?](https://dev.to/koddr/are-sure-what-your-lovely-web-framework-running-so-fast-2jl1)
- [Fiber v1.8. What's new, updated and re-thinked?](https://dev.to/koddr/fiber-v1-8-what-s-new-updated-and-re-thinked-339h)
- [Fiber released v1.7! What\'s new and is it still fast, flexible and friendly?](https://dev.to/koddr/fiber-v2-is-out-now-what-s-new-and-is-he-still-fast-flexible-and-friendly-3ipf)
- [Welcome to Fiber — an Express.js styled web framework written in Go with ❤️](https://dev.to/koddr/welcome-to-fiber-an-express-js-styled-fastest-web-framework-written-with-on-golang-497)

## 🤖 Benchmarks
Several benchmarks to compare Fiber with other frameworks.
- [TechEmpower](https://www.techempower.com/benchmarks/#section=data-r20&hw=ph&test=json)
- [web-frameworks-benchmark](https://web-frameworks-benchmark.netlify.app/result)
- [go-web-framework-benchmark](https://github.com/smallnest/go-web-framework-benchmark)


### 👍 Contributing

Contribution guidelines can be found on [CONTRIBUTING.md](https://github.com/gofiber/awesome-fiber/blob/master/CONTRIBUTING.md)

**Note:** Check finally: https://github.com/search?l=Go&p=3&q=fiber&type=Repositories, https://dev.to/search?q=fiber
