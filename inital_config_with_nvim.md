<h1>Install Ubuntu</h1> 
Terminal on Ubuntu to run following cmd:

sudo apt update
sudo apt upgrade
sudo apt install openssh-server
sudo systemctl status ssh
ip a => check ip.


Iterms on Macos or Xshell on Win10,
should be able to connect now.
If not working so far:
sudo ufw allow ssh

sudo apt-get install python3-pip
sudo apt install git-all
sudo apt install python3-venv

sudo apt install vim
<h1>NVIM</h1>   
Install the NeoVim AppimagePermalink
Download and install the appimage, use the output-document option to rename it to nvim:

wget --quiet https://github.com/neovim/neovim/releases/download/nightly/nvim.appimage --output-document nvim
Set the owner to root, and make nvim accessible to all users:

chmod +x nvim
sudo chown root:root nvim
Move the binary file to /usr/bin:

sudo mv nvim /usr/bin
Move into your home directory and create the subfolder structure to store the configuration file:

cd ~
mkdir -p .config/nvim

sudo apt install curl

# PLUGIN   INSTALL
curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim


# python support
pip3 install --user neovim
sudo apt-get install vim
ln -s ~/.vim ~/.config/nvim
ln -s ~/.vimrc ~/.config/nvim/init.vim

If autoload folder not exist, reinstall Plugin

 @@@@@@ might need to CREATE ~/.vimrc.@@@@@


----------------------------------------------------------
for file .vimrc

syntax on
call plug#begin()
Plug 'roxma/nvim-completion-manager'
Plug 'SirVer/ultisnips'
Plug 'honza/vim-snippets'
Plug 'morhetz/gruvbox'
call plug#end()

set background =dark
colorscheme gruvbox


