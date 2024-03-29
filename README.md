# ncm2-phpactor-workflow
My workflow for [ncm2](https://github.com/ncm2/ncm2) integration
with [phpactor](https://github.com/phpactor/phpactor)

In order to have Vim configuration a bit easier to compose I'll extract
configurations for specific plugins into "workflow plugins". So it's something
that make sense for the way that I'm working but that can be removed once
the plugin is not used anymore.

## How to use it
I recommend to use [Plug](https://github.com/junegunn/vim-plug) but can be
any vim package manager or git clone inside ~/.vim/autoload.

A quick/durty/easy way to install Plug is like this:
```bash
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

Then add this to you .vimrc
```vim
call plug#begin('~/.vim/my-stuff')
    Plug 'ncm2/ncm2'
    Plug 'roxma/nvim-yarp'
    Plug 'phpactor/ncm2-phpactor'
    Plug 'EHER/ncm2-phpactor-workflow'
call plug#end()
```
Reload .vimrc and `:PlugInstall` to install plugins.

Enjoy! ;)
