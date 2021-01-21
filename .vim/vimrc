" Enable plugins
if empty(glob('$HOME/.vim/autoload/plug.vim'))
		  silent !curl -fLo $HOME/.vim/autoload/plug.vim --create-dirs
		          \ https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
		    autocmd VimEnter * PlugInstall --sync | source $MYVIMRC
	endif

call plug#begin('~/.config/nvim/plugged')

" ======== Plugins ========
Plug 'sainnhe/sonokai'
Plug 'sheerun/vim-polyglot'
Plug 'preservim/nerdtree'
Plug 'tiagofumo/vim-nerdtree-syntax-highlight'
Plug 'ryanoasis/vim-devicons'
Plug 'Xuyuanp/nerdtree-git-plugin'
Plug 'airblade/vim-gitgutter'
Plug 'scrooloose/syntastic'
Plug 'tpope/vim-surround'
Plug 'vim-airline/vim-airline'
Plug 'jiangmiao/auto-pairs'

call plug#end()

inoremap jk <ESC>

set tabstop=4

" Color theme
set termguicolors 
let g:sonokai_style='andromeda'
let g:sonokai_enable_italic=1
colorscheme sonokai

" Syntastic config
set statusline+=%#warningmsg#
set statusline+=%{SyntasticStatuslineFlag()}
set statusline+=%*

let g:syntastic_always_populate_loc_list = 1
let g:syntastic_auto_loc_list = 1
let g:syntastic_check_on_open = 1
let g:syntastic_check_on_wq = 0

" Toggle NERDTree
map <C-n> :NERDTreeToggle<CR>
let g:NERDTreeIgnore = ['^node_modules$']

" Show line numbers
set number

