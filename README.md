# flycheck-title
[![MELPA](http://melpa.org/packages/flycheck-title-badge.svg)](http://melpa.org/#/flycheck-title)

![screenshot](flycheck_title.png)

flycheck-title lets you view flycheck messages in the frame title,
keeping the minibuffer free for other things.

## Existing approaches

Flycheck shows errors in the minibuffer by default. However, if
you're also using eldoc, you can get flicker:

![flicker](eldoc_conflict.gif)

An alternative is
[flycheck-pos-tip](https://github.com/flycheck/flycheck-pos-tip),
which shows the errors in a pop-up. This can be problematic when
you're using completion pop-ups:

![overlapping](overlapping_popups.png)

## How do I install it?

Install from MELPA, then add the following to
your Emacs configuration:

``` emacs-lisp
(with-eval-after-load 'flycheck
  (flycheck-title-mode))
```
