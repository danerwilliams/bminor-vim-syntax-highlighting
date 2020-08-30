# Bminor syntax highlighting in vim

Simple syntax highlighter written in vimscript for the [Bminor language](https://www3.nd.edu/~dthain/courses/cse40243/fall2019/bminor.html).
This is a bit too little, too late as the [Compilers and Language Design](https://www3.nd.edu/~dthain/compilerbook/compilerbook.pdf)
course recently ended a few weeks prior to starting this. I had wanted to make this during the semester to make reading and writing Bminor code a bit
easier, but couldn't find the time to work on it. I figured I might as well make it now that I have time over winter break
so I can at least learn some more vimscript.

## Vundle Installation

If you use [vundle](https://github.com/VundleVim/Vundle.vim) then you can simple install by adding:  
`Plugin 'ginglis13/bminor-vim-syntax-highlighting'`  
to your .vimrc

## How to use it

You must have the `syntax` and 	`ftdetect` folders in the top level of your `~/.vim/` folder. `syntax` defines keywords and regular
expressions to match things like strings, operators, numbers, etc., and highlights them appropriately. This is doing a lot of the same
work as the [scanner](https://www3.nd.edu/~dthain/compilerbook/compilerbook.pdf#chapter.3) stage of the Bminor compiler.
`ftdetect` just checks a file's extension (`*.bminor`) and uses the appropriate highlighting.

vim reference docs: [http://vimdoc.sourceforge.net/htmldoc/syntax.html](http://vimdoc.sourceforge.net/htmldoc/syntax.html)

## Example

![](https://yld.me/raw/rnK.png)
