# Type Theory

## Notes

* A value is some concrete thing, and a type is a collection of concrete things \(but is itself not a concrete thing. For example any individual integer is a value, but the collection of all integers is a type. Much like elements and sets in set theory.
* A type is a collection of values which inhabit that type. A type is a value which is a member of the type of types.
* Type theory goes much much further than just tagging data.
* The type determines which data structure you use.
* Dependent types is basically about being able to express arbitrary things in your type system, meaning that you can construct arbitrary proofs. That's how Coq, Agda and Idris work.
* Types are types and propositions are propositions; types come from programming languages, and propositions from logic, and they seem to have no relation to each other.
* [Types are specifications of behavior.](https://www.youtube.com/watch?v=LE0SSLizYUI)
* Roughly speaking, a [type is a specification of its possible values](https://github.com/skaslev/why-types/blob/master/why-types.pdf).

## Links

* [Learn TT](https://github.com/jozefg/learn-tt) - A collection of resources for learning type theory and type theory adjacent fields.
* [Homotopy Type Theory lecture materials](https://github.com/RobertHarper/hott-materials)
* [A textbook on informal homotopy type theory](https://github.com/HoTT/book)
* [Homotopy type theory book](https://github.com/HoTT/HoTT)
* [GHOTL Project scope and outline plan](https://sphalerite.org/ghotl/posts/2017-10-16-project-scope-outline.html) - Good read.
* [What I wish I knew when learning HoTT](https://abooij.github.io/wiwikwlhott/)
* [Collected works of Per Martin-Löf](https://github.com/michaelt/martin-lof) - [Web version](http://archive-pml.github.io/).
* [Type Theory: Does understanding of the Curry-Howard correspondence make you a better programmer?](http://qr.ae/TUpF3Z)
* [Hazel](https://github.com/hazelgrove/hazel) - Live functional programming environment with typed holes. \([Web](https://hazel.org/)\)
* [LaTTe](https://github.com/latte-central/LaTTe) - Laboratory for Type Theory experiments \(in clojure\).
* [TT Lite](https://github.com/ilya-klyuchnikov/ttlite) - SuperCompiler for Martin-Löf's Type Theory.
* [Implementation of spartan type theory](https://github.com/andrejbauer/spartan-type-theory)
* [Why Types Matter](https://github.com/skaslev/why-types/blob/master/why-types.pdf)
* [Introduction to type theory based on meaning explanations](https://github.com/jonsterling/type-theory-and-its-meaning-explanations)
* [SymmetryBook](https://github.com/UniMath/SymmetryBook) - Undergraduate textbook written in the univalent style, taking advantage of the presence of symmetry in the logic at an early stage.
* [nbe-for-mltt](https://github.com/jozefg/nbe-for-mltt) - Normalization by Evaluation for Martin-Löf Type Theory.
* [Martin Escardo's research](http://www.cs.bham.ac.uk/~mhe/)
* [Lambdas are Codatatypes \(2019\)](http://blog.ielliott.io/lambdas-are-codatatypes/)
* [On the Relationship Between Static Analysis and Type Theory \(2019\)](https://semantic-domain.blogspot.com/2019/08/on-relationship-between-static-analysis.html) \([Lobsters](https://lobste.rs/s/irow0u/on_relationship_between_static_analysis)\)
* \[Timeline for Logic, λ-Calculus, and Programming Language Theory \(2012\)\([http://fm.csl.sri.com/SSFT15/Timeline.pages.pdf](http://fm.csl.sri.com/SSFT15/Timeline.pages.pdf)\) \([HN](https://news.ycombinator.com/item?id=20860888)\)
* [Types and Programming Languages book](https://www.cis.upenn.edu/~bcpierce/tapl/)
* [Type Theory and Formal Proof book](https://www.goodreads.com/book/show/21442441-type-theory-and-formal-proof)
* [qtt](https://github.com/LightAndLight/qtt) - Quantitative Type Theory implementation.
* [Normalization by evaluation for Martin-Löf Type Theory with dependent records](https://github.com/brendanzab/rust-nbe-for-mltt)
* [Introduction to Type Theory \(2019\)](https://jadon.io/blog/type-theory/)
* [No, dynamic type systems are not inherently more open \(2020\)](https://lexi-lambda.github.io/blog/2020/01/19/no-dynamic-type-systems-are-not-inherently-more-open/) \([HN](https://news.ycombinator.com/item?id=22090700)\) \([Lobsters](https://lobste.rs/s/qqlkk0/no_dynamic_type_systems_are_not)\)
* [Hindley-Milner type system/Algorithm W study \(2018\)](http://boxbase.org/entries/2018/mar/5/hindley-milner/)
* [HN: So you want to write a type checker](https://news.ycombinator.com/item?id=15583515)
* [What are the common ways of performing typechecking? \(2019\)](https://www.reddit.com/r/ProgrammingLanguages/comments/87c5dw/what_are_the_common_ways_of_performing/)
* [mlsub](https://github.com/stedolan/mlsub) - Prototype type inference engine.
* [Papers and talks around type inference](http://stedolan.net/research/#mlsub)
* [Low-Level Liquid Types](http://goto.ucsd.edu/~rjhala/papers/low_level_liquid_types.pdf)
* [PRL Project](http://www.nuprl.org/) - Implementing computational mathematics and providing logic-based tools that help automate programming.
* [Code is Engineering; Types are Science \(2020\)](https://www.tweag.io/posts/2020-03-05-peirce.html) \([HN](https://news.ycombinator.com/item?id=22791187)\)
* [Implementation of "Complete and Easy Bidirectional Typechecking for Higher-Rank Polymorphism" in Rust](https://github.com/JDemler/BidirectionalTypechecking) \([Paper](https://arxiv.org/pdf/1306.6032.pdf)\)
* [Milner Award Lecture: The Type Soundness Theorem That You Really Want to Prove \(and now you can\)](https://www.youtube.com/watch?v=8Xyk_dGcAwk)
* [Experimenting with Dependent Type Theory in Rust](https://github.com/phase/dtt)
* [Making Illegal States Unrepresentable \(2020\)](https://buttondown.email/hillelwayne/archive/making-illegal-states-unrepresentable/) \([Lobsters](https://lobste.rs/s/b0p6ib/making_illegal_states_unrepresentable)\)
* [Beautiful, interactive visualizations of logical inference](https://github.com/ezyang/logitext)
* [Type Inference by Example](https://github.com/Ahnfelt/type-inference-by-example)
* [First-Class Dynamic Types \(2019\)](https://michael.homer.nz/Publications/DLS2019/pattern-types.pdf)
* [Gradual Typing for Extensibility by Rows \(2019\)](https://arxiv.org/pdf/1910.08480.pdf)
* [Graduality and Parametricity: Together Again for the First Time \(2020\)](https://www.ccs.neu.edu/home/amal/papers/gradparam.pdf)
* [Abstracting gradual typing: metatheory and applications \(2019\)](http://repositorio.uchile.cl/bitstream/handle/2250/170935/Abstracting-gradual-typing-Metatheory-and-applications.pdf?sequence=1)
* [Gradual Typing as if Types Mattered \(2020\)](https://wgt20.irif.fr/wgt20-final28-acmpaginated.pdf)
* [Disjoint Intersection Types: Theory and Practice \(2018\)](https://bixuanzju.github.io/files/Thesis.pdf)
* [The Fire Triangle \(2020\)](https://hal.archives-ouvertes.fr/hal-02383109/document)
* [Foreign Function Typing: Semantic Type Soundness for FFIs \(2020\)](https://wgt20.irif.fr/wgt20-final23-acmpaginated.pdf)
* [Bidirectional Typing \(2019\)](https://arxiv.org/pdf/1908.05839.pdf)
* [Refinement Kinds \(2019\)](https://arxiv.org/pdf/1908.00441.pdf) - Type-safe Programming with Practical Type-level Computation.
* [Refinement type contracts for verification of scientific investigative software \(2019\)](https://arxiv.org/pdf/1909.00427.pdf)
* [Design and Evaluation of Contracts for Gradual Typing \(2019\)](https://jackw.io/papers/thesis.pdf)
* [Manifest Contracts with Intersection Types \(2019\)](https://arxiv.org/pdf/1908.03010.pdf)
* [Kinds are calling conventions \(2019\)](https://www.microsoft.com/en-us/research/uploads/prod/2019/03/eta.pdf)
* [Space-Efficient Monotonic References \(2020\)](https://wgt20.irif.fr/wgt20-final70-acmpaginated.pdf)
* [Label-Dependent Session Types \(2019\)](https://arxiv.org/pdf/1911.00705.pdf)
* [Tabled Typeclass Resolution \(2020\)](https://arxiv.org/pdf/2001.04301.pdf)
* [A type and effect system for uniqueness and immutability \(2018\)](https://www.researchgate.net/publication/326164533_A_type_and_effect_system_for_uniqueness_and_immutability)
* [Inferring Types and Effects via Static Single AssignmentLeonardo](https://dl.acm.org/doi/pdf/10.1145/3341105.3373888)
* [smalltt](https://github.com/AndrasKovacs/smalltt) - Demo for high-performance type theory elaboration.
* [Hoare Type Theory](https://github.com/imdea-software/htt) - Contains the main libraries of Hoare Type Theory \(HTT\) for reasoning about sequential heap-manipulating programs.
* [Type inference under the hood \(2019\)](https://www.aleksandra.codes/type-inference)
* [Type inference for beginners \(2019\)](https://medium.com/@dhruvrajvanshi/type-inference-for-beginners-part-1-3e0a5be98a4b)
* [Algorithm W Step by Step \(2006\)](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.65.7733&rep=rep1&type=pdf) - Implementation of the classic algorithm W for Hindley- Milner polymorphic type inference in Haskell.
* [Elaboration with First-Class Implicit Function Types \(2020\)](https://github.com/AndrasKovacs/icfp20sub/blob/master/paper.pdf) \([Code](https://github.com/AndrasKovacs/icfp20sub/tree/master/fcif)\)
* [Experimental type-checker for internally parametric type theory](https://github.com/ecavallo/ptt)
* [Type Systems as Macros \(2017\)](http://www.ccs.neu.edu/home/stchang/pubs/ckg-popl2017.pdf)
* [Compositional Explanation of Types and Algorithmic Debugging of Type Errors \(2001\)](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.25.818)
* [Christian Williams: Structural types for algebraic theories \(2020\)](https://www.youtube.com/watch?v=aJyxtUopJ74)
* [Peter LeFanu Lumsdaine, What are we thinking when we present a type theory? \(2020\)](https://www.youtube.com/watch?v=kQe0knDuZqg)
* [Mathematics in type theory \(2020\)](https://xenaproject.wordpress.com/2020/06/20/mathematics-in-type-theory/) \([HN](https://news.ycombinator.com/item?id=23612856)\)
* [Division by zero in type theory: a FAQ \(2020\)](https://xenaproject.wordpress.com/2020/07/05/division-by-zero-in-type-theory-a-faq/) \([HN](https://xenaproject.wordpress.com/2020/07/05/division-by-zero-in-type-theory-a-faq/)\)
