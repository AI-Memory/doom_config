
//# for vterm compilation

sudo apt install cmake libtool libtool-bin

cd ~/.config/doom

git init

git remote add origin https://github.com/AI-Memory/doom_config.git

git pull

git checkout main -f

export GPG_TTY=$(tty)
# remove the emacs old-style configuraton folder
rm .emacs.d

# install the following servers in elisp

copilot server

lsp server
