This is a simple plugin that highlights operator characters for every language.
I want characters like `+,-,/,*,.,:,=` etc. highlighted in every programming
language I write, so I (Val Markovic) wrote this simple script.

Set the highlight color of the operators using `OperatorChars`

_Example:_
```
  highlight OperatorChars ctermfg=red guifg=red 
```

You can also configure the plugin to ignore certain filetypes and thus not
highlight operators in them. This is done by adding a new key to the
`g:ophigh_filetypes_to_ignore` dictionary (with whatever value you want, only
the key needs to be present). For example:
`g:ophigh_filetypes_to_ignore.markdown = 1`.

If you add that to your vimrc, then markdown files will be ignored. NOTE: the
key needs to be the filetype, not the extension! You can get the filetype of the
current file in Vim with `:set filetype?`.

