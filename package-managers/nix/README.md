# Nix

## Notes

* Nix never uses host dependencies, it always builds with exactly precise dependencies every time, and will always refer to them from then on.
* Nix lets you roll back changes atomically.
* nix-shell lets you make build environments that are totally reproducible across machines, and don’t interfere with each other. You can freely mix any number of libraries of versions or software on the same machine and they don’t conflict.
* With Ubuntu, every time you want to fix something with your car, you roll it into the garage, pop open the hood and get to work. It's intensive labour, results will vary, and undoing a change can be difficult.
  * With NixOS, it's like 3D printing a new car every time. You'll design a model, press a button, and the car gets built from scratch. If you don't like it, tweak the design a bit, and print a new car. If the new car breaks, just go back to the previous known-good one, which is already in your garage. You can even take the design documents to your friend and generate an exactly identical model.
* `sudo` command sets the wrong `$HOME`, have to use `sudo -i` for nix commands that need sudo.
* Nix is Turing complete language used for configuration and building packages.
* Can use nox, nix search, nix-repl, [nixOS packages](https://nixos.org/nixos/packages.html#) to search for packages.
* Think of Nix \(the language\) as an expression-based programming language where every program evaluates to a single \(possibly complex\) value; that resulting value is what is used as eg. the configuration of your system or a package, but it means that you can generate that value based on arbitrary logic and abstractions like you would with a regular programming language.
* As for domain-specific package managers, It Depends; it's possible with varying degrees of hackiness \(and I definitely use eg. npm for development\), but for a 'real' deployment - whether as a service on a server or as a local application - you'd want to convert your project's metadata to a Nix expression and let Nix handle the dependency management.
* Overlay adds/overrides something in the global package set.
* In general, you should only install things with nix, and not use any other package managers.
* The main idea of the Nix approach is to store software components in isolation from each other in a central component store, under path names that contain cryptographic hashes of all inputs involved in building the component, such as `/nix/store/rwmfbhb2znwp...-ﬁrefox1.0.4`.
* Don't install libraries with Nix.
* Can put ``` in``sha256`initially. Before getting the real SHA256 with`nix-prefetch-url\`.
* Derivations are variables + build script.
* Docs are in `.xml` files in `/docs`
* To build derivation in nixpkgs, at root of `nixpkgs`, run `nix build -f . <pkg-name>` \(ie `nix build -f . wifi-password`\)
* To find out the SHA256, run `nix-prefetch-url -A <pkg-name>.src` \(ie `nix-prefetch-url -A wifi-password.src`\). `nix-prefetch-url` works with GitHub. This gives you the SHA256 you can copy.

## Links

* [Nix manual](https://nixos.org/nix/manual/)
* [Nix pills](https://nixos.org/nixos/nix-pills/index.html)
* [Benefits of using nix](https://www.reddit.com/r/haskell/comments/7wmhyi/an_opinionated_guide_to_haskell_in_2018/du2506q/)
* [Nix, the purely functional build system](http://www.boronine.com/2018/02/02/Nix/) - Great intro article.
* [A Gentle Introduction to the Nix Family](https://ebzzry.io/en/nix/)
* [Nix: A Reproducible Setup for Linux and macOS](http://nmattia.com/posts/2018-03-21-nix-reproducible-setup-linux-macos.html)
* [hnix](https://github.com/jwiegley/hnix) - Haskell re-implementation of the Nix expression language.
* [Haskell & Nix](https://github.com/Gabriel439/haskell-nix)
* [Brian McKenna - Nix for Functional Systems](https://www.youtube.com/watch?v=mIxtBVKo7JE)
* [Learning Nix by Example: Building FFmpeg 4.0](https://blog.kiloreux.me/2018/05/24/learning-nix-by-example-building-ffmpeg-4-dot-0/)
* [nix-shell and Shebang Lines](http://iam.travishartwell.net/2015/06/17/nix-shell-shebang/)
* [Domen Kožar, Lead DevOps, Nix workshop](https://www.youtube.com/watch?v=BjRGlKNHeEc)
* [Cheap Docker images with Nix](http://lethalman.blogspot.com/2016/04/cheap-docker-images-with-nix_15.html)
* [When to use declarative approach and when not](https://www.reddit.com/r/NixOS/comments/95vczu/when_to_use_declarative_approach_and_when_not/)
* [example-nix](https://github.com/shajra/example-nix) - A way to develop software with Nix.
* [Hercules CI](https://hercules-ci.com/) - Hosted CI for building Nix projects on your infrastructure.
* [Dysnomia](https://github.com/svanderburg/dysnomia) - Tool and plug-in system that can be used to automatically deploy mutable components.
* [Disnix](https://github.com/svanderburg/disnix) - Nix-based distributed service deployment tool.
* [NUR](https://github.com/nix-community/NUR) - Nix User Repository: User contributed nix packages.
* [Eris](https://github.com/thoughtpolice/eris) - Binary cache for Nix.
* [pypi2nix](https://github.com/garbas/pypi2nix) - Generate Nix expressions for Python packages.
* [hnix-store](https://github.com/haskell-nix/hnix-store) - Haskell implementation of the nix store API.
* [nix-cheatsheet](https://github.com/knedlsepp/nix-cheatsheet)
* [Nix RFCs](https://github.com/NixOS/rfcs)
* [nix-linter](https://github.com/Synthetica9/nix-linter) - Linter for the Nix expression language.
* [Install Nix docs by Mozilla](https://docs.mozilla-releng.net/develop/install-nix.html) - Pretty good.
* [Nix scripts shared across IOHK projects](https://github.com/input-output-hk/iohk-nix)
* [niv](https://github.com/nmattia/niv) - Painless dependencies for Nix projects.
* [Cachix](https://cachix.org/) - Build Nix packages once and share them for good.
* [Alternative Haskell Infrastructure for Nixpkgs](https://github.com/input-output-hk/haskell.nix) - Works by automatically translating your Cabal or Stack project and its dependencies into Nix code.
* [nix-bundle](https://github.com/matthewbauer/nix-bundle) - Bundle Nix derivations to run anywhere.
* [crate2nix](https://github.com/kolloch/crate2nix) - Nix build file generator for rust crates. \([Lobsters](https://lobste.rs/s/26xnzy/crate2nix_nix_build_file_generator_for)\)
* [lorri](https://github.com/target/lorri) - nix-shell replacement for project development.
* [Awesome Nix](https://github.com/nix-community/awesome-nix)
* [nixfmt](https://github.com/serokell/nixfmt) - Formatter for Nix code.
* [Nix for devs](https://github.com/uniphil/nix-for-devs) - Collection of recipes focused on nix-shell to make setting up project environments easy.
* [nixpkgs-fmt](https://github.com/nix-community/nixpkgs-fmt) - Nix code formatter for nixpkgs.
* [Nix builder for Kubernetes](https://gist.github.com/tazjin/08f3d37073b3590aacac424303e6f745)
* [Nixery](http://nixery.dev/nixery.html) - Provides the ability to pull ad-hoc container images from a Docker-compatible registry server. \([Code](https://github.com/google/nixery)\)
* [Nixery: Improved Layering Design \(2019\)](https://tazj.in/blog/nixery-layers)
* [hnix-lsp](https://github.com/domenkozar/hnix-lsp) - Language Server Protocol for Nix.
* [Make Nix precisely emulate gitignore](https://github.com/hercules-ci/gitignore.nix)
* [Nixery](https://github.com/google/nixery) - Container registry which transparently builds images using the Nix package manager.
* [Nix - A One Pager](https://github.com/tazjin/nix-1p) - A \(more or less\) one page introduction to Nix, the language.
* [yants](https://github.com/tazjin/yants) - Tiny type-checker for data in Nix, written in Nix.
* [nix-shorts](https://github.com/justinwoo/nix-shorts) - Collection of short notes about Nix, down to what is immediately needed for users.
* [rnix-parser](https://github.com/nix-community/rnix-parser) - Nix parser written in Rust.
* [Naersk](https://github.com/nmattia/naersk) - Nix support for building cargo crates.
* [nix-diff](https://github.com/Gabriel439/nix-diff) - Explain why two Nix derivations differ.
* [Optimising Docker Layers for Better Caching with Nix \(2018\)](https://grahamc.com/blog/nix-and-layered-docker-images)
* [nix-du](https://github.com/symphorien/nix-du) - Visualise which gc-roots to delete to free some space in your nix store.
* [NixCon 2019 - Main Track](https://www.youtube.com/watch?v=aUG9aGYYCY8)
* [Nix flakes \(2019\)](https://www.youtube.com/watch?v=UeBX7Ide5a0)
* [Nix: How and Why it Works \(2019\)](https://www.youtube.com/watch?v=lxtHH838yko)
* [Nix recipes for Haskellers](https://www.srid.ca/haskell-nix.html)
* [format-nix](https://github.com/justinwoo/format-nix) - Simple formatter for Nix using tree-sitter-nix.
* [go-nix](https://github.com/orivej/go-nix) - Nix language parser and Nix-compatible file hasher in Go.
* [nix-dns](https://github.com/kirelagin/nix-dns) - Nix DSL for DNS zone files.
* [Nix-based app VMs](https://github.com/jollheef/appvm)
* [nix-index](https://github.com/bennofs/nix-index) - Quickly locate nix packages with specific files.
* [Nix-bisect](https://github.com/timokau/nix-bisect) - Bisect Nix Builds.
* [Thoughts on Nix \(2020\)](https://christine.website/blog/thoughts-on-nix-2020-01-28) \([Lobsters](https://lobste.rs/s/tp6o0q/thoughts_on_nix)\)
* [I was Wrong about Nix \(2020\)](https://christine.website/blog/i-was-wrong-about-nix-2020-02-10) \([HN](https://news.ycombinator.com/item?id=22295102)\) \([Lobsters](https://lobste.rs/s/4otqzp/i_was_wrong_about_nix)\)
* [Grafanix](https://github.com/stolyaroleh/grafanix) - Visualize your Nix dependencies.
* [What's your configuration.nix like?](https://www.reddit.com/r/NixOS/comments/9aa08b/whats_your_configurationnix_like/)
* [Built with Nix](https://builtwithnix.org/) - Build software only once. \([Code](https://github.com/nix-community/builtwithnix.org)\)
* [How I Start: Nix \(2020\)](https://christine.website/blog/how-i-start-nix-2020-03-08) \([Lobsters](https://lobste.rs/s/lktf6u/how_i_start_nix)\)
* [rnix-lsp](https://github.com/nix-community/rnix-lsp) - WIP Language Server for Nix.
* [Eelco Dolstra's talks/papers](https://edolstra.github.io/) \([Code](https://github.com/edolstra/edolstra.github.io)\)
* [Nix Haskell Monorepo Tutorial](https://github.com/fghibellini/nix-haskell-monorepo)
* [The journey of packaging a .NET app on Nix \(2020\)](https://sgt.hootr.club/molten-matter/dotnet-on-nix/)
* [nixpkgs](https://github.com/NixOS/nixpkgs) - Nix Packages collection.
* [Nix IRC logs](https://logs.nix.samueldr.com/)
* [Nixology \(2020\)](https://www.youtube.com/playlist?list=PLRGI9KQ3_HP_OFRG6R-p4iFgMSK1t5BHs) - Series of videos I've been releasing within Shopify to help promote and educate about Nix.
* [Nix function to easily create derivations \(packages\) to install binaries from location](https://twitter.com/mitchellh/status/1259521715211657216)
* [What Is Nix \(2020\)](https://engineering.shopify.com/blogs/engineering/what-is-nix) \([HN](https://news.ycombinator.com/item?id=23251754)\) \([Lobsters](https://lobste.rs/s/bgwsd8/what_is_nix)\)
* [comma](https://github.com/Shopify/comma) - Runs software without installing it. Wraps together nix run and nix-index.
* [nix-derivation](https://github.com/Gabriel439/Haskell-Nix-Derivation-Library) - Parse and render \*.drv files.
* [nix-build-uncached](https://github.com/Mic92/nix-build-uncached) - CI friendly wrapper around nix-build.
* [nix-tests](https://github.com/cleverca22/nix-tests) - Scratchpad for small experimental things I am doing with Nix.
* [Nix Flakes, Part 1: An introduction and tutorial \(2020\)](https://www.tweag.io/posts/2020-05-25-flakes.html)
* [Nix Flakes, Part 1: An introduction and tutorial](https://www.tweag.io/blog/2020-05-25-flakes/) \([Lobsters](https://lobste.rs/s/h99uo8/nix_flakes_part_1_introduction_tutorial)\)
* [nix-overlays of Antonio Monteiro](https://github.com/anmonteiro/nix-overlays)
* [A Nix terminology primer by a newcomer \(2020\)](https://stephank.nl/p/2020-06-01-a-nix-primer-by-a-newcomer.html)
* [Statistical Rethinking and Nix \(2020\)](https://rgoswami.me/posts/rethinking-r-nix/)
* [flake-utils](https://github.com/numtide/flake-utils) - Pure Nix flake utility functions.
* [nix.dev](https://nix.dev/) - Opinionated guide for developers wanting to get things done using the Nix ecosystem. \([Code](https://github.com/nix-dot-dev/nix.dev)\)
* [Nix language antipatterns](https://nix.dev/anti-patterns/language.html)
* [So, tell me about Nix \(2020\)](https://ghedam.at/15490/so-tell-me-about-nix)
* [nixdu](https://github.com/utdemir/nixdu) - Interactively browse the dependency graph of your Nix derivations.
* [Nix Package Versions](https://lazamar.co.uk/nix-versions/) - Search for old versions of Nix packages. \([Code](https://github.com/lazamar/nix-package-versions)\) \([Reddit](https://www.reddit.com/r/NixOS/comments/gc68ec/find_older_versions_of_a_package_in_the_nix/)\)
* [Opinionated Nix repository template](https://github.com/nix-dot-dev/getting-started-nix-template) - Based on nix.dev tutorials, repository template to get you started with Nix.
* [Tools to manage a Nix-based project](https://github.com/shajra/nix-project)
* [Building static Haskell binary with Nix on Linux \(2020\)](https://blog.patchgirl.io/haskell/2020/07/13/static-haskell-binary.html)
* [Template for NUR repositories](https://github.com/rvolosatovs/nur-packages)
