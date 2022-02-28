# kak-k
A kakoune plugin for the [K programming language](https://k.miraheze.org).

Provides syntax highlighting, commands and some indentation, borrowed from the [BQN](https://github.com/mlochbaum/BQN) plugin.

Primarily targeted at [ngn/k](https://codeberg.org/ngn/k) but it will work with any K executable that supports `\l`.

# Requirements
- rlwrap
- `declare-option k_exec "<path-to-k>"` in kakrc

# Commands
- `k-repl`: Start a new K repl.
- `k-repl-from-selection`: Start a new K repl with the current selection executed in it.
- `k-execute-line`: execute the current line in a new K repl.
- `k-run-file`: Run the current file in a new K repl.
