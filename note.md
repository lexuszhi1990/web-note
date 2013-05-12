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

GEM: simple_form meta-tag
[SimpleForm](https://github.com/plataformatec/simple_form "official")
[MetaSearch](https://github.com/kpumuk/meta-tags "official")

4.25
----------
gmagick 

    [Install gmagick on Ubuntu](http://www.gerd-riesselmann.net/development/how-install-imagick-and-gmagick-ubuntu)
    Install pecl 
    sudo apt-get install php-pear php5-dev
    [CarrierWare-doc](http://carrierwave.rubyforge.org/rdoc/)
        resise_to_limit: Will only resize the image if it is larger than the specified dimensions.
        resize_to_fit: Resize the image to fit within the specified dimensions while retaining the original aspect ratio.
    
colorbox
    [colorbox](http://www.jacklmoore.com/colorbox/)
    [carrierwave](http://www.jacklmoore.com/colorbox/)

git-add
    git add -i [--interactive]
    git add -p [--patch]

5.2
-------------
git commit --amend 
    amend the last commit 

5.3
-------------
rake tasks
    [rake](http://erik.debill.org/2011/12/04/rake-for-rails-developers)
    [thesmallestrailsapp](http://thesmallestrailsapp.com/)
    [single-table-inheritance](http://blog.thirst.co/post/14885390861/rails-single-table-inheritance)


5.5
--------------
git reset --soft HEAD^1
git commit --amend

5.11
-------------------
可以用下面的命令回到合并之前的状态：
git reset --hard HEAD

PS1:
------
export PS1="\[\033[00;31m\]\W \[\033[32;40m\]\$(parse_git_branch)$\[\033[00m\]"

5.12
ctrlp
    ctrl f / d / o
git reset --mixed br

gd: 跳转到局部变量的定义处；
gD: 跳转到全局变量的定义处，从当前文件开头开始搜索；
g;: 上一个修改过的地方；
g,: 下一个修改过的地方；
[[: 跳转到上一个函数块开始，需要有单独一行的{。
]]: 跳转到下一个函数块开始，需要有单独一行的{。
[]: 跳转到上一个函数块结束，需要有单独一行的}。
][: 跳转到下一个函数块结束，需要有单独一行的}。
[{: 跳转到当前块开始处；
]}: 跳转到当前块结束处；
[/: 跳转到当前注释块开始处；
]/: 跳转到当前注释块结束处；

ci', di', yi'：修改、剪切或复制'之间的内容。
ca', da', ya'：修改、剪切或复制'之间的内容，包含'。"" () [] {} <>

vim 自动补全
-----------
C-x C-s -- 拼写建议。
C-x C-v -- 补全vim选项和命令。
C-x C-l -- 整行补全。
C-x C-f -- 自动补全文件路径。弹出菜单后，按C-f循环选择，当然也可以按C-n和C-p。
C-x C-p 和C-x C-n -- 用文档中出现过的单词补全当前的词。直接按C-p和C-n也可以。
C-x C-o -- 编程时可以补全关键字和函数名啊。
C-x C-i -- 根据头文件内关键字补全。
C-x C-d -- 补全宏定义。
C-x C-n -- 按缓冲区中出现过的关键字补全。 直接按C-n或C-p即可。

vim 文件加解密
--------------
vim -x file: 开始编辑一个加密的文件。
:X -- 为当前文件设置密码。
:set key= -- 去除文件的密码。
这里是 滇狐总结的比较高级的vi技巧。

vim 文件的编码
---------------
:e ++enc=utf8 filename, 让vim用utf-8的编码打开这个文件。
:w ++enc=gbk，不管当前文件什么编码，把它转存成gbk编码。
:set fenc或:set fileencoding，查看当前文件的编码。
在vimrc中添加set
fileencoding=ucs-bom,utf-8,cp936，vim会根据要打开的文件选择合适的编码。
注意：编码之间不要留空格。 cp936对应于gbk编码。
ucs-bom对应于windows下的文件格式。

[Vim Notes](http://snails.github.io/2012/05/08/Learn-to-Markdown)
