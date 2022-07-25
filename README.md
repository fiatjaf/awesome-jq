Awesome jq [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) [<img src="https://stedolan.github.io/jq/jq.png" width="200" align="right" alt="./jq">](https://github.com/stedolan/jq)
========================================================================

A curated list of awesome things built with the JSON processor and
_turing-complete functional language_ **jq**.

* [Awesome **jq**](#awesome-jq)
  * [Tools](#tools)
  * [Documentation](#documentation)
  * [Use Cases](#use-cases)
  * [Libraries and tools for jq itself](#libraries-and-tools-for-jq-itself)
  * [External libraries](#external-libraries)
  * [Contribute](#contribute)
  * [License](#license)

----


Tools
------------------------------------------------------------------------

_**jq**-based JSON visualizers and explorers_.

### Command-line

* [jq](https://stedolan.github.io/jq/) ([github](https://github.com/stedolan/jq)) &ndash; **jq** itself, the command-line JSON processor.
* [gojq](https://github.com/itchyny/gojq) &ndash; A _full_ **jq** implementation in Go (yes), also usable as a library.
* [jaq](https://lib.rs/crates/jaq) &ndash; A **jq** implementation in Rust that misses some small features but is often more correct than the original.
* [faq](https://github.com/jzelinskie/faq) &ndash; CLI program that processes BSON, Bencode, JSON, TOML, XML, YAML using **libjq**.
* [jiq](https://github.com/fiatjaf/jiq) &ndash; A visual command-line interactive JSON explorer with **jq** filters.
* `echo '' | fzf --print-query --preview "cat *.json | jq {q}"` &ndash; An [fzf](https://github.com/junegunn/fzf) hack that turns it into an interactive **jq** explorer.
* [jqq](https://github.com/jcsalterego/jqq/) &ndash; A visual command-line interactive **jq** explorer written in Ruby.
* [yq](https://github.com/kislyuk/yq) (and `xq`) &ndash; **jq** wrapper for YAML and XML documents.
* [yiq](https://github.com/zoetrope/yiq) &ndash; Like `jiq`, but using `yq` instead, so it supports YAML documents.
* [ijq](https://github.com/fiatjaf/ijq) &ndash; **jq** REPL with automatic variable assignment and global statements support.
* [jqsh](https://github.com/bmatsuo/jqsh) &ndash; An interactive wrapper written in Go.
* [jq-zsh-plugin](https://github.com/reegnz/jq-zsh-plugin) zsh line editor for constructing jq queries interactively.
* [fq](https://github.com/wader/fq) &ndash; jq for binary formats
* [jq-fish-plugin](https://github.com/jihchi/jq-fish-plugin) &ndash; Inspired by [jq-zsh-plugin](https://github.com/reegnz/jq-zsh-plugin), interactively build jq expressions in fish shell.

### Web

* [jiq-web](https://jq.alhur.es/jiq/) ([github](https://github.com/fiatjaf/jiq-web)) &ndash; jiq, but in a web page.
* [jq play](https://jqplay.org/) ([github](https://github.com/jingweno/jqplay)) &ndash; A playground for **jq** with sharing capabilities.
* [jq kung fu](https://www.jqkungfu.com/) &ndash; A **jq** playground in WebAssembly powered by the original **jq** compiled with _emscripten_.
* [jq-finder](https://jq.alhur.es/finder/) ([github](https://github.com/fiatjaf/jq-finder)) &ndash; A multipanel, Finder-like, JSON explorer with **jq** filters instead of paths.
* [jqaas](https://github.com/captn3m0/jqaas) &ndash; **jq** as a service, an open HTTP endpoint that executes **jq** queries.
* [jqp](https://github.com/sighrobot/jqp) &ndash; A free serverless proxy for filtering JSON and CSV data using **jq**.

### Desktop

* [jqi](https://nire0510.github.io/jqi/) ([github](https://github.com/nire0510/jqi)) &ndash; The almighty **jq** processor wrapped in a graphical UI, for Mac OSX.
* [jqview](https://github.com/fiatjaf/jqview) &ndash; A **jq** JSON explorer with a minimalist native GUI.

### Extensions

* [bro/q](https://github.com/zalando-incubator/bro-q) &ndash; A Chrome Extension for JSON formatting and **jq** filtering.
* [virtual-json-viewer](https://github.com/paolosimone/virtual-json-viewer) &ndash; A JSON Chrome/Firefox Extension with virtual DOM, full-text search and **jq** filtering.
* [atom-jq](https://github.com/sanack/atom-jq) &ndash; Interactive **jq** playground inside the Atom editor.
* [jq-mode](https://github.com/ljos/jq-mode) &ndash; A **jq** mode for Emacs.
* [vscode-jq](https://github.com/andricDu/vscode-jq) &ndash; A **jq** extension for VS Code.
* [vscode-jq-playground](https://github.com/davidnussio/vscode-jq-playground) &ndash; A **jq** playground notebook extension for VS Code.
* [vim-jqplay](https://github.com/bfrg/vim-jqplay) &ndash; Interactive **jq** playground inside Vim.
* `:%!jq '.'` is a Vim command that formats JSON in-place with **jq** (beware of any other tricks you might be thinking of).
* [@runjqbot](https://github.com/fiatjaf/runjqbot) &ndash; A Telegram bot that executes arbitrary **jq** code.


Documentation
------------------------------------------------------------------------

_Readings about **jq**_.

### Core documentation

* [Manual](https://stedolan.github.io/jq/manual/) &ndash; **jq** manual (development version).
* [FAQ](https://github.com/stedolan/jq/wiki/FAQ) &ndash; **jq** FAQ.
* [Cookbook](https://github.com/stedolan/jq/wiki/Cookbook) &ndash; **jq** cookbook.
* [Advanced Topics](https://github.com/stedolan/jq/wiki/Advanced-Topics) &ndash; **jq** advanced topics.

### Good small specific tutorials

* [Bash that JSON (with jq)](http://blog.librato.com/posts/jq-json).
* [JSON on the command line with jq](https://shapeshed.com/jq-json/).
* [Reshaping JSON with jq](https://programminghistorian.org/en/lessons/json-and-jq).
* [jq is sed for JSON](https://robots.thoughtbot.com/jq-is-sed-for-json).
* [Mastering jq: part 1](https://codefaster.substack.com/p/mastering-jq-part-1-59c)
* [An Introduction to JQ](https://earthly.dev/blog/jq-select/)

### Code examples

* [jq at Rosetta Code](http://rosettacode.org/wiki/Category:Jq) &ndash; Dozens of algorithms written in **jq** .
* [Builtins](https://github.com/stedolan/jq/blob/master/src/builtin.jq) &ndash; **jq** builtins coded in _jq_ itself, not C.


Use Cases
------------------------------------------------------------------------

_Apps using **jq** in the wild_.

* [jqmd](https://github.com/bashup/jqmd) &ndash; A "literate devops" tool that allows embedding jq code, shell scripts, YAML, and JSON in a markdown document and making it executable. (A bit like R markdown or IPython notebooks, except with shell/jq/YAML/JSON, and as a CLI scripting tool rather than a GUI.)
* [sc](https://github.com/annacrombie/sc) &ndash; A lightweight [SoundCloud](https://soundcloud.com/) client, with a composable api, powered by **jq**.
* [jc](https://github.com/kellyjonbrazil/jc) &ndash; CLI tool that converts the output of popular command-line programs and filetypes to JSON so they can be piped to **jq**.
* [@incomingnotificationbot](https://t.me/incomingnotificationbot) &ndash; A [Telegram](https://telegram.org/) bot that gives you HTTP endpoints and notifies you when a webhook arrives, filtering and formatting content with **jq**.
* [jqt](https://fadado.github.io/jqt/index.html) ([github](https://github.com/fadado/jqt)) &ndash; A web template engine that uses **jq** as expression language.
* [Vudash](https://vudash.com/#/transformers/?id=jq-transformer-vudashtransformer-jq) &ndash; A flexible and JSON-powered configurable open-source dashboard with support for a **jq** transformer.
* [datasette-jq](https://github.com/simonw/datasette-jq) &ndash; A plugin that enables **jq** queries on JSON columns on [datasette](https://datasette.readthedocs.io/) deployments.
* [jtool](https://github.com/fadado/jtool) &ndash; **jq**-based JSON tools for a modern shell.
* [just-dashboard](https://kantord.github.io/just-dashboard/) &ndash; A serverless app for implementing JSON-powered dashboards with JSON or YAML files (and **jq** filters as strings) serving as the only source of configuration.
* [bf.jq](https://github.com/MakeNowJust/bf.jq) &ndash; A Brainfuck interpreter written in **jq**.
* [jq-voronoi](https://github.com/hosuaby/jq-voronoi) &ndash; Implementation of Fortune’s algorithm to calculate Voronoi diagram on **jq**.
* [etleneum](https://etleneum.com/) &ndash; A centralized smart contract platform that works with sats and uses **jq** for easing the life of clients that want to fetch JSON states.

Libraries and tools for jq itself
------------------------------------------------------------------------

_Incrementing **jq** capabilities_.

* [jqnpm](https://joelpurra.com/projects/jqnpm/) ([github](https://github.com/joelpurra/jqnpm)) &ndash; A **jq** package manager that installs modules from GitHub and runs **jq** scripts.
* [JBOL](https://github.com/fadado/JBOL) &ndash; A collection of utility modules for **jq** (math, prelude, set, string etc.).
* [bigint](https://github.com/joelpurra/jq-bigint), [array](https://github.com/joelpurra/jq-disarray), [string](https://github.com/joelpurra/jq-stress) and [other libraries](https://github.com/joelpurra?utf8=%E2%9C%93&tab=repositories&q=jq) &ndash; **jq** libraries from the author of jqnpm.


External libraries
------------------------------------------------------------------------

_Using **jq** from other languages_.

* [gojq](https://github.com/itchyny/gojq) &ndash; A _full_ **jq** implementation in Go, usable either as a library or as a standalone CLI.
* [jq-web](https://github.com/fiatjaf/jq-web) &ndash; **jq** itself compiled to JavaScript with _emscripten_. There's also an alternative at [jqdash](https://www.npmjs.com/package/jqdash).
* [jq-go](https://github.com/threatgrid/jq-go) &ndash; Golang cgo bindings for **libjq** ([jqpipe-go](https://github.com/threatgrid/jqpipe-go) is a CLI wrapper from the same people).
* [libjq-go](https://github.com/flant/libjq-go) &ndash; Golang cgo bindings for **libjq**. This one works with recent versions of **jq**: 1.5, 1.6+.
* [node-jq](https://github.com/sanack/node-jq) &ndash; A **jq** wrapper for Node.js.
* [ruby-jq](https://github.com/winebarrel/ruby-jq) &ndash; A **jq** wrapper for Ruby.
* [pyjq](https://github.com/doloopwhile/pyjq) &ndash; A **jq** wrapper for Python.
* [jq.py](https://github.com/mwilliamson/jq.py) &ndash; Another **jq** wrapper for Python.
* [php-ext-jq](https://github.com/kjdev/php-ext-jq) &ndash; PHP extension for **jq**.
* [java-jq](https://github.com/arakelian/java-jq) &ndash; A **jq** wrapper for Java ([jackson-jq](https://github.com/eiiches/jackson-jq) is a Jackson extension).
* [jqr](https://github.com/ropensci/jqr) &ndash; R interface to **jq**.
* [Ansible jq](https://github.com/moreati/jq-filter) &ndash; A **jq** filter for [Ansible](https://ansible.com) configuration manager.


Contribute
------------------------------------------------------------------------

Please contribute! Open an issue or a PR and we’ll discuss it or merge it. If
you’re opening a PR, please ensure all formatting is ok (if you’re in a hurry
just open an issue).


License
------------------------------------------------------------------------

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
