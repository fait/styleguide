# fait Styleguide

Style rules to encourage clean, consistent makefiles.

## Variable naming

* Variables should be named in `param-case`
* Internal variables which are not intended to be modified by your module's users should be prefixed with `~`
* Modules should prefix their variables with a short string unique to the module

## Functions

* Functions are variables intended to be used with `eval` and/or `call`
* Functions should be written with `define`, even if they are only one line
* `define` lines must not contain a variable assignment operator (i.e. `=`, `:=`)

## Rules

* Avoid double-colon explicit rules. If you really need them, write a comment explaining when the rule will run and what other rules have the same target (and will thus run at the same time).

## Whitespace

* `=` and `:=` must be surrounded by whitespace
* `:` in rule definitions must be followed by whitespace and must not be preceded by whitespace
* `::` in rule definitions must be surrounded by whitespace
