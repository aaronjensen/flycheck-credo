# flycheck-credo

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

## Thanks

* [@rrrene][] for [credo][].
* [@lunaryorn][] for [flycheck][].

[flycheck]: http://www.flycheck.org/
[credo]: https://github.com/rrrene/credo
[@rrrene]: https://github.com/rrrene
[@lunaryorn]: https://github.com/lunaryorn
[Melpa]: http://melpa.milkbox.net/
