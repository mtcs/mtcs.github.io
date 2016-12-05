---
layout: post
title:  "Some Nice Vim Plugins"
date:   2016-11-17 18:45:00
categories: [news,blog]
---

I've been using Vim for a very long time now, so I think it would be a good thing to share the list plugins I use.

But fist, you should use something plugin management utility like Patogen or Vundle. I personally prefer Vundle since it handles plugin installation, load, update and cleaning. Unfortunelly you have to install it manually:

[https://github.com/VundleVim/Vundle.vim]()

Once Vundle is installed and configured, all you have to do is to include "Plugin" command in your .vimrc and run a :PluginInstall in order to include a plugin to your personal repository. It downloads the plugin directly from GitHub for you.

So, this is the list of plugins I am using now:

~~~~
Plugin 'Shougo/vimproc.vim'
Plugin 'scrooloose/nerdtree'
Plugin 'oplatek/Conque-Shell'
Plugin 'godlygeek/csapprox'
Plugin 'vim-scripts/AnsiEsc.vim'
Plugin 'scrooloose/syntastic'
Plugin 'Valloric/YouCompleteMe'
Plugin 'vim-scripts/taglist.vim'
Plugin 'bling/vim-bufferline'
Plugin 'powerline/powerline', {'rtp': 'powerline/bindings/vim/'}
Plugin 'tpope/vim-fugitive'
Plugin 'puppetlabs/puppet-syntax-vim'
Plugin 'rodjek/vim-puppet'
Plugin 'kien/ctrlp.vim'
Plugin 'godlygeek/tabular'
Plugin 'vim-scripts/DoxygenToolkit.vim'
Plugin 'jceb/vim-orgmode'
Plugin 'vim-scripts/utl.vim'
Plugin 'xuhdev/vim-latex-live-preview'
Plugin 'tpope/vim-dispatch'
Plugin 'tpope/vim-surround'
Plugin 'scrooloose/nerdcommenter'
~~~~

## File Browsing - Nerdtree

For file exploring inside VIM. It gives you a nice interface for browsing files and directories

~~~~
Plugin 'scrooloose/nerdtree'
~~~~

## Integrated Shell - Conque-Shell

It implements a shell interface inside VIM. Besides from usual shell usage, you can run blocks of code from other buffers, set to automatically run interpreters for types of files etc. It is particularly useful for testing interpreted languages on-the-fly like R, Python, Scala etc. you can also use to compile C/C++ code, but then you will not have access to the quickfix VIM offers you.

~~~~
Plugin 'oplatek/Conque-Shell'
~~~~

## Colors - Csapprox and AnsiESC

I don't know if Csapprox is really necessary nowadays, but if you are having problems with RGB hicolor inconsistency, this plugins solves just that. AnsiESC, in the other hand, helps when you open a file with Ansi color codes, interpreting them into color.

~~~~
Plugin 'godlygeek/csapprox'
Plugin 'vim-scripts/AnsiEsc.vim'
~~~~

## Syntactic Analysis - Syntastic and YouCompleteMe

While Synthastic highlights syntactic errors, YouCompleteMe does syntactic-aware completion. YCM needs to install more then just a VIM plugin, it uses a background daemon to compile code in real time, see their web page for more info.

~~~~
Plugin 'scrooloose/syntastic'
Plugin 'Valloric/YouCompleteMe'
~~~~

## Source code quick navigation - TagList

A classical source code navigation tool, it gives you a buffer much like Nerdtree, but with source tags, like: code function declarations etc.

~~~~
Plugin 'vim-scripts/taglist.vim'
~~~~

## Buffers and Status Line - BufferLine and PowerLine

While bufferline changes the statusline to show oppen buffers, Powerline does much much much more. Powerline overhauls all lines in vim (except command line) making it much nicer to look at. Also, Powerline also can improuve Bash, Zsh, Tmux and other applications status lines.

~~~~
Plugin 'bling/vim-bufferline'
Plugin 'powerline/powerline', {'rtp': 'powerline/bindings/vim/'}
~~~~

## Git Integration - Fugitive

Integrates with Git allowing for easier git status commits etc.

~~~~
Plugin 'tpope/vim-fugitive'
~~~~

## Puppet Integration

Well... better puppet integration...

~~~~
Plugin 'puppetlabs/puppet-syntax-vim'
Plugin 'rodjek/vim-puppet'
~~~~

## Buffer search - CTRL-P

Uses fuzzy search to find open buffers...

~~~~
Plugin 'kien/ctrlp.vim'
~~~~

## Table auto aligment - Tabular

Enables you to auto align characters in a buffer with "simple" commands.

~~~~
Plugin 'godlygeek/tabular'
~~~~

## Doxygen Integration - DoxygenToolkit

Helps with code commenting for Doxygen. It creates snippets for you!

~~~~
Plugin 'vim-scripts/DoxygenToolkit.vim'
~~~~

## Orgmode smart editing - vim-orgmode

For VIM fans jealous of the AWESOME Emacs Orgmode. It is NOT Emacs Orgmode, but it will get there some day... It helps you edit Orgmode files.

~~~~
Plugin 'jceb/vim-orgmode'
~~~~

## Latex Previewer - latex-live-preview

I swear I did not remember this plugin!!! :D It enables you to preview latex while you are editing it

~~~~
Plugin 'xuhdev/vim-latex-live-preview'
~~~~

## Enclosing helper - Sourround

Helps you to handle with enclosing text. Like "text text text"

~~~~
Plugin 'tpope/vim-surround'
~~~~

## NerdCommenter

Comment helper tool. With it you can comment blocks of code easier.

~~~~
Plugin 'scrooloose/nerdcommenter'
~~~~

