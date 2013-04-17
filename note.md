Markdown-link
-------------
[1]: http://daringfireball.net/projects/markdown/syntax "Daring"
[2]: http://markdown.tw/
- [Markdown-official][1]
- [Markdown-tx][2]
- [Notes](http://snails.github.io/2012/05/08/Learn-to-Markdown/)

Tmux copy
---------
* Ctrl-a + [        => try to select
* space             => start to copy
* Enter
* Ctrl-a + ]        => paste

Vim cml
-------
*`:set ft`* => check the filetype

surround-vim:
-------------
- dst  
- ds [ put in cml]

rails patial
------------
*   use V or v to choose code 
*   jump into cml (shift + :)
*   Rextract "name"

add public key
--------------
- ssh-keygen -t dsa
- sudo apt-get install xclip
- cat /home/jiesse/.ssh/id_dsa.pub | xclip -sel clip

2013.4.10




auto load .bashrc in ubuntu 
---------------
add ` source $HOME/.bashrc ` in '~/.bash_login'

skip log in console
----------
ActiveRecord::Base.logger = nil

todo
----------
GEM: rolify, sequel, meta_search
- The Database Toolkit for Ruby
- doc: http://rubydoc.info/gems/sequel/3.36.1/frames
- used in db migration task
gem 'sequel', '~> 3.36.1' # June 2, 2012

- Allows simple search forms to be created against an AR3 model and its associations, has useful view helpers for sort links and multiparameter fields as well.
- http://rubygems.org/gems/meta_search
gem "meta_search", "~> 1.1.3"


JS: easytabs
--------
[EasyTabs](http://os.alfajango.com/easytabs "official")


4.17
