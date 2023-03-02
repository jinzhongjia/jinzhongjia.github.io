---
layout: post
title: Emacs Config
date: 2023-03-02 19:28:20
tags:
    - emacs
    - linux
---

# Preface

Recently, I learned `emacs` and elisp, this article records the problems I encountered during using.

Some learning data:

- [Elisp Tutorial](https://www.codeplayer.org/Wiki/Emacs/elisp-tutorial.html)

## Boolean in `elisp`

In `elisp`, only nil is flase, others are true (including empty vector).

For convenience, we usually use t to represent true

## How to set custom virable file name

Just as this:

```lisp
;; set custom config file
(setq custom-file (expand-file-name "custom.el" user-emacs-directory))
;; auto load custom file
(when (file-exists-p custom-file)
  (load-file custom-file))
```

More to be added!