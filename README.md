# kak-k
A kakoune plugin for the [K programming language](https://k.miraheze.org).

Provides syntax highlighting, commands and some indentation, borrowed from the [BQN](https://github.com/mlochbaum/BQN) plugin.

Primarily targeted at [ngn/k](https://codeberg.org/ngn/k) but it will work with any K executable that supports `\l`.

# Requirements
- rlwrap

# Commands
This plugin defines a new user mode(`:doc user-mode`) called `k`. You can enter the user mode and use the keybinds mentioned here.
I personally recommend adding `map global normal <c-k> ": enter-user-mode k<ret>"` to your kakrc. Replace `<c-k>` with a keybinding of choice.

If you do not have `declare-option k_exec "<path-to-k>"` in your kakrc, the plugin will assume `~/k/k` as the location of your K binary. 

- `k-repl` (`r`): Start a new K repl.
- `k-repl-from-selection` (`s`): Start a new K repl with the current selection executed in it.
- `k-execute-line` (`x`): execute the current line in a new K repl.
- `k-run-file` (`l`): Run the current file in a new K repl.
