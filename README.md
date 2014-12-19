vim-php-dictionary
==================

This is not a script, but a building stone for a script.
Although of minor significance, it may be useful to someone.

Learn about the use of dictionaries in general and you will - as a PHP programmer - be able to use this.

It's forked original plugin that a mirror of http://www.vim.org/scripts/script.php?script_id=534

What differense to original plugin ?
------------------------------------

* It's Maintenanced for the PHP latest version
* It's be Easy installation using plugin manager ([neobundle.vim][], [vundle][], [vim-pathogen][], ...)

Installation
------------

### Using [neobundle.vim][]

for master as PHP latest Version

```vim
set nocompatible               " Be iMproved
if has('vim_starting')
   set runtimepath+=~/.vim/bundle/neobundle.vim/
endif

call neobundle#rc(expand('~/.vim/bundle/'))

" Let NeoBundle manage NeoBundle
NeoBundleFetch 'Shougo/neobundle.vim'


" Declare the vim-php-dictionary
NeoBundle 'nishigori/vim-php-dictionary'


filetype plugin indent on     " Required

" Installation check.
NeoBundleCheck
```

Specified PHP version (either one):

```vim
" For PHP-5.5
NeoBundle 'nishigori/vim-php-dictionary', 'php5.4'
" For PHP-5.4
NeoBundle 'nishigori/vim-php-dictionary', 'php5.4'
" For PHP-5.3
NeoBundle 'nishigori/vim-php-dictionary', 'php5.3'
```

### Using [vim-pathogen][]

```sh
cd ~/.vim/bundle
git clone git://github.com/nishigori/vim-php-dictionary.git
```

[neobundle.vim]:    https://github.com/Shougo/neobundle.vim
[vundle]:           https://github.com/gmarik/vundle
[vim-pathogen]:     https://github.com/tpope/vim-pathogen
