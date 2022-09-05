# flycheck-credo

[flycheck][] checker for [credo][]. This repository is forked version.


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

And you cann specify `--checks-with-tag` argument.

```elisp
(setq flycheck-elixir-credo-checks-with-tag "target")
```

## Thanks

* [@rrrene][] for [credo][].
* [@lunaryorn][] for [flycheck][].

[flycheck]: http://www.flycheck.org/
[credo]: https://github.com/rrrene/credo
[@rrrene]: https://github.com/rrrene
[@lunaryorn]: https://github.com/lunaryorn
[Melpa]: http://melpa.milkbox.net/
