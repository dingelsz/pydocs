# pydocs

This project contains code for a pretty sweet python documentation workflow.

## Setup

Add the following to your `.emacs` file:
```
(load "/path/to/pydocs.el")
```

And create a new yasnippet:
```
# -*- mode: snippet -*-
# name: deff
# key: deff
# contributer: Zach Dingels
# --
def $1($2):
"""$1$0${2:$(if (not (string= yas-text \"\")) 
		(concat \"\\n\\n\" (make-docstring yas-text))
		"")}
"""
```

And your good to 
