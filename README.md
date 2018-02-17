# Awesome jq [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) [<img src="https://stedolan.github.io/jq/jq.png" width="200" align="right" alt="./jq">](https://github.com/stedolan/jq)

A curated list of awesome things built with the JSON processor and _turing-complete functional language_ **jq**.

Inspired by the [awesome](https://github.com/sindresorhus/awesome) list.

* [Awesome jq](#awesome-jq)
  * [Tools](#tools)
  * [Use Cases](#use-cases)
  * [Libraries and tools for jq itself](#libraries-and-tools-for-jq-itself)
  * [External libraries](#external-libraries)
  * [Contribute](#contribute)
  * [Wrappers](#wrappers)

## Tools

_jq-based JSON visualizers and explorers_

**Command-line**
* [jq](https://stedolan.github.io/jq/) ([github](https://github.com/stedolan/jq)) - **jq** itself, the command-line JSON processor.
* [yq](https://github.com/kislyuk/yq) (and `xq`) - jq wrapper for YAML and XML documents.
* [ijq](https://github.com/fiatjaf/ijq) - jq REPL with automatic variable assignment and global statements support.
* [jqr](https://github.com/charlesetc/jqr) - A pure-bash jq REPL.
* [jiq](https://github.com/fiatjaf/jiq) - A visual command-line interactive JSON explorer with jq filters.

**Web**
* [jiq-web](https://jq.alhur.es/jiq/) ([github](https://github.com/fiatjaf/jiq-web)) - jiq, but in a web page.
* [jq play](https://jqplay.org/) ([github](https://github.com/jingweno/jqplay)) - A playground for jq with sharing capabilities.
* [jq-finder](https://jq.alhur.es/finder/) ([github](https://github.com/fiatjaf/jq-finder)) - A multipanel, Finder-like, JSON explorer with jq filters instead of paths.
* [jqaas](https://github.com/captn3m0/jqaas) - jq as a service, an open HTTP endpoint that executes jq queries.

**Desktop**
* [jqi](https://nire0510.github.io/jqi/) ([github](https://github.com/nire0510/jqi)) - The almighty jq processor wrapped in a graphical UI, for Mac OSX.

**Extensions**

* [atom-jq](https://github.com/sanack/atom-jq) - Interactive jq playground inside the Atom editor.

## Use Cases

_Apps using jq in the wild_

* [jqt](https://fadado.github.io/jqt/index.html) ([github](https://github.com/fadado/jqt)) - A web template engine that uses jq as expression language.
* [Vudash](https://vudash.com/#/transformers/?id=jq-transformer-vudashtransformer-jq) - A flexible and JSON-powered configurable open-source dashboard with support for a jq transformer.
* [jq-voronoi](https://github.com/hosuaby/jq-voronoi) - Implementation of Fortune's algorithm to calculate Voronoi diagram on jq.
* [bf.jq](https://github.com/MakeNowJust/bf.jq) - A Brainfuck interpreter written in jq.
* [just-dashboard](https://kantord.github.io/just-dashboard/) - A serverless app for implementing JSON-powered dashboards with JSON or YAML files (and jq filters as strings) serving as the only source of configuration.
* [jtool](https://github.com/fadado/jtool) - jq-based JSON tools for a modern shell.

## Libraries and tools for jq itself

_Incrementing jq capabilities_

* [jqnpm](https://joelpurra.com/projects/jqnpm/) ([github](https://github.com/joelpurra/jqnpm)) - a jq package manager that installs modules from GitHub and runs jq scripts.
* [JBOL](https://github.com/fadado/JBOL) - A collection of utility modules for jq (math, prelude, set, string etc.).
* [bigint](https://github.com/joelpurra/jq-bigint), [array](https://github.com/joelpurra/jq-disarray), [string](https://github.com/joelpurra/jq-stress) and [other](https://github.com/joelpurra?utf8=%E2%9C%93&tab=repositories&q=jq) jq libraries from the author of jqnpm.

## External libraries

_For using jq from other languages_

* [jackson-jq](https://github.com/eiiches/jackson-jq) - jq extension for the Java Jackson JSON Processor.
* [jq-web](https://github.com/fiatjaf/jq-web) - jq compiled to JavaScript with emscripten.
* [node-jq](https://github.com/sanack/node-jq) - A simple jq wrapper for Node.js.
* [ruby-jq](https://github.com/winebarrel/ruby-jq) - A humble jq wrapper for Ruby.
* [pyjq](https://github.com/doloopwhile/pyjq) - An honest jq wrapper for Python.
* [java-jq](https://github.com/arakelian/java-jq) - A lightweight jq wrapper for Java.
* [jqr](https://github.com/ropensci/jqr) - R interface to jq.
* [jq-in-the-browser](https://github.com/kantord/jq-in-the-browser) - early-stage jq port in pure JavaScript.

## Contribute
Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.

## License
[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
