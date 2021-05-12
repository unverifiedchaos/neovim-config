# neovim-config
my neovim configuration 


```
   1 set runtimepath+=~/.vim_runtime
   2 set number
   3 set background = "dark"
   4 
   5 nmap <F6> :NERDTreeToggle<CR>
   6 nmap v :vsp<CR>
   7 
   8 
   9 let g:rainbow_active = 1 
  10 let g:papaya_gui_color='blue'
  11 let g:snipMate={ 'snippet_version' : 1 }
  12 let g:onedark_hide_endofbuffer=1
  13 let g:onedark_termcolors=256
  14 let g:onedark_terminal_italics=1
  15 let g:NERDTreeWinPos = "left"
  16 let g:lightline={
  17   \ 'colorscheme': 'onedark',
  18   \ }
  19 
  20 let g:airline_theme='onedark'
  21 
  22 source ~/.vim_runtime/vimrcs/basic.vim
  23 source ~/.vim_runtime/vimrcs/filetypes.vim
  24 source ~/.vim_runtime/vimrcs/plugins_config.vim
  25 source ~/.vim_runtime/vimrcs/extended.vim
  26 
  27 call plug#begin('~/.vim/plugged')
  28 
  29 Plug 'luochen1990/rainbow'
  30 Plug 'HenryNewcomer/vim-theme-papaya'
  31 Plug 'scrooloose/nerdtree'
  32 Plug 'junegunn/vim-easy-align'
  33 Plug 'joshdick/onedark.vim'
  34 
  35 call plug#end()
  36 
  37 set guifont=Hack:h12
  38 syntax on
  39 colorscheme onedark
  40 set termguicolors
  41 
  42 try
  43 source ~/.vim_runtime/my_configs.vim
  44 catch
  45 endtry
~
~
~
```

# Activate my config using 
:source %
:PlugInstall
