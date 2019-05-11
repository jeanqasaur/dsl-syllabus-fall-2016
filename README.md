# Domain-Specific Languages Syllabus

Something I spend a lot of time thinking about is how to use the right tool for the task, in programming and otherwise. It was this, rather than a love for logic or formal semantics, that made me fall in love with the study of programming languages. (Although I did go to logic summer camp as a kid...) For this reason, I strongly believe that every programming language is a domain-specific language and we should regard and evaluate languages through the lenses of their domains.

When I first joined Carnegie Mellon University as an Assistant Profesor, I had the luxury of designing a PhD seminar on any topic of my choosing. What I wanted to do was to give students a tour of how I think about designing and implementing programming languages, with the view that we're looking at each language in the context of its domain. Here is the syllabus for my [advanced topics domain-specific languages course](http://www.cs.cmu.edu/~jyang2/courses/fall16/15819/) at CMU, fall 2016.

Since people have been asking about the reading list, I thought I'd post it here. I hope it's a useful resource for people hoping to get a broader context for thinking about programming languages and language design.

## Unit 1: Why domain-specific languages?
* **To make things pretty.** We look at how DSLs improve functional reactive programming.
   * [ELM: Concurrent FRP for Functional GUI](http://people.seas.harvard.edu/~chong/pubs/pldi13-elm.pdf)
   * [Flapjax: A Programming Language for Ajax Applications](http://www.cs.brown.edu/~sk/Publications/Papers/Published/mgbcgbk-flapjax/)
* **To make things fast.** We look at DSLs for high-performance computing in graphics.
   * [Halide: A Language and Compiler for Optimizing Parallelism, Locality, and Recomputation in Image Processing Pipelines](http://people.csail.mit.edu/jrk/halide-pldi13.pdf)
* **To make things correct.** We look at the specification and verification of software-defined networks.
   * [NetKAT: semantic foundations for networks](http://dl.acm.org/citation.cfm?id=2535862)
   * [Frenetic: A High-Level Language for OpenFlow Networks](http://frenetic-lang.org/publications/frenetic-presto10.pdf)
   * [Machine-Verified Network Controllers](http://frenetic-lang.org/publications/verified-pldi13.pdf)
* **Some combination of the above.** We look at languages for scientific programming.
   * [Terra: A Multi-Stage Language for High-Performance Computing](http://terralang.org/pldi071-devito.pdf)
   * [Julia talk: "Solving the Two-Language Problem"](https://www.youtube.com/watch?v=B9moDuSYzGo)
   * [Cython: C-Extensions for Python](http://cython.org/)
* **Analyzing programs for interesting properties.** We look at how Resource-Aware ML can give us bounds we never previously dreamed of.
   * [Resource Aware ML](http://www.cs.cmu.edu/~janh/papers/hah12cav.pdf)
   * [End-to-End Verification of Stack-Space Bounds for C Programs](http://www.cs.cmu.edu/~janh/papers/veristack2014.pdf)
   
## Unit 2: How to build domain-specific languages?
* **Embedding languages into other languages.** Making languages gets easier and easier as we can just hijack the machinary from another language. We look at how to make EDSLs in Ruby, Scala, and Haskell.
   * [Building Embedded Systems with Embedded DSLs](https://www.cs.indiana.edu/~lepike/pubs/embedded-experience.pdf)
   * [Contracts for Domain-Specific Languages in Ruby](http://www.cs.umd.edu/~jfoster/papers/dls12.pdf)
   * [Safely Composable Type-Specific Languages](https://github.com/wyvernlang/docs/raw/master/ecoop14/ecoop14.pdf)			
* **Implementing standalone DSLs.** A closer look at LLVM and other techniques.
   * [LLVM chapter of open source book](http://www.aosabook.org/en/llvm.html)
   * [LLVM Tutorial](http://llvm.org/docs/tutorial/index.html)				
* **Staging.** We look at meta-programming techniques that can help with implementing DSLs.
   * [A Gentle Introduction to Multi-stage Programming](https://www.cs.rice.edu/~taha/publications/journal/dspg04a.pdf)
   * [Lightweight Modular Staging: A Pragmatic Approach to Runtime Code Generation and Compiled DSLs](http://cacm.acm.org/magazines/2012/6/149801-lightweight-modular-staging/abstract)
   * [Functional Pearl: A SQL to C Compiler in 500 Lines of Code](https://www.cs.purdue.edu/homes/rompf/papers/rompf-icfp15.pdf)
* **Adding types to existing languages.** You don't even need to make a language to make a language! We look at typed scheme, gradual types, and languages that add more types to a language that already has types.
   * [Gradual Typing for Functional Languages](http://scheme2006.cs.uchicago.edu/13-siek.pdf)
   * [What is Gradual Typing](http://homes.soic.indiana.edu/jsiek/what-is-gradual-typing/)
   * [Hack and HHVM Manual](https://docs.hhvm.com/hack/types/annotations)
