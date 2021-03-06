
# My custom dotfiles for Linux and Mac

This repo contains my dotfiles and config files for Bash, ZSH, Git and Vim, for
Unix-ish systems.

## Download / Installation

Run
```
git clone --recurse-submodules https://github.com/DarthFloopy/mydotfiles.git`
```
to get all the files. Then, `cd` into the repo folder (`mydotfiles`) and run
```
`./install.sh [--shush]`
```
to copy files into your home directory. (The `--shush` option omits prompts and
friendly make-sure-you-pulled-the-latest-version reminders.) To pull updates,
run
```
git pull --recurse-submodules
```

 - When you're done, log out and back in to use the new config.
 - To use Vim plugins, follow the Vundle download prompt and plugin install
   instructions next time you start Vim. (I.e., hit enter to download Vundle and
   then run `:PluginInstall`.)
   - (The prompts I set up seem to be slightly broken now for some reason. Just
     run those commands and it will work.)
   - To use the CoC vim plugin, run `:CocInstall coc-marketplace` and then
     `:CocList marketplace`. Then search and navigate around, and hit enter to
     install language-specific plugins.
     - Useful CoC plugins include `coc-snippets` (for text snippets),
       `coc-tsserver` and `coc-json` (JS/TS), `coc-html` and `coc-emmet` (HTML)
       and `coc-metals` (Scala).
 

What is all this `--recurse-submodules` funny business, you ask? It's to
download any git submodules that this repo uses (e.g., ZSH or Vim plugins I got
from GitHub).

