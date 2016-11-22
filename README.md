# flycheck-credo [![MELPA](https://melpa.org/packages/flycheck-credo-badge.svg)](https://melpa.org/#/flycheck-credo)

[flycheck][] checker for [credo][].

## Installation

You can install this package from [Melpa][]

```
M-x package-install RET flycheck-credo RET
```

## Usage

Ensure that `credo` is installed in your project.

Then, in your `init.el`:

```elisp
(eval-after-load 'flycheck
  '(flycheck-credo-setup))
(add-hook 'elixir-mode-hook 'flycheck-mode)
```

## Options

You can tell flycheck-credo to call credo with the '--strict' argument.

```elisp
(setq flycheck-elixir-credo-strict t)
```

## Thanks

* [@rrrene][] for [credo][].
* [@lunaryorn][] for [flycheck][].

[flycheck]: http://www.flycheck.org/
[credo]: https://github.com/rrrene/credo
[@rrrene]: https://github.com/rrrene
[@lunaryorn]: https://github.com/lunaryorn
[Melpa]: http://melpa.milkbox.net/
