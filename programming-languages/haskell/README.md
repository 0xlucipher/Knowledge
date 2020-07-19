# Haskell

## Notes

* [Kinds are the types of types. Typeclasses are more like predicates or relations between types.](https://www.reddit.com/r/haskell/comments/8cdiql/isnt_a_typeclass_just_a_type_of_a_type/)
* The fewer type parameters in a class, the better. Can you turn any into associated types? Can you split the class into two classes? Can you hive off some of the parameters into a superclass?
* Don't worry about strictness until it's time to optimize.
* Intuition about optimization tends to be bad. Before profiling, limit yourself to reasoning about complexity classes.
* Don't judge haskell based on these definitions. They appear strange and crazy, but when you actually do stuff most of them turn out to be quite intuitive.
  * Advice is to ignore these things. Don't read a million monad tutorials. Just play around and code something, you don't have to understand the monad-definition before you can use the do-notation. Try to ignore them. After a while you get an intuition and then the definitions will make sense.
* Objects are a way to generalize reusability and composability \(Interheritance, Encapsulation, Polymorphism\) Haskell goes down a different route of reusability and composability that draws more from math than from object models. The real benefit to learning haskell is learning to think in that way rather than an object oriented or imperative way.
* In Haskell, you could say that the type system is a syntactic method for classifying program phrases according to the kinds of values they compute.
* Because Haskell \(usually\) only evaluates into [WHNF](https://wiki.haskell.org/Weak_head_normal_form) if you produce data constructors while doing the infinite recursion you can use infinite recursion.
* If, while forcing a thunk, you see the same thunk being forced again, you can report infinite recursion.
* [GADTs](https://en.wikibooks.org/wiki/Haskell/GADT) might give you a radically simple way to express things that rudimentary type systems like Go's cant express.
* Haskell's type system lets you express a lot of domain specific invariants and logic in a statically verifiable manner.
* Go is as type safe as haskell, the language doesn't allow invalid operations on data types. What people mean with "weak" is often expressivity. Go's enums sucks and it doesn't have ADTs or generic.
  * When people talk about strong type system, they usually just mean expressivity, not safety.

## Links

* [Haskell Programming Book](https://haskellbook.com/)
* [Thinking with Types by Sandy Maguire](https://leanpub.com/thinking-with-types)
* [How I Learned to Stop Worrying and Love the Type System](http://reasonablypolymorphic.com/blog/love-types/)
* [Simon Peyton Jones - Closer to Nirvana](https://www.youtube.com/watch?v=xmjvOLlCdFU)
* [Curry-Howard-Lambek correspondence](https://wiki.haskell.org/Curry-Howard-Lambek_correspondence)
* [Theoretical foundations](https://wiki.haskell.org/Category:Theoretical_foundations)
* [FP course](https://github.com/data61/fp-course)
* [Russian Haskell book FAQ](https://www.ohaskell.guide/haskell-faq.html)
* [An opinionated guide to Haskell in 2018](https://lexi-lambda.github.io/blog/2018/02/10/an-opinionated-guide-to-haskell-in-2018/)
* [Please Don't Learn Category Theory to Learn Haskell](https://jozefg.bitbucket.io/posts/2013-10-14-please-dont-learn-cat-theory.html)
* [How do you guys get anything done?](https://www.reddit.com/r/haskell/comments/5wb5qw/how_do_you_guys_get_anything_done/)
* [If Haskell is so great, why hasn't it taken over the world? And the curious case of Go.](https://pchiusano.github.io/2017-01-20/why-not-haskell.html)
* [Haskell IDE Engine](https://github.com/haskell/haskell-ide-engine) - Engine for haskell ide-integration.
* [Of Ideas and men](http://reasonablypolymorphic.com/blog/ideas-and-men/)
* [What is the track to mastering Haskell and where would it lead me professionally?](https://www.quora.com/profile/Edward-Kmett)
* [Nix and Haskell in production](https://github.com/Gabriel439/haskell-nix)
* [Revisiting Combinators by Edward Kmett](https://www.youtube.com/watch?v=PA1Fc7DNKtA)
* [Haskell Programming From First Principles - Follow-up Resources](https://github.com/pushcx/hpffp-resources) \([Solutions](https://github.com/Anton-Latukha/Haskell-Programming-From-First-Principles)\)
* [Quchen's articles](https://github.com/quchen/articles)
* [Haskell Design Patterns?](https://www.reddit.com/r/haskell/comments/5r271m/haskell_design_patterns/)
* [Haskell companies](https://github.com/erkmos/haskell-companies) - Curated list of companies using Haskell in industry.
* [Snack](https://github.com/nmattia/snack) - Nix-based incremental build tool for Haskell projects.
* [What exactly makes the Haskell type system so revered \(vs say, Java\)?](https://softwareengineering.stackexchange.com/questions/279316/what-exactly-makes-the-haskell-type-system-so-revered-vs-say-java)
* [HN: Introducing Haskell to a Company](https://news.ycombinator.com/item?id=18118874)
* [Haskell's kind system - a primer](https://diogocastro.com/blog/2018/10/17/haskells-kind-system-a-primer/)
* [Fused effects](https://github.com/robrix/fused-effects) - Fast, flexible, fused effect system for Haskell.
* [Examples of Dependently-typed programs in Haskell](https://github.com/sweirich/dth)
* [haskell-lsp](https://github.com/alanz/haskell-lsp) - Haskell library for the Microsoft Language Server Protocol.
* [Lambda World 2018 - Opening Keynote by Edward Kmett](https://www.youtube.com/watch?v=HGi5AxmQUwU)
* [Haskell Source Extensions](https://github.com/haskell-suite/haskell-src-exts) - Package for handling and manipulating Haskell source code.
* [Hedgehog](https://github.com/hedgehogqa/haskell-hedgehog) - Modern property-based testing system, in the spirit of QuickCheck.
* [Haskeleton: a Haskell project skeleton](http://taylor.fausak.me/2014/03/04/haskeleton-a-haskell-project-skeleton/)
* [Haskell ITMO course at CTDHaskell ITMO course at CTD](https://github.com/jagajaga/FP-Course-ITMO)
* [Google's Haskell training: 101 and 102](https://github.com/google/haskell-trainings)
* [brittany](https://github.com/lspitzner/brittany) - Haskell source code formatter.
* [Stack](https://github.com/commercialhaskell/stack) - Cross-platform program for developing Haskell projects.
* [List of Foundational Haskell Papers](https://github.com/cohomolo-gy/haskell-resources)
* [hpack](https://github.com/sol/hpack) - Modern format for Haskell packages.
* [Haskell Code Explorer](https://github.com/alexwl/haskell-code-explorer) - Web application for exploring and understanding Haskell codebases.
* [static-haskell-nix](https://github.com/nh2/static-haskell-nix) - Easily build most Haskell programs into fully static Linux executables.
* [Real World Haskell](http://book.realworldhaskell.org/read/)
* [Real World Haskell updated to 2019](https://github.com/tssm/up-to-date-real-world-haskell)
* [Higher-order Type-level Programming in Haskell \(2019\)](https://www.microsoft.com/en-us/research/uploads/prod/2019/03/ho-haskell-5c8bb4918a4de.pdf) \([HN](https://news.ycombinator.com/item?id=19412667)\)
* [Why Haskell?](https://github.com/github/semantic/blob/master/docs/why-haskell.md)
* [Property-Based Testing in a Screencast Editor: Introduction \(2019\)](https://wickstrom.tech/programming/2019/03/02/property-based-testing-in-a-screencast-editor-introduction.html)
* [Haskell Fan Site](http://www-cs-students.stanford.edu/~blynn/haskell/) \([HN](https://news.ycombinator.com/item?id=20255694)\)
* [An opinionated beginner's guide to Haskell in mid 2019](https://github.com/theindigamer/not-a-blog/blob/master/opinionated-haskell-guide-2019.md)
* [Why I \(as of June 22 2019\) think Haskell is the best general purpose language](http://www.philipzucker.com/why-i-as-of-june-22-2019-think-haskell-is-the-best-general-purpose-language-as-of-june-22-2019/)
* [Ormolu](https://github.com/tweag/ormolu) - Formatter for Haskell source code. \([Announcement article](https://www.tweag.io/posts/2019-10-11-ormolu-first-release.html)\)
* [Koka](https://github.com/koka-lang/koka) - Function-oriented language with effect inference.
* [Write You a Haskell](http://dev.stephendiehl.com/fun/) - Building a modern functional compiler from first principles.
* [Write You a Haskell 2](https://github.com/JKTKops/Write-You-a-Haskell-2) - Continuation of Steven Diehl's Write You a Haskell.
* [Verification with Refinement Types](https://ranjitjhala.github.io/CAV19-tutorial/00-outline.html)
* [Hoogle](https://github.com/ndmitchell/hoogle) - Haskell API search engine.
* [Haskell Papers](https://mitchellwrosen.github.io/haskell-papers/)
* [Simon Peyton Jones how GHC type inference engine actually works \(2019\)](https://www.youtube.com/watch?v=x3evzO8O9e8)
* [Chris Penner - Comonads by Example \(2019\)](https://www.youtube.com/watch?v=HOmOQnQGtPU&list=PLcAu_kKy-krxDD1WwRX_9rc0knAFK3nHs&index=7)
* [Haskell Disappointment \(2019\)](https://gist.github.com/nrinaudo/b02d0d17f62b6babea60cb0b52ded287) \([Reddit](https://www.reddit.com/r/haskell/comments/cyfs94/someones_haskell_disappointment_gist_i_came_across/)\)
* [MuniHac 2019: Making a Haskell IDE \(2019\)](https://www.youtube.com/watch?v=cijsaeWNf2E&list=PLxxF72uPfQVRdAsvj7THoys-nVj-oc4Ss) \([Slides](https://ndmitchell.com/downloads/slides-making_a_haskell_ide-07_sep_2019.pdf)\)
* [ghcide](https://github.com/digital-asset/ghcide) - Library for building Haskell IDE tooling.
* [llvm-hs](https://github.com/llvm-hs/llvm-hs) - Haskell bindings for LLVM.
* [Releaser](https://github.com/domenkozar/releaser) - Automation of Haskell package release process.
* [CodeWorld](https://github.com/google/codeworld) - Educational computer programming environment using Haskell.
* [Summoner](https://github.com/kowainik/summoner) - Tool for scaffolding batteries-included production-level Haskell projects.
* ["Building Haskell Programs with Fused Effects" by Patrick Thomson \(2019\)](https://www.youtube.com/watch?v=vfDazZfxlNs)
* [Haste Compiler](https://github.com/valderman/haste-compiler) - GHC-based Haskell to JavaScript compiler.
* [What is Good About Haskell? \(2019\)](https://doisinkidney.com/posts/2019-10-02-what-is-good-about-haskell.html) \([HN](https://news.ycombinator.com/item?id=21145014)\)
* [Learning Haskell is no harder than learning any other programming language \(2019\)](https://williamyaoh.com/posts/2019-10-05-you-are-already-smart-enough.html) \([HN](https://news.ycombinator.com/item?id=21170547)\) \([Reddit](https://www.reddit.com/r/haskell/comments/ddsvbk/you_are_already_smart_enough_to_write_haskell/)\)
* [Haskell eXchange 2019 talks](https://skillsmatter.com/conferences/11741-haskell-exchange-2019#skillscasts)
* [Implementation of the Elm Architecture in Haskell with parallel side effects](https://github.com/lazamar/elm-architecture-haskell)
* [Haskell in Production \(2019\)](http://felixmulder.com/writing/2019/10/05/Haskell-in-Production.html) \([HN](https://news.ycombinator.com/item?id=21282647)\)
* [Beating Decades Of Optimized C With 80 Lines Of Haskell \(2019\)](https://chrispenner.ca/posts/wc) \([HN](https://news.ycombinator.com/item?id=21266201)\) \([Lobsters](https://lobste.rs/s/l0lkyo/beating_decades_optimized_c_with_80_lines)\)
* [Servant's type-level domain specific language \(2019\)](https://dev.to/bradparker/servant-s-type-level-domain-specific-language-52m8)
* [Solutions to the Haskell Book exercises](https://github.com/kutyel/haskell-book) \([Solutions 2](https://github.com/yingw787/thehaskellbook)\)
* [Runtime Support for Multicore Haskell](https://simonmar.github.io/bib/papers/multicore-ghc.pdf)
* [GHC exercises](https://github.com/i-am-tom/haskell-exercises) - Little course to learn about some of the more obscure GHC extensions.
* [Typing the technical interview \(2017\)](https://aphyr.com/posts/342-typing-the-technical-interview)
* [Aelve Guide \| Haskell](https://guide.aelve.com/haskell) - Wiki-like guide to Haskell ecosystem and community.
* [rien](https://github.com/mrkgnao/rien) - Predictable Haskell development environments with Cabal and Nix.
* [Confessions of a Used Programming Language Salesman Getting the Masses Hooked on Haskell](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.72.868&rep=rep1&type=pdf)
* [Lambda World 2019 - Painless software development with Haskell - Paweł Szulc](https://www.youtube.com/watch?v=idU7GdlfP9Q)
* [Stay Tuned: Best Haskell Sources to Follow \(2019\)](https://serokell.io/blog/haskell-sources)
* [A dead-simple web stack in Haskell \(2019\)](https://williamyaoh.com/posts/2019-11-16-a-dead-simple-web-stack.html) \([HN](https://news.ycombinator.com/item?id=21566546)\)
* [simple-twitter](https://github.com/Gabriel439/simple-twitter) - Bare-bones Twitter clone implemented in a single file of Haskell deployed with Nix. \([HN](https://news.ycombinator.com/item?id=21599546)\) \([Slides](https://github.com/Gabriel439/slides/blob/master/simple-twitter/slides.md)\)
* [Boring Haskell Manifesto \(2019\)](https://www.snoyman.com/blog/2019/11/boring-haskell-manifesto)
* [HaskellR](https://github.com/tweag/HaskellR) - Full power of R in Haskell.
* [A List of Haskell Articles on good design, good testing](https://www.onikudaki.net/blog/wp-content/uploads/2019/12/HaskellArticles-1.pdf)
* [Is Haskell the functional end station or are there heavier drugs? \(2019\)](https://www.reddit.com/r/haskell/comments/e021oe/is_haskell_the_functional_end_station_or_are/)
* [Dependently Typed Haskell in Industry \(Experience Report\) \(2019\)](https://www.youtube.com/watch?v=Q6PKdRDKcKA)
* [Write Junior Code - A plea to Haskellers everywhere \(2019\)](https://www.parsonsmatt.org/2019/12/26/write_junior_code.html) \([Lobsters](https://lobste.rs/s/gdwjpc/plea_haskellers_everywhere_write_junior)\)
* [The road to proficient Haskell \(2020\)](https://williamyaoh.com/posts/2020-01-11-road-to-proficient.html)
* [Try the advanced stuff \(2020\)](https://williamyaoh.com/posts/2020-01-05-try-the-advanced-stuff.html)
* [Design Patterns in Haskell \(2010\)](http://blog.ezyang.com/2010/05/design-patterns-in-haskel/)
* [Courting Haskell \(2020\)](https://honzajavorek.cz/blog/courting-haskell)
* [Programming in Haskell book](http://www.cs.nott.ac.uk/~pszgmh/pih.html)
* [Static types are dangerously interesting](https://alexnixon.github.io/2020/01/14/static-types-are-dangerous.html) \([Lobsters](https://lobste.rs/s/6gzmym/static_types_are_dangerously)\)
* [Let's Get Dangerous](https://www.reddit.com/r/haskell/comments/epkn0z/lets_get_dangerous/) \([Reddit](https://www.reddit.com/r/haskell/comments/epkn0z/lets_get_dangerous/)\)
* [Functional Programming in Haskell \(Stepik course notes\) \(2020\)](https://hmemcpy.com/2020/01/functional-programming-in-haskell-stepik-course-notes-module-1/)
* [Haskell Problems For a New Decade \(2020\)](http://www.stephendiehl.com/posts/decade.html) \([HN](https://news.ycombinator.com/item?id=22137120)\)
* [Haskell performance checklist](https://github.com/haskell-perf/checklist)
* [Setting up a Haskell development environment in minutes in Visual Studio Code \(2020\)](https://hmemcpy.com/2020/02/setting-up-a-haskell-development-environment-in-minutes-in-vscode/) \([Lobsters](https://lobste.rs/s/b1tltx/setting_up_haskell_development)\)
* [Lessons learned from writing ShellCheck, GitHub’s now most starred Haskell project \(2020\)](https://www.vidarholen.net/contents/blog/?p=859) \([HN](https://news.ycombinator.com/item?id=22279585)\)
* [What I wish I knew when learning Haskell](http://dev.stephendiehl.com/hask/) \([Code](https://github.com/sdiehl/wiwinwlh)\) \([HN](https://news.ycombinator.com/item?id=22840211)\)
* [Awesome Haskell Deep Learning](https://github.com/austinvhuang/awesome-haskell-deep-learning)
* [Haskell Profile Highlight](https://github.com/Petrosz007/haskell-profile-highlight) - Color highlighting for Haskell profiling information.
* [Story told by Type Errors](https://kodimensional.dev/type-errors)
* [API design notes](https://gist.github.com/Gabriel439/563fa662f84e0a845c79775756cfce78) \([Video](https://www.twitch.tv/videos/581490043)\)
* [Retrie](https://github.com/facebookincubator/retrie) - Powerful, easy-to-use codemodding tool for Haskell.
* [Learn You a Haskell for Great Good](http://learnyouahaskell.com/chapters)
* [Lessons in Managing Haskell Memory \(2020\)](https://tech.channable.com/posts/2020-04-07-lessons-in-managing-haskell-memory.html)
* [Building a web app with functional programming - Haskell \(2020\)](https://blog.patchgirl.io/haskell/2020/03/08/haskell-part-I.html)
* [haskell-language-server](https://github.com/haskell/haskell-language-server) - Integration point for ghcide and haskell-ide-engine. One IDE to rule them all.
* [Why Haskell Matters](https://github.com/thma/WhyHaskellMatters)
* [Fast Fibonacci numbers using Monoids \(2020\)](http://www.haskellforall.com/2020/04/blazing-fast-fibonacci-numbers-using.html) \([HN](https://news.ycombinator.com/item?id=22946710)\)
* [Permissive, then restrictive: learning how to design Haskell programs \(2020\)](https://williamyaoh.com/posts/2020-04-19-permissive-vs-restrictive.html)
* [10 Reasons to Use Haskell \(2020\)](https://serokell.io/blog/10-reasons-to-use-haskell) \([Lobsters](https://lobste.rs/s/afq4js/10_reasons_use_haskell)\)
* [Haskell Study Plan](https://github.com/soupi/haskell-study-plan)
* [Examples of Incorrect Abstractions in Other Languages \(2020\)](https://www.reddit.com/r/haskell/comments/glz389/examples_of_incorrect_abstractions_in_other/) \([Lobsters](https://lobste.rs/s/ky2fu3/examples_incorrect_abstractions_non)\)
* [Haskell Platform](https://github.com/haskell/haskell-platform) - Combination of the GHC compiler and core libraries, plus additional tools and libraries covering a range of common programming tasks.
* [Stan](https://github.com/kowainik/stan) - Haskell static analyser.
* [Software Design and Architecture in Haskell](https://github.com/graninas/software-design-in-haskell) - Structured set of materials. How to build real-world applications in Haskell.
* [The Pain Points of Haskell: A Practical Summary \(2020\)](https://dixonary.co.uk/blog/haskell/pain/) \([HN](https://news.ycombinator.com/item?id=23454352)\)
* [nix-hs](https://github.com/pjones/nix-hs) - Thin layer over the existing Haskell infrastructure in nixpkgs which adds all of the tools needed for interactive development.
* [Haskell for Imperative Programmers \(2020\)](https://www.youtube.com/playlist?list=PLe7Ei6viL6jGp1Rfu0dil1JH1SHk9bgDV)
* [Haskell Zettelkasten](https://haskell.zettel.page/) - Seeks to be a comprehensive community-maintained knowledge-base for Haskell. \([Code](https://github.com/Kuratoro/haskell.zettel.page)\)
* [Opening Ceremony & "Languages all the way down" by Rob Rix - ZuriHac 2020](https://www.youtube.com/watch?v=kCpQ4aTzlis) \([Code](https://github.com/robrix/languages-all-the-way-down)\)
* [ZuriHac 2020](https://www.youtube.com/playlist?list=PLiU7KJ5_df6aZbNfh_TUJt-6w9N3rYkTX)
* [Smuggler2](https://github.com/jrp2014/smuggler2) - Minimise haskell imports, make exports explicit.
* [Alexis King - “Effects for Less” \(2020\)](https://www.youtube.com/watch?list=PLiU7KJ5_df6aZbNfh_TUJt-6w9N3rYkTX&v=0jI-AlWEwYI)
* [A Generic Journey - Design Decisions about datatype-generic programming in Haskell \(2020\)](https://github.com/well-typed/gp-zurihac-2020/blob/master/GP.pdf)
* [Linear types are merged in GHC \(2020\)](https://www.tweag.io/blog/2020-06-19-linear-types-merged/) \([Proposal](https://github.com/ghc-proposals/ghc-proposals/pull/111)\) \([Lobsters](https://lobste.rs/s/lc20e3/linear_types_are_merged_ghc)\) \([HN](https://news.ycombinator.com/item?id=23574072)\) \([Drafts, notes](https://github.com/tweag/linear-types)\)
* [GHC Proposals](https://github.com/ghc-proposals/ghc-proposals)
* [Fundamental Haskell notes](https://blog.latukha.com/haskell-notes) \([Code](https://github.com/Anton-Latukha/haskell-notes)\)
* [Haskell for a New Decade](http://dev.stephendiehl.com/new_decade.pdf) \([HN](https://news.ycombinator.com/item?id=23621080)\) \([Talk](https://www.youtube.com/watch?v=B9_xAixGlmk)\) \([Lobsters](https://lobste.rs/s/jbugyx/haskell_for_new_decade)\)
* [IHP](https://ihp.digitallyinduced.com/) - Modern batteries-included Web Framework, built on top of Haskell and Nix. \([HN](https://news.ycombinator.com/item?id=23610527)\) \([Code](https://github.com/digitallyinduced/ihp)\)
* [The power of IO in Haskell \(2020\)](https://www.47deg.com/blog/io-haskell/)
* [JSON Parser 100% From Scratch in Haskell \(only 111 lines\) \(2019\)](https://www.youtube.com/watch?v=N9RUqGYuGfw)
* [Learn Haskell in a couple of tweets \(2020\)](https://twitter.com/k0001/status/1277615394560360449)
* [Kindness for Mean Girls: Primer on the cruel, tacit laws of type-level programming in Haskell \(2020\)](https://www.aymannadeem.com/haskell/2020/05/15/Kindness-for-Mean-Girls.html)
* [Deploying statically-linked Haskell to Lambda \(2020\)](https://lazamar.github.io/deploying-statically-linked-haskell-to-lambda/)
* [Retrie](https://github.com/facebookincubator/retrie/) - Powerful, easy-to-use codemodding tool for Haskell. \([Article](https://engineering.fb.com/open-source/retrie/)\)
* [cabal-edit](https://github.com/sdiehl/cabal-edit) - Utility for managing Hackage dependencies from the command line.
