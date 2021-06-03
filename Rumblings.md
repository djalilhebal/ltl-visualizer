# Rumblings

Rumblings about `ltl-visualizer`.


## Cheatsheet

 Name            | TINA  | LaTeX         | Quickstrom keyword
-----------------|-------|---------------|--------------------
always (_G_)     | `[]`  | `\Box`        | **always**
next   (_X_)     | `()`  | `\bigcirc`    | **next**
finally (_F_)    | `<>`  | `\Diamond`    | **eventually**
until   (_U_)    | `U`   | `\mathcal{U}` | **until**
not              | `-`   | `\lnot`       | **not**
and              | `/\`  | `\land`       | **and**
or               | `\/`  | `\lor`        | **or**
implies          | `=>`  | `\implies`    | **implies**
is equivalent to | `<=>` | `\iff`        | _NOT IMPLEMENTED!_


## TODO

- [ ] `and` and `or` should throw if given `arguments.length !== 2`. (They are supposed to be binary operators.)

- [ ] Implement `iff`.

- [ ] Accept user-defined atomics other than the A-Z range.  
Maybe treat any non-keyword sequence of characters as an atomic proposition?

- [ ] Print the propositions that hold true on top of each state
([a la Wikipedia](https://en.wikipedia.org/wiki/Linear_temporal_logic#/media/File:Ltlrelease-stop.svg)).
Maybe show it only on hover or something.

---

Take my old shit and turn it into something useful...
https://djalil.me/shit/2018-09/lm-chap1/

```js
// Parse TINA syntax
// string -> Formula
function parseTina() {}

// to TeX syntax, for Mathjax KaTex
// Formula -> string
function toLatex() {}

// to HTML entities, as an alternative for TeX.
// Formula -> string
function toHtml() {}

// Formula -> string
function toQuickstrom() {}
```

---

FIN.
