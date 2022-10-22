1. 安装Git
Git是目前世界上最先进的分布式版本控制系统，可以有效、高速的处理从很小到非常大的项目版本管理。Git的作用是将本地的网页文件传到github上。

Git下载地址
Git教程
windows： 到git官网上下载.exe文件,Download git,安装选项全部默认即可。

2. 安装node.js
Hexo是基于node.js编写的，所以需要安装一下node.js和里面的npm工具。

windows： 到Node.js官网下载.exe文件，安装选项全部默认。安装好之后，按Win+R打开cmd命令提示符，输入node -v和npm -v，若出现版本号，则说明安装成功。

3. 添加npm国内源
使用阿里的国内镜像进行加速下载

npm config set registry https://registry.npm.taobao.org
4. 安装Hexo
前面git和nodejs安装好后，就可以安装hexo了，你可以先创建一个文件夹MyBlog，用来存放自己的博客文件，然后cd到这个文件夹下（或者在这个文件夹下直接鼠标右键git bash打开）。

比如我的博客文件都存放在C:\MyBlog目录下。

在该目录下右键点击Git Bash Here，打开git的控制台窗口，以后我们所有的操作都在git控制台进行，就不用Windows自带的cmd了。

定位到该目录下，输入npm install -g hexo-cli安装Hexo。可能会有几个报错，不用理会。

npm install -g hexo-cli
安装完后输入hexo -v验证是否安装成功。

接下来初始化一下hexo,即初始化我们的博客网站。例如我的在C:\MyBlog文件夹下的命令行中，输入hexo init初始化文件夹

hexo init
新建完成后，指定文件夹MyBlog目录下有：

node_modules: 依赖包
public：存放生成的页面
scaffolds：生成文章的一些模板
source：用来存放你的文章
themes：主题**
_config.yml: 博客的配置文件**
到此为止，本地的Hexo基础环境搭建完成了。
