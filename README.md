# magit-find-file

[magit](https://github.com/magit/magit) powered equivalent of
TextMate's `cmd-t` functionality (or
[ctrlp.vim](https://github.com/kien/ctrlp.vim), if that's your bag).

Depends on Magit.

## Installation

Install it from [Melpa](http://melpa.milkbox.net/), or drop
`magit-find-file.el` into your load path and add:

```emacs
(require 'magit-find-file)
```

into your `init.el`. The Melpa version uses `autoload`, so once
installed you won't need to add anything to your `init.el`.

## Finding files

Invoking `magit-find-file-completing-read` will give you a list of
candidates as ascertained by `git ls-files`. So basically all the
files you should care about. It includes staged and not-yet-added
files in the list.

You may want to add it as a key command:

```emacs
(global-set-key (kbd "C-c p") 'magit-find-file-completing-read)
```

## Contributors

- [@chmouel](https://github.com/chmouel)
- [@tarsius](https://github.com/tarsius)

## Licence

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or (at
your option) any later version.

This program is distributed in the hope that it will be useful, but
WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
02110-1301, USA.
