# my-vim-config
Vim Configuration using vim-plug, dracula, nercommenter and others.

## Init
- Install: https://github.com/junegunn/vim-plug
- Create file: .vimrc
- Copy contetnt bellow in .vimrc
- Run vim command: `:PlugInstall`

## File .vimrc

    call plug#begin('~/.vim/plugged')

    Plug 'junegunn/vim-easy-align'
    Plug 'chiel92/vim-autoformat'
    Plug 'tpope/vim-fugitive'
    Plug 'scrooloose/nerdcommenter'
    Plug 'scrooloose/nerdtree'
    Plug 'dracula/vim', { 'as': 'dracula' }
    Plug 'itchyny/lightline.vim'
    Plug 'whatyouhide/vim-gotham'
    call plug#end()

    xmap ga <Plug>(EasyAlign)
    nmap ga <Plug>(EasyAlign)
    noremap <F3> :Autoformat<CR>

    filetype plugin on

    syntax on
    color dracula
    set number

    map <C-o> :NERDTreeToggle<CR> 
    set laststatus=2
    set noshowmode

## Notes:
- Nerd Commenter: `[\] + [c] +[space]`
- Numbers in vim: `:set nu`, `:set nonu`, `:set number`, `:set nonumber`  

## Install Oh-My-ZSH

See [this easy guide](https://github.com/jnfran92/my-vim-config.git)
