# Go

Go is currently my favorite programming language.

I mostly love the tooling around it like [VS Code](../../text-editors/vs-code/) and its [Go plugin](https://github.com/golang/vscode-go). The powerful `go` command line tool and the rich ecosystem of libraries and tools that people have built.

Go promotes composition over inheritance.

## Commenting Go code

* Comments documenting declarations should be full sentences.
* Comments should begin with the name of the thing being described and end in a period.

## Error checking

* You can `log.Fatal(err)` when playing with code.
  * In actual applications you need to decide what you need to do with each error response - bail immediately, pass it to the caller, show it to the user, log it and continue, etc ...

## Notes

* I can call functions from anywhere if they are in the same package.
* The package “main” tells the Go compiler that the package should compile as an executable program instead of a shared library.
* Note that any type implements the empty interface interface{} because it doesn't have any methods and all types have zero methods by default.
* Simply pushing my source code to GitHub, makes it `go get`table.
* Interface types represent fixed sets of methods.
* the prevailing wisdom in Go is to use a flat directory structure and only create new directories when you are building self-contained functionality.
* `go get` = download the source code to your PC.
* `go install` = download, build, and put it in the path so you can use it.
* I don't need to comment all functions as some are self describing. I do need to comment exported functions however.
* [What works well is to use Go to create an HTTP API and leave the rest \(html templates etc\) to a client-side frontend \(e.g. React\). That gives you the best of both worlds: a fast and lightweight backend in Go with a rich frontend in JS.](https://www.reddit.com/r/golang/comments/8eeolx/recommended_web_framework_for_go/)
* This is a core concept in Go’s type system; instead of designing our abstractions in terms of what kind of data our types can hold, we design our abstractions in terms of what actions our types can execute.
* [In Go, as long as you are not sharing data, you don't really have to care about whether something is concurrent or parallel, the runtime takes care of it for you. You just use goroutines, IO transparently happens on a dedicated threadpool, CPU heavy tasks are spread out over the available cores.](https://news.ycombinator.com/item?id=20210850)
* [How to edit Go packages locally](https://twitter.com/zekjur/status/1226487216937086976)
* [The main sell point of Go is not simplicity, but overall balance and flexibility](https://news.ycombinator.com/item?id=21744910)

## Links

* [Tour of Go](https://tour.golang.org) \([Solutions](https://github.com/golang/tour/tree/master/solutions)\)
* [Effective Go](https://golang.org/doc/effective_go.html)
* [How to Write Go Code](https://golang.org/doc/code.html)
* [Go proverbs](https://go-proverbs.github.io/)
* [Go internals](https://github.com/teh-cmc/go-internals)
* [Go 101](https://go101.org/article/101.html) - Great book.
* [Notes on Go](https://brandur.org/go)
* [Avoiding complexity in Go](https://bradgignac.com/2014/09/24/avoiding-complexity-with-go.html)
* [Gopher reading list](https://github.com/enocom/gopher-reading-list)
* [Go Code Review Comments](https://github.com/golang/go/wiki/CodeReviewComments)
* [Performance without the event loop \(2015\)](https://dave.cheney.net/2015/08/08/performance-without-the-event-loop)
* [7 common mistakes in Go and when to avoid them by Steve Francia](https://www.youtube.com/watch?v=29LLRKIL_TI)
* [Performance without the event loop \(2015\)](https://dave.cheney.net/2015/08/08/performance-without-the-event-loop)
* [What I learned in 2017 Writing Go](https://www.commandercoriander.net/blog/2017/12/31/writing-go/)
* [Golang interfaces](https://blog.chewxy.com/2018/03/18/golang-interfaces/)
* [Go in 5 minutes](https://github.com/arschles/go-in-5-minutes)
* [Learn Go with tests](https://github.com/quii/learn-go-with-tests)
* [Using Instruments to profile Go programs](https://rakyll.org/instruments/)
* [Design Philosophy On Packaging](https://www.ardanlabs.com/blog/2017/02/design-philosophy-on-packaging.html)
* [Go best practices, six years in](https://peter.bourgon.org/go-best-practices-2016/#repository-structure)
* [Standard Package Layout](https://medium.com/@benbjohnson/standard-package-layout-7cdbc8391fc1)
* [Style guideline for Go packages](https://rakyll.org/style-packages/)
* [Share memory by communicating](https://blog.golang.org/share-memory-by-communicating)
* [Go Build Template](https://github.com/thockin/go-build-template)
* [Go for Industrial Programming](https://peter.bourgon.org/go-for-industrial-programming/) - Great insights.
* [Sum Types in Go](http://www.jerf.org/iri/post/2917)
* [Gophercises](https://gophercises.com/) - Free coding exercises for budding gophers.
* [Joy Compiler](https://mat.tm/joy/) - Translate idiomatic Go into concise JavaScript that works in every browser.
* [The Go Type System for newcomers](https://rakyll.org/typesystem/)
* [Web Assembly and Go: A look to the future \(2018\)](https://brianketelsen.com/web-assembly-and-go-a-look-to-the-future/)
* [How I Learned to Stop Worrying and Love Golang](https://corte.si/posts/code/go/golang-practicaly-beats-purity/index.html)
* [List of advices and tricks in the Go's world](https://github.com/cristaloleg/go-advices)
* [Golang challenge](http://golang-challenge.org/)
* [dep2nix](https://github.com/nixcloud/dep2nix) - Using golang/dep to create a deps.nix file for go projects to package them for nixpkgs.
* [GopherCon 2018 - Rethinking Classical Concurrency Patterns](https://about.sourcegraph.com/go/gophercon-2018-rethinking-classical-concurrency-patterns/) - [Slides](https://drive.google.com/file/d/1nPdvhB0PutEJzdCq5ms6UI58dp50fcAN/view)
* [Standard Go Project Layout](https://github.com/golang-standards/project-layout)
* [Building Web Apps with Go](https://codegangsta.gitbooks.io/building-web-apps-with-go/content/)
* [Golang Monorepo](https://github.com/flowerinthenight/golang-monorepo) - Example of a golang-based monorepo.
* [Lorca](https://github.com/zserge/lorca) - Build cross-platform modern desktop apps in Go + HTML5.
* [Data Structures with Go Language](https://github.com/Dentrax/Data-Structures-with-Go)
* [go-hardware](https://github.com/rakyll/go-hardware) - Directory of hardware related libs, tools, and tutorials for Go.
* [HN: Go 2, here we go \(2018\)](https://news.ycombinator.com/item?id=18561587)
* [gotestsum](https://github.com/gotestyourself/gotestsum) - Runs tests, prints friendly test output and a summary of the test run.
* [Nice example of a small Go CLI tool](https://github.com/htdvisser/did)
* [GolangCI-Lint](https://github.com/golangci/golangci-lint) - Linters Runner for Go. 5x faster than gometalinter. Nice colored output. Can report only new issues. Fewer false-positives. Yaml/toml config.
* [Nice VS Code Go snippets](https://github.com/tj/vscode-snippets)
* [revive](https://github.com/mgechev/revive) - Fast, configurable, extensible, flexible, and beautiful linter for Go.
* [Going Infinite, handling 1M websockets connections in Go \(2019\)](https://github.com/eranyanay/1m-go-websockets)
* [Awesome Go Linters](https://github.com/golangci/awesome-go-linters)
* [Awesome Go Books](https://github.com/dariubs/GoBooks)
* [Leaktest](https://github.com/fortytw2/leaktest) - Goroutine Leak Detector.
* [Practical Go: Real world advice for writing maintainable Go programs \(2018\)](https://dave.cheney.net/practical-go/presentations/qcon-china.html) \([HN](https://news.ycombinator.com/item?id=19218097)\)
* [The State of Go: Feb 2019](https://speakerdeck.com/campoy/the-state-of-go-feb-2019?slide=38)
* [gomacro](https://github.com/cosmos72/gomacro) - Interactive Go interpreter and debugger with generics and macros.
* [go2ll-talk](https://github.com/pwaller/go2ll-talk) - Live coding a basic Go compiler with LLVM in 20 minutes.
* [Thoughts on Go performance optimization](https://github.com/dgryski/go-perfbook)
* [Go Package Store](https://github.com/shurcooL/Go-Package-Store) - App that displays updates for the Go packages in your GOPATH.
* [Why are my Go executable files so large? Size visualization of Go executables using D3 \(2019\)](https://science.raphael.poss.name/go-executable-size-visualization-with-d3.html)
* [goweight](https://github.com/jondot/goweight) - Tool to analyze and troubleshoot a Go binary size.
* [Go Patterns](https://github.com/tmrts/go-patterns) - Curated list of Go design patterns, recipes and idioms.
* [Go Developer Roadmap](https://github.com/Alikhll/golang-developer-roadmap) - Roadmap to becoming a Go developer in 2019.
* [Clear is better than clever \(2019\)](https://dave.cheney.net/paste/clear-is-better-than-clever.pdf) \([HN](https://news.ycombinator.com/item?id=19837981)\)
* [Retool](https://github.com/twitchtv/retool) - Vendoring for executables written in Go.
* [Why Go? – Key advantages you may have overlooked](https://yourbasic.org/golang/advantages-over-java-python/)
* [Go Creeping In \(2019\)](https://www.tbray.org/ongoing/When/201x/2019/06/12/Go-Creeping-In) \([HN](https://news.ycombinator.com/item?id=20210850)\)
* [Getting to Go: The Journey of Go's Garbage Collector \(2018\)](https://blog.golang.org/ismmkeynote)
* [Clean Go Code](https://github.com/Pungyeon/clean-go-article) - Reference for the Go community that aims to help developers write cleaner code.
* [Go Language Server](https://github.com/sourcegraph/go-langserver) - Adds Go support to editors and other tools that use the Language Server Protocol \(LSP\).
* [Go talks](https://github.com/golang/talks)
* [TinyGo](https://github.com/tinygo-org/tinygo) - Go compiler for small places.
* [Yaegi](https://github.com/containous/yaegi) - Another Elegant Go Interpreter.
* [Delve](https://github.com/go-delve/delve) - Debugger for the Go programming language.
* [Experiment, Simplify, Ship \(2019\)](https://blog.golang.org/experiment)
* [Go programming language secure coding practices guide](https://github.com/OWASP/Go-SCP)
* [Ultimate Go study guide](https://github.com/hoanhan101/ultimate-go) \([HN](https://news.ycombinator.com/item?id=20701671)\)
* [Redress](https://github.com/goretk/redress) - Tool for analyzing stripped binaries.
* [Ask HN: Is there a project based book or course on Go for writing web APIs? \(2019\)](https://news.ycombinator.com/item?id=20704993)
* [Data Structure Libraries and Algorithms implementation in Go](https://github.com/x899/algorithms)
* [GitHub Actions for Go](https://github.com/mvdan/github-actions-golang) - Using GitHub Actions as CI effectively for Go.
* [NFPM](https://github.com/goreleaser/nfpm) - Simple deb and rpm packager written in Go.
* [Why Go and not Rust? \(2019\)](https://kristoff.it/blog/why-go-and-not-rust/) \([HN](https://news.ycombinator.com/item?id=20983922)\)
* [Algorithms implemented in Go \(for education\)](https://github.com/TheAlgorithms/Go)
* [go-callvis](https://github.com/TrueFurby/go-callvis) - Visualize call graph of a Go program using dot \(Graphviz\).
* [goo](https://github.com/benbjohnson/goo) - Simple wrapper around the Go toolchain.
* [Go Cheat Sheet](https://github.com/a8m/golang-cheat-sheet) - Overview of Go syntax and features.
* [packr](https://github.com/gobuffalo/packr) - Simple and easy way to embed static files into Go binaries.
* [Uber Go Style Guide](https://github.com/uber-go/guide/blob/master/style.md) \([HN](https://news.ycombinator.com/item?id=21225401)\)
* [Interpreting Go \(2019\)](http://notes.eatonphil.com/interpreting-go.html)
* [gijit](https://github.com/gijit/gi) - Just-in-time trace-compiled golang REPL. Standing on the shoulders of giants \(GopherJS and LuaJIT\).
* [unconvert](https://github.com/mdempsky/unconvert) - Remove unnecessary type conversions from Go source.
* [Gox](https://github.com/mitchellh/gox) - Simple Go Cross Compilation.
* [Learning Go: Lexing and Parsing \(2016\)](http://blog.leahhanson.us/post/recursecenter2016/recipeparser.html)
* [Running a serverless Go web application \(2019\)](https://bartfokker.com/posts/cloud-run/)
* [Awesome Go Storage](https://github.com/gostor/awesome-go-storage)
* [Go Modules: v2 and Beyond \(2019\)](https://blog.golang.org/v2-go-modules)
* [Let's Create a Simple Load Balancer With Go \(2019\)](https://kasvith.github.io/posts/lets-create-a-simple-lb-go/) \([HN](https://news.ycombinator.com/item?id=21490731)\)
* [The Value in Go's Simplicity \(2019\)](https://benjamincongdon.me/blog/2019/11/11/The-Value-in-Gos-Simplicity/) \([HN](https://news.ycombinator.com/item?id=21545425)\)
* [Google OAuth Go Sample Project - Web application](https://github.com/Skarlso/google-oauth-go-sample)
* [Go’s features of last resort \(2019\)](https://www.arp242.net/go-last-resort.html) \([Lobsters](https://lobste.rs/s/bq4nxd/go_s_features_last_resort)\) \([HN](https://news.ycombinator.com/item?id=21603483)\)
* [Minigo](https://github.com/DQNEO/minigo) - Small Go compiler made from scratch. It can compile itself. The goal is to be the most easy-to-understand Go compiler.
* [Writing An Interpreter In Go](https://interpreterbook.com/) \([HN](https://news.ycombinator.com/item?id=21626972)\) \([Notes](https://joeprevite.com/book-review-writing-an-interpreter-in-go)\)
* [Source Code for Go In Action](https://github.com/goinaction/code)
* [garble](https://github.com/mvdan/garble) - Obfuscate Go builds.
* [Using Makefile\(s\) for Go \(2019\)](https://danishpraka.sh/2019/12/07/using-makefiles-for-go.html)
* [The Go runtime scheduler's clever way of dealing with system calls \(2019\)](https://utcc.utoronto.ca/~cks/space/blog/programming/GoSchedulerAndSyscalls) \([HN](https://news.ycombinator.com/item?id=21736342)\)
* [Go Things I Love: Methods On Any Type \(2019\)](https://www.justindfuller.com/posts/2019-12-14_Go-Things-I-Love-Methods-On-Any-Type) \([Reddit](https://www.reddit.com/r/golang/comments/eaqnyh/go_things_i_love_methods_on_any_type/)\)
* [Golang for Node.js Developers](https://github.com/miguelmota/golang-for-nodejs-developers) - Examples of Golang examples compared to Node.js for learning.
* [Testing in Go: Test Doubles by Example \(2019\)](https://ieftimov.com/post/testing-in-go-test-doubles-by-example/)
* [Chime](https://www.chimehq.com/) - Go editor for macOS. \([HN](https://news.ycombinator.com/item?id=21963708)\)
* [Go Things I Love: Channels and Goroutines \(2020\)](https://www.justindfuller.com/2020/01/go-things-i-love-channels-and-goroutines/) \([HN](https://news.ycombinator.com/item?id=21968939)\)
* [go-ruleguard](https://github.com/quasilyte/go-ruleguard) - Define and run pattern-based custom linting rules.
* [Go by Example](https://gobyexample.com/) - Hands-on introduction to Go using annotated example programs. \([Code](https://github.com/mmcgrana/gobyexample)\)
* [Introduction to Programming in Go book](https://www.golang-book.com/books/intro)
* [A Chapter in the Life of Go’s Compiler \(2020\)](https://medium.com/samsara-engineering/a-chapter-in-the-life-of-gos-compiler-c89b9db74617)
* [JWT Authorization in Golang \(2019\)](https://www.cloudjourney.io/articles/security/jwt_in_golang-su/)
* [govalidate](https://github.com/rakyll/govalidate) - Validates your Go installation and dependencies.
* [Go: Best Practices for Production Environments](https://peter.bourgon.org/go-in-production/)
* [Go Code Review Comments](https://github.com/golang/go/wiki/CodeReviewComments)
* [A theory of modern Go \(2017\)](https://peter.bourgon.org/blog/2017/06/09/theory-of-modern-go.html)
* [Golang IO Cookbook](https://github.com/jesseduffield/notes/wiki/Golang-IO-Cookbook)
* [cob](https://github.com/knqyf263/cob) - Continuous Benchmark for Go Project.
* [Concurrency in Go - Fundamentals \(2018\)](https://rogerwelin.github.io/golang/go/concurrency/2018/09/04/golang-concurrency-fundamentals.html)
* [Go + Services = One Goliath Project \(2020\)](https://engineering.khanacademy.org/posts/goliath.htm) \([HN](https://news.ycombinator.com/item?id=21853727)\)
* [Pure reference counting garbage collector in Go](https://github.com/sendilkumarn/gopurerc) \([HN](https://news.ycombinator.com/item?id=22052119)\)
* [JSON to Go](https://mholt.github.io/json-to-go/) - Convert JSON to Go struct. \([Code](https://github.com/mholt/json-to-go)\)
* [The await/async concurrency pattern in Golang \(2020\)](https://madeddu.xyz/posts/go-async-await/)
* [Exposing interfaces in Go \(2019\)](https://www.efekarakus.com/golang/2019/12/29/working-with-interfaces-in-go.html)
* [Go Error Handling — Best Practice in 2020](https://itnext.io/golang-error-handling-best-practice-a36f47b0b94c)
* [An Introduction To Concurrency In Go \(2020\)](https://seancarpenter.io/posts/concurrency_in_go/)
* [Concurrency in Go book \(2017\)](https://www.oreilly.com/library/view/concurrency-in-go/9781491941294/)
* [PubSub using channels in Go \(2020\)](https://eli.thegreenplace.net/2020/pubsub-using-channels-in-go/)
* [Build Web Application with Golang book](https://astaxie.gitbooks.io/build-web-application-with-golang/en/)
* [SOLID Go Design \(2016\)](https://dave.cheney.net/2016/08/20/solid-go-design)
* [Better Go Playground](https://github.com/x1unix/go-playground) - Improved Go Playground powered by Monaco Editor and React.
* [Algorithms with Go course](https://algorithmswithgo.com/)
* [Interfaces in Go \(2018\)](https://medium.com/rungo/interfaces-in-go-ab1601159b3a) - Interface is a great and only way to achieve Polymorphism in Go.
* [Allocation efficiency in high-performance Go services \(2017\)](https://segment.com/blog/allocation-efficiency-in-high-performance-go-services/)
* [service-training](https://github.com/ardanlabs/service-training) - Training material for the service repo.
* [Starter code for writing web services in Go](https://github.com/ardanlabs/service)
* [How I write Go HTTP services after seven years \(2018\)](https://medium.com/statuscode/how-i-write-go-http-services-after-seven-years-37c208122831)
* [Let's Go! Learn to Build Professional Web Applications With Golang](https://lets-go.alexedwards.net/)
* [Go's Tooling Is an Undervalued Technology \(2020\)](https://nullprogram.com/blog/2020/01/21/) \([HN](https://news.ycombinator.com/item?id=22113827)\)
* [GoProxy](https://github.com/goproxyio/goproxy) - Global proxy for Go modules. \([Web](https://goproxy.io/)\)
* [Adrian Cockcroft: Communicating Sequential Goroutines \(2016\)](https://www.youtube.com/watch?v=gO1qF19y6KQ)
* [Go FAQ](https://golang.org/doc/faq)
* [gosec](https://github.com/securego/gosec) - Golang Security Checker.
* [Inlined defers in Go \(2020\)](https://rakyll.org/inlined-defers/)
* [Andre Carvalho - Understanding Go's Memory Allocator \(2018\)](https://andrestc.com/post/go-memory-allocation-pt1/) \([Video](https://www.youtube.com/watch?v=3CR4UNMK_Is)\)
* [Make resilient Go net/http servers using timeouts, deadlines and context cancellation \(2020\)](https://ieftimov.com/post/make-resilient-golang-net-http-servers-using-timeouts-deadlines-context-cancellation/) \([Lobsters](https://lobste.rs/s/hmzsdm/make_resilient_go_net_http_servers_using)\)
* [tparse](https://github.com/mfridman/tparse) - Command line tool for analyzing and summarizing go test output.
* [Go Walkthrough](https://medium.com/go-walkthrough) - Series of walkthroughs to help you understand the Go standard library better.
* [Go modules by example](https://github.com/go-modules-by-example/index)
* [curl-to-Go](https://mholt.github.io/curl-to-go/) - Instantly convert curl commands to Go code. \([Code](https://github.com/mholt/curl-to-go)\)
* [Best Practices for Errors in Go \(2014\)](https://justinas.org/best-practices-for-errors-in-go)
* [Go command overview](https://golang.org/cmd/go/)
* [Functional options on steroids \(2020\)](https://sagikazarmark.hu/blog/functional-options-on-steroids/) \([Reddit](https://www.reddit.com/r/golang/comments/ev863i/functional_options_on_steroids/)\)
* [Go internals: capturing loop variables in closures \(2020\)](https://eli.thegreenplace.net/2019/go-internals-capturing-loop-variables-in-closures/)
* [go-mod-upgrade](https://github.com/oligot/go-mod-upgrade) - Update outdated Go dependencies interactively.
* [go: observing stack grow and shrink \(2020\)](https://ops.tips/notes/go-observing-stack-grow-and-shrink/)
* [Readiness notifications in Go \(2020\)](https://michael.stapelberg.ch/posts/2020-02-02-readiness-notifications-in-golang/)
* [GoReleaser](https://github.com/goreleaser/goreleaser) - Deliver Go binaries as fast and easily as possible.
* [Zen of Go](https://the-zen-of-go.netlify.com/) - Ten engineering values for writing simple, readable, maintainable Go code. \([Code](https://github.com/davecheney/the-zen-of-go)\) \([HN](https://news.ycombinator.com/item?id=22396405)\)
* [go-clean-arch](https://github.com/bxcodec/go-clean-arch) - Go Clean Architecture based on Reading Uncle Bob's Clean Architecture.
* [Why Discord is switching from Go to Rust \(2020\)](https://blog.discordapp.com/why-discord-is-switching-from-go-to-rust-a190bbca2b1f) \([HN](https://news.ycombinator.com/item?id=22238335)\) \([Reddit](https://www.reddit.com/r/programming/comments/eyuebc/why_discord_is_switching_from_go_to_rust/)\) \([Lobsters](https://lobste.rs/s/34sse3/why_discord_is_switching_from_go_rust)\)
* [Running Go CLI programs in the browser \(2020\)](https://www.arp242.net/wasm-cli.html) \([Lobsters](https://lobste.rs/s/5r1h5r/running_go_cli_programs_browser)\)
* [GoDays Go talks \(2020\)](https://speakerdeck.com/godays)
* [Golang basics - writing unit tests \(2017\)](https://blog.alexellis.io/golang-writing-unit-tests/)
* [Buffered channels in go: tips & tricks \(2020\)](https://www.rapidloop.com/blog/golang-channels-tips-tricks.html)
* [The Evolution of a Go Programmer](https://github.com/SuperPaintman/the-evolution-of-a-go-programmer)
* [Staticcheck](https://github.com/dominikh/go-tools) - Collection of static analysis tools for working with Go code.
* [Go Diagnostics](https://golang.org/doc/diagnostics.html)
* [Experience report on a large Python-to-Go translation](https://gitlab.com/esr/reposurgeon/blob/master/GoNotes.adoc) \([HN](https://news.ycombinator.com/item?id=22304131)\)
* [profefe](https://github.com/profefe/profefe) - Collect profiling data for long-term analysis.
* [Go support for Mobile devices](https://github.com/golang/mobile)
* [Go for Cloud \(2020\)](https://rakyll.org/go-cloud/)
* [Why are my Go executable files so large?](https://dr-knz.net/go-executable-size-visualization-with-d3.html) - Size visualization of Go executables using D3.
* [Testing in Go: Clean Tests Using t.Cleanup \(2020\)](https://ieftimov.com/post/testing-in-go-clean-tests-using-t-cleanup/)
* [Go Up](https://github.com/rvflash/goup) - Checks if there are any updates for imports in your module.
* [I want off Mr. Golang's Wild Ride \(2020\)](https://news.ycombinator.com/item?id=22443363) \([HN](https://news.ycombinator.com/item?id=22443363)\)
* [Early Impressions of Go from a Rust Programmer \(2020\)](https://pingcap.com/blog/early-impressions-of-go-from-a-rust-programmer/)
* [Install go tools from modules with brew-gomod \(2020\)](https://blog.filippo.io/install-go-tools-from-modules-with-brew-gomod/)
* [Illustrated Tales of Go Runtime Scheduler \(2020\)](https://medium.com/@ankur_anand/illustrated-tales-of-go-runtime-scheduler-74809ef6d19b)
* [Google Cloud Platform Go Samples](https://github.com/GoogleCloudPlatform/golang-samples)
* [prealloc](https://github.com/alexkohler/prealloc) - Go static analysis tool to find slice declarations that could potentially be preallocated.
* [Why you shouldn't use func main in Go](https://pace.dev/blog/2020/02/12/why-you-shouldnt-use-func-main-in-golang-by-mat-ryer) \([Lobsters](https://lobste.rs/s/nvjvm0/why_you_shouldn_t_use_func_main_go)\)
* [Diago](https://github.com/remeh/diago) - Visualization tool for CPU profiles and heap snapshots generated with `pprof`.
* [pkgviz-go](https://github.com/tiegz/pkgviz-go) - Generate a visualization of a Go package's types.
* [Setup for Your Next Golang Project](https://martinheinz.dev/blog/5) \([HN](https://news.ycombinator.com/item?id=21725869)\)
* [HN: Go Turns 10](https://news.ycombinator.com/item?id=21483933)
* [Benchmarking Go programs \(2017\)](https://scene-si.org/2017/06/06/benchmarking-go-programs/)
* [gopkg](https://labix.org/gopkg.in) - Service provides versioned URLs that offer the proper metadata for redirecting the go tool onto well defined GitHub repositories. \([Code](https://github.com/niemeyer/gopkg)\)
* [Go Binaries](https://github.com/tj/gobinaries) - On-demand binary server, allowing non-Go users to quickly install tools written in Go without installing go itself. \([Article](https://cto.ai/blog/on-demand-go-binaries/)\)
* [gosize](https://github.com/bradfitz/gosize) - Analyze size of Go binaries.
* [tre](https://github.com/zegl/tre) - LLVM backed Go compiler.
* [Statically compiling Go programs \(2020\)](https://www.arp242.net/static-go.html)
* [Understanding bytes in Go by building a TCP protocol \(2020\)](https://ieftimov.com/post/understanding-bytes-golang-build-tcp-protocol/)
* [Go Quirks \(2020\)](https://blog.sbstp.ca/go-quirks/)
* [Debugging with Delve](https://tpaschalis.github.io/delve-debugging/) \([HN](https://news.ycombinator.com/item?id=22865526)\)
* [GoDoc Tricks](https://godoc.org/github.com/fluhus/godoc-tricks) \([Code](https://github.com/fluhus/godoc-tricks)\)
* [Thanos Coding Style Guide](https://thanos.io/contributing/coding-style-guide.md/)
* [faillint](https://github.com/fatih/faillint) - Report unwanted import path and declaration usages.
* [Broccoli](https://github.com/aletheia-icu/broccoli) - Using brotli compression to embed static files in Go.
* [Export data, the secret of Go's fast builds \(2020\)](https://www.jayconrod.com/posts/112/export-data--the-secret-of-go-s-fast-builds)
* [Awesome Go performance](https://github.com/cristaloleg/awesome-go-perf)
* [Understand Go pointers in less than 800 words or your money back \(2017\)](https://dave.cheney.net/2017/04/26/understand-go-pointers-in-less-than-800-words-or-your-money-back) \([Reddit](https://www.reddit.com/r/golang/comments/g5o3k4/coming_from_javascript_and_im_on_a_go_project_now/)\)
* [Go & iOS: remember to enable Cocoa multithreading \(2020\)](https://medium.com/@steeve/go-ios-remember-to-enable-cocoa-multithreading-95394491ad5e)
* [Go Tools](https://github.com/golang/tools) - Various packages and tools that support the Go programming language.
* [Collection of Technical Interview Questions solved with Go](https://github.com/shomali11/go-interview)
* [Go Project Design Documents](https://github.com/golang/proposal)
* [Inlining optimisations in Go \(2020\)](https://dave.cheney.net/2020/04/25/inlining-optimisations-in-go)
* [Examples for my talk on structuring Go apps](https://github.com/katzien/go-structure-examples)
* [Rob Pike interview: “Go has indeed become the language of cloud infrastructure“ \(2020\)](https://evrone.com/rob-pike-interview) \([HN](https://news.ycombinator.com/item?id=23031778)\)
* [I think you should generally be using the latest version of Go \(2020\)](https://utcc.utoronto.ca/~cks/space/blog/programming/GoVersionsMyView) \([Lobsters](https://lobste.rs/s/xwedeg/i_think_you_should_generally_be_using)\)
* [Go Build Tools](https://github.com/golang/build) - Go's continuous build and release infrastructure.
* [What's coming in Go 1.15](https://docs.google.com/presentation/d/1veyF0y6Ynr6AFzd9gXi4foaURlgbMxM-tmB4StDrdAM/edit) \([Lobsters](https://lobste.rs/s/b6nyir/what_s_coming_go_1_15)\)
* [Writing Useful go/analysis Linter \(2019\)](https://disaev.me/p/writing-useful-go-analysis-linter/)
* [How to check whether a struct implements an interface in GoLang](https://www.pixelstech.net/article/1588481241-How-to-check-whether-a-struct-implements-an-interface-in-GoLang) \([Lobsters](https://lobste.rs/s/fhpv3s/how_check_whether_struct_implements)\)
* [How the Go runtime implements maps efficiently \(without generics\) \(2018\)](https://dave.cheney.net/2018/05/29/how-the-go-runtime-implements-maps-efficiently-without-generics)
* [Write your own Go static analysis tool \(2020\)](https://about.houqp.me/posts/write-your-own-go-static-analysis-tool/) \([Lobsters](https://lobste.rs/s/dslgsa/write_your_own_go_static_analysis_tool)\)
* [Hand-crafted Go exercises and examples](https://github.com/inancgumus/learngo) \([HN](https://news.ycombinator.com/item?id=23206440)\)
* [GoLand Tips & Tricks](https://github.com/dlsniper/golandtipsandtricks)
* [gorram](https://github.com/natefinch/gorram) - Like go run for any go function.
* [errwrap](https://github.com/fatih/errwrap) - Go tool to wrap and fix errors with the new %w verb directive.
* [mockery](https://github.com/vektra/mockery) - Mock code autogenerator for golang.
* [Writing type parametric functions in Go \(2013\)](https://blog.burntsushi.net/type-parametric-functions-golang/)
* [maybedoer: the Maybe Monoid for Go \(2020\)](https://christine.website/blog/maybedoer-2020-05-23) \([Lobsters](https://lobste.rs/s/kfsim9/maybedoer_maybe_monoid_for_go)\)
* [Learning Go \(2020\)](https://destroytoday.com/blog/learning-go)
* [golintui](https://github.com/nakabonne/golintui) - TUI tool that helps you run various kinds of linters with ease and organize its results, with the power of golangci-lint.
* [Instrumentation in Go \(2020\)](https://gbws.io/articles/instrumentation-in-go/) \([HN](https://news.ycombinator.com/item?id=23308357)\)
* [Go Vanity URLs](https://github.com/GoogleCloudPlatform/govanityurls) - Simple Go server that allows you to set custom import paths for your Go packages.
* [Pkger](https://github.com/markbates/pkger) - Embed static files in Go binaries.
* [asmfmt](https://github.com/klauspost/asmfmt) - Go Assembler Formatter.
* [Diving into Go by building a CLI application \(2020\)](https://eryb.space/2020/05/27/diving-into-go-by-building-a-cli-application.html) \(\[[HN](https://news.ycombinator.com/item?id=23318137)\]\) \([Reddit](https://www.reddit.com/r/golang/comments/grgvlu/diving_into_go_by_building_a_cli_application/)\)
* [Testify](https://github.com/stretchr/testify) - Toolkit with common assertions and mocks that plays nicely with the standard library.
* [Go and CPU Caches \(2020\)](https://medium.com/@teivah/go-and-cpu-caches-af5d32cc5592)
* [go-mod-outdated](https://github.com/psampaz/go-mod-outdated) - Easy way to find outdated dependencies of your Go projects.
* [Featherweight Go \(2020\)](https://arxiv.org/abs/2005.11710) \([HN](https://news.ycombinator.com/item?id=23368453)\) \([Talk](https://www.youtube.com/watch?v=Dq0WFigax_c)\) \([Implementation](https://github.com/rhu1/fgg)\)
* [lean](https://github.com/jadekler/lean) - Smart Go module dependency inspection and pruning.
* [impl](https://github.com/josharian/impl) - Generates method stubs for implementing an interface.
* [air](https://github.com/cosmtrek/air) - Live reload for Go apps.
* [The Go compiler needs to be smarter \(2020\)](https://lemire.me/blog/2020/06/04/the-go-compiler-needs-to-be-smarter/) \([HN](https://news.ycombinator.com/item?id=23423755)\) \([Reddit](https://www.reddit.com/r/golang/comments/gwlrms/the_go_compiler_needs_to_be_smarter/)\)
* [Swag](https://github.com/swaggo/swag) - Converts Go annotations to Swagger Documentation 2.0.
* [The Cache Replacement Problem \(2020\)](http://alexandrutopliceanu.ro/post/cache-replacement-problem/)
* [Tengo](https://github.com/d5/tengo) - Small, dynamic, fast, secure script language for Go.
* [Getting Hands-on with io\_uring using Go \(2020\)](https://developers.mattermost.com/blog/hands-on-iouring-go/)
* [json2go web parser](https://m-zajac.github.io/json2go/) - Paste json to generate go struct. \([Code](https://github.com/m-zajac/json2go)\)
* [Writing Go CLIs With Just Enough Architecture \(2020\)](https://blog.carlmjohnson.net/post/2020/go-cli-how-to-and-advice/) \([Reddit](https://www.reddit.com/r/golang/comments/gyxfvp/how_to_write_a_cli_with_just_enough_architecture/)\)
* [Go SPA](https://github.com/tj/spa) - Tiny Single Page Application server for Go with `spa` command-line tool.
* [Featherweight Generic Go Generator](https://github.com/wenkokke/featherweight-go-gen)
* [An intro to Go for non-Go developers \(2020\)](https://benhoyt.com/writings/go-intro/) \([Lobsters](https://lobste.rs/s/epfuar/introduction_go_for_non_go_developers)\)
* [Ultimate Go Programming Videos \(2018\)](https://www.oreilly.com/library/view/ultimate-go-programming/9780135261651/)
* [Building a better Go linker \(2019\)](http://golang.org/s/better-linker)
* [Gdlv](https://github.com/aarzilli/gdlv) - GUI frontend for Delve.
* [The Next Step for Generics \(2020\)](https://blog.golang.org/generics-next-step) \([HN](https://news.ycombinator.com/item?id=23543131)\) \([Reddit](https://www.reddit.com/r/golang/comments/haaz5w/the_next_step_for_generics_the_go_blog/)\) \([Lobsters](https://lobste.rs/s/ondg75/next_step_for_generics)\)
* [oto](https://github.com/pacedotdev/oto) - Go driven rpc code generation tool for right now.
* [In Go, the compiler needs to know the types of things when copying values \(2020\)](https://utcc.utoronto.ca/~cks/space/blog/programming/GoValueCopyIsTyped) \([Lobsters](https://lobste.rs/s/rnm3re/go_compiler_needs_know_types_things_when)\)
* [exportloopref](https://github.com/kyoh86/exportloopref) - Analyzer that finds exporting pointers for loop variables.
* [A Concise Guide to the Latest Go Generics Draft Design \(2020\)](https://pmihaylov.com/go-generics-draft-design/) \([HN](https://news.ycombinator.com/item?id=23562897)\)
* [fgprof](https://github.com/felixge/fgprof) - Sampling Go profiler that allows you to analyze On-CPU as well as Off-CPU \(e.g. I/O\) time together. \([Tweet](https://twitter.com/felixge/status/1275833124103086080)\)
* [How To Code in Go book by Digital Ocean \(2020\)](https://www.digitalocean.com/community/books/how-to-code-in-go-ebook)
* [astextract](https://github.com/lu4p/astextract) - Convert a go file to its ast representation.
* [binclude](https://github.com/lu4p/binclude) - Include files in your binary the easy way.
* [Go Modules- A guide for monorepos \(2020\)](https://engineering.grab.com/go-module-a-guide-for-monorepos-part-1)
* [Generics for Go \(2020\)](https://lwn.net/SubscriberLink/824716/ee9bbbfad58cef3d/) \([Lobsters](https://lobste.rs/s/ac83w9/generics_for_go)\)
* [Go is boring, and that’s fantastic \(2020\)](https://www.capitalone.com/tech/software-engineering/go-is-boring/) \([HN](https://news.ycombinator.com/item?id=23711735)\) \([Reddit](https://www.reddit.com/r/golang/comments/hjqouw/go_is_boringand_thats_fantastic/)\)
* [godepgraph](https://github.com/kisielk/godepgraph) - Program for generating a dependency graph of Go packages.
* [\[RU\] Multithreading in Go - Aliaksandr Valialkin \(2018\)](https://www.youtube.com/watch?v=HzAXT1ORH3o)
* [A Go lesson learned: sometimes I don't want to use goroutines if possible \(2020\)](https://utcc.utoronto.ca/~cks/space/blog/programming/GoWhenNotManyGoroutines) \([Lobsters](https://lobste.rs/s/joicca/go_lesson_learned_sometimes_i_don_t_want)\)
* [Why Go’s Error Handling is Awesome \(2020\)](https://rauljordan.com/2020/07/06/why-go-error-handling-is-awesome.html) \([HN](https://news.ycombinator.com/item?id=23758509)\) \([Reddit](https://www.reddit.com/r/golang/comments/hmnhkz/why_gos_error_handling_is_awesome/)\)
* [Keeping Your Modules Compatible \(2020\)](https://blog.golang.org/module-compatibility) \([HN](https://news.ycombinator.com/item?id=23761450)\)
* [Using go/analysis to fix your source code \(2020\)](https://arslan.io/2020/07/07/using-go-analysis-to-fix-your-source-code/)
* ["Interface smuggling", a Go design pattern for expanding APIs \(2020\)](https://utcc.utoronto.ca/~cks/space/blog/programming/GoInterfaceSmuggling)
* [What feature of Go is used often by experienced programmers, but not so much by a newbie? \(2020\)](https://www.reddit.com/r/golang/comments/hp4mk3/what_feature_of_go_is_used_very_often_by/)
* [copyist](https://github.com/cockroachdb/copyist) - Mocking your SQL database in Go tests has never been easier. \([HN](https://news.ycombinator.com/item?id=23811698)\)
* [PopCount on ARM64 in Go Assembler \(2020\)](https://barakmich.dev/posts/popcnt-arm64-go-asm/)
* [GopherCon Europe: Online 2020](https://www.youtube.com/playlist?list=PLtoVuM73AmsKnUvoFizEmvWo0BbegkSIG)
* [Go’s History in Code \(2020\)](https://seh.dev/go-legacy/)
* [The impact on middleware of expanding APIs with Go's interface smuggling](https://utcc.utoronto.ca/~cks/space/blog/programming/GoMiddlewareVsInterfaceSmuggling) \([HN](https://news.ycombinator.com/item?id=23799833)\)
