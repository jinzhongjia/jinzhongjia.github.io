---
layout: post
title: Try migrating to wayfire 2
date: 2023-02-24 23:20:28
tags:
    - linux
---

## Preface

I have already migrate to wayfire, but I also have some other minor issues when using.

## Question

The following records the problems I encountered during use.

### `nm-connection-editor` doesn't save password ?

`nm-connection-editor` depends on gnome-keyring, but it's a bit heavy for `wm`, so I'm looking for a lighter alternative.

The solution now is to install two package called `gnome-keyring` and `libsecret`, and add `gnome-keyring-daemon --start` to sectin `autostart`.

Then, everything about network will work fines.

!!!!!!!!!!
More to be done!
!!!!!!!!!!
