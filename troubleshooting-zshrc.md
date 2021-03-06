## Installation

Follow this Gist and remember to log off/ log in after the install; otherwise zsh won't work.

https://gist.github.com/tsabat/1498393

## Timing a slow terminal start

- Add this on line one of .zshrc: `zmodload zsh/zprof` this file.
- Add this on last line of .zshrc: `zprof`

## Syntax highlighting

```
# Syntax highlighting fails when tabbing on an incomplete command e.g. with:

➜  k8s-
➜  ~ _fizsh-expand-or-complete-and-highlight:2: command not found: _zsh_highlight_highlighter_brackets_paint
_fizsh-expand-or-complete-and-highlight:3: command not found: _zsh_highlight_highlighter_main_paint
_fizsh-expand-or-complete-and-highlight:4: command not found: _zsh_highlight_highlighter_cursor_paint
_fizsh-expand-or-complete-and-highlight:5: command not found: _zsh_highlight_highlighter_pattern_paint
_fizsh-expand-or-complete-and-highlight:6: command not found: _zsh_highlight_highlighter_root_paint
```

This is because the `zsh-syntax-highlighting` module is not installed;

To fix it, you need to install this module within your `/home/<your-user>/.oh-my-zsh/plugins` folder as per the install instructions:

https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md#in-your-zshrc
