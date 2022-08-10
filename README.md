# My_Better_Terminal
enjoy my better terminal


# 纯净版
使用bash即可，需安装fzf，bat，ripgrep
`conda install -yc conda-forge fzf,bat,ripgrep` 

只需要添加.completion.bash，.fzf.bash至HOME目录即可(AllMy_config目录下)。

并在.bashrc中添加 source ~/.fzf.bash

## 纯净版功能
### ** 补全
tab键识别前置命令补全，支持
- 命令选项补全
- 路径补全 `cd **<tab>`
- 进程补全 `kill **<tab>`
- ssh补全 
- 所有命令输入文件补全 `command **<tab>`
- 等等

### CTRL+R 历史命令

### CTRL+T 文件检索


### CTRL+Y 目录切换

### 其余命令
`ff` 文件搜索
`fff` 内容搜索
`mkdircd` 创建目录并切换
`lc` 统计数目




## 完全版功能（集合了比较多的个人常用功能）
#### 主题
`ZSH_THEME="powerlevel10k/powerlevel10k"`
所有主题在.oh-my-zsh/themes，可自己定义。

#### 扩展
`plugins=(git z extract rand-quote zsh-autosuggestions zsh-syntax-highlighting fzf-tab)`
扩展详细可自己查询。
z：快捷命令切换目录
zsh-autosuggestions zsh-syntax-highlighting：命令补全

#### 命令
mkdircd:创建目录并切换至该目录
lc：ls + wc -l 
ff：搜索含有某些内容的文件，可二次筛选文件
fff：搜索含有内容
**：自动代码补全
#### 快捷键
Ctrl+R：调出历史命令
Ctrl+|：快捷进入目录
Ctrl+T：搜索文件并预览


## 使用方法一
git clone ： 方便快捷，看心情持续更新
```shell
cd $HOME
git clone git@github.com:cherryamme/My_Better_Terminal.git
#symbol link, choose file you want or all
ln -sf $HOME/My_Better_Terminal/AllMy_config/{.completion.bash,.completion.zsh,.Rprofile,.fzf.bash,.fzf.zsh,.p10k.zsh,.radian_profile,.rgignore,.tmux.conf,.tmux.conf.local,.zshrc} ~
ln -sf $HOME/My_Better_Terminal/.ohmyzsh ~
```

## 使用方法二
将上述文件添加至HOME目录下,删除仓库。


