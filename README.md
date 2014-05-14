# The Clojure Code Translation Suite


DITA documentation (eventually, maybe) for:

* [clojure/tools.analyzer](https://github.com/clojure/tools.analyzer) An analyzer for Clojure code, written in Clojure and producing AST in EDN
* [clojure/tools.analyzer.jvm](https://github.com/clojure/tools.analyzer.jvm) jvm-specific passes for tools.analyzer
* [clojure/tools.emitter.jvm](https://github.com/clojure/tools.emitter.jvm) A JVM bytecode generator for ASTs compatible with tools.analyzer(.jvm)
* [clojure/tools.reader](https://github.com/clojure/tools.reader) A complete Clojure reader and an EDN-only reader, works with Clojure versions >= 1.3.0
* [clojure/jvm.tools.analyzer](https://github.com/clojure/jvm.tools.analyzer) Clojure's analysis compilation phase holds rich information about Clojure forms, like type/reflection information.  jvm.tools.analyzer provides an interface to this phase, callable a la carte. The output is similar to ClojureScript's analyzer.
* [clojure/core.match](https://github.com/clojure/core.match)
* [clojure/core.unify](https://github.com/clojure/core.unify)

With some remarks on related tools:

* [instaparse](https://github.com/Engelberg/instaparse) Instaparse aims to be the simplest way to build parsers in Clojure.
* [parsely](https://github.com/cgrand/parsley)  a DSL for creating total and truly incremental parsers in Clojure
* [Parse-EZ](https://github.com/protoflex/parse-ez) Parse-EZ is a parser library for Clojure programmers. It allows easy mixing of declarative and imperative styles and does not require any special constructs, macros, monads, etc. to write custom parsers. All the parsing is implemented using regular Clojure functions.
* [clearly](https://github.com/mthvedt/clearley)
* [clj-antlr](https://github.com/aphyr/clj-antlr) Clojure bindings for the ANTLR 4 parser
* [lein-antlr](https://github.com/alexhall/lein-antlr)


and some members of the parser combinator cottage industry inspired by
[Haskell's Parsec library](http://www.haskell.org/haskellwiki/Parsec).

* [parsatron](https://github.com/youngnh/parsatron) Clojure parser combinators.  Born from Haskell's Parsec library, The Parsatron is a functional parser library. The Parsatron provides a lot of very small functions that can be combined into larger ones to very quickly write parsers for languages.
* [parsero](https://github.com/alejandrogomez/parsero) Parser combinator library inspired by Haskell's Parsec.  parsero makes parsers first-class entities and provides a set of combinators for deriving new parsers out of existing ones. A few primitive parsers are included for convenience, too.
* [kern](https://github.com/blancas/kern) Kern is a library of parser combinators for Clojure. It is useful for implementing recursive-descent parsers based on predictive LL(1) grammars with on-demand, unlimited look-ahead. The inspiration for Kern comes from Parsec, a Haskell library written by Daan Leijen, and from work by Graham Hutton, Erik Meijer, and William Burge.
* [zetta-parser](https://github.com/van-clj/zetta-parser)
* [parsec](https://github.com/xudifsd/parsec)
* [clarsec](https://github.com/mmikulicic/clarsec)

and some PEG (Parsing Expression Grammar) parsers:

* [squarepeg](https://github.com/ericnormand/squarepeg)
* [amotoen](https://github.com/richard-lyman/amotoen)
* [dj.peg](https://github.com/bmillare/dj.peg)
* [clj-peg](https://github.com/Hercynium/clj-peg)
* [clj-peg](http://lithinos.com/clj-peg/) a different clj-peg


## building the docs

DITA-OT cmd:

    ant -Dargs.input=/Users/gar/dev/doc/doc.parsing/parsing.ditamap -Doutput.dir=/Users/gar/dev/doc/doc.tools.analyzer/target -Dtranstype=pdf
