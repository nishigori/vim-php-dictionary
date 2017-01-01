vim-php-dictionary
==================

This is not a script, but a building stone for a script.
Although of minor significance, it may be useful to someone.

Learn about the use of dictionaries in general and you will - as a PHP programmer - be able to use this.

It's forked original plugin that a mirror of http://www.vim.org/scripts/script.php?script_id=534

What differense to original plugin ?
------------------------------------

* It's Maintenanced for the PHP latest version
* It's be Easy installation using plugin manager ([dein.vim][], [vundle][], [vim-pathogen][], ...)

Installation
------------

### Using [dein.vim][]

for master as PHP latest Version

```vim
" Prepare Instalattion:
"   1. curl https://raw.githubusercontent.com/Shougo/dein.vim/master/bin/installer.sh > installer.sh
"   1. sh ./installer.sh {specify the installation directory}

" Edit your .vimrc like this.
if &compatible
  set nocompatible
endif
set runtimepath+={path to dein.vim directory}

if dein#load_state({path to plugin base path directory})
  call dein#begin({path to plugin base path directory})

  call dein#add('nishigori/vim-php-dictionary', {'on_ft': 'php'})
  ...

  call dein#end()
  call dein#save_state()
endif

filetype plugin indent on
syntax enable

" Open vim and install dein
" :call dein#install()
```

Specified PHP version (either one):

```vim
" For PHP-7.1
call dein#add('nishigori/vim-php-dictionary', {'on_ft': 'php', 'rev': 'php7.1'})
" For PHP-7.0
call dein#add('nishigori/vim-php-dictionary', {'on_ft': 'php', 'rev': 'php7.0'})
" For PHP-5.6
call dein#add('nishigori/vim-php-dictionary', {'on_ft': 'php', 'rev': 'php5.6'})
" For PHP-5.5
call dein#add('nishigori/vim-php-dictionary', {'on_ft': 'php', 'rev': 'php5.5'})
" For PHP-5.4
call dein#add('nishigori/vim-php-dictionary', {'on_ft': 'php', 'rev': 'php5.4'})
" For PHP-5.3
call dein#add('nishigori/vim-php-dictionary', {'on_ft': 'php', 'rev': 'php5.3'})
```

### Using [vim-pathogen][]

```sh
cd ~/.vim/bundle
git clone git://github.com/nishigori/vim-php-dictionary.git
git checkout -b ${PHP_VERSION_U_WANT} origin/${PHP_VERSION_U_WANT}
```

[dein.vim]:         https://github.com/Shougo/dein.vim
[vundle]:           https://github.com/gmarik/vundle
[vim-pathogen]:     https://github.com/tpope/vim-pathogen
