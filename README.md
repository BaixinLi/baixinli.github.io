# My Homepage
This is an academic homepage of Baixin Li, powered by GitHub Pages.   
Homepage: [baixinli.github.io](https://baixinli.github.io/)


## 简介
我正在尝试制作一个尽可能简单的个人学术主页。  
我称之为 An academic homepage that is as simple as possible.  
我希望将其简写为简写为 Homepage-ASAP。中文是 ASAP 主页。  

我希望这个网站在满足下面的条件的基础上，尽可能减少代码：  
- 可以显示数学公式
- 可以包含多层网页
- 更新内容操作简单

如果你有更ASAP的方法，欢迎分享。  

## 网站风格样式
这个网站基于 Jekyll 构造，但是并未使用任何 Jekyll 主题，比如常见的 Minima 和 Minimal。  
本网站使用近似于 Github 默认的 Markdown 渲染风格作为网站风格样式。  

Github 默认的 Markdown 渲染格式中，并不支持对于 Latex 等数学公式相关语法的支持。  
所以尽管网站可以正常渲染，但是其中的数学公式并不会正确显示。  
为了正确渲染数学公式，不使用 Github 默认风格，使用自定义的近似于 Github 默认风格的样式。  

网站风格样式被写在 _layouts/default.html 文件中。  
这个文件中使用 Gemini（一种人工智能AI服务）写了类似于 Github 默认风格的样式。并追加了 MathJax 来正确渲染数学公式。  

## 网站构造方法
Jekyll 是将 Markdown 文件自动转换为 Html 文件的一种服务。  

本网站在本地 VScode 的 Container 中运行，并使用本地 Jeklly 服务来测试构造。  
网站主页写在 index.md 等文件中，由 Jeklly 自动转换为 Html 类型的静态网站。  
产生的 _site 文件夹是使用本地 Jeklly 服务构造的静态网站。  

但是本网站并不使用构造好的 _site 文件夹中的 html 文件来作为网站的源文件。  
本网站使用 Markdown 文件和 Github 默认的 Jekyll 转译服务来构造网站。  
也就是在 Github 仓库中上传 Markdown 文件，利用 Github Pages 内置转译服务来构造网站。  
因此，即便是 _site 文件夹不上传到仓库中，Github 一样可以根据 Markdown 文件来构造网站。


## 文件说明
Gemfile 和 _config.yml 是 Jekyll 配置的重要文件。  

Gemfile 记录了 Jekyll，Ruby 版本，Github Pages 等信息。  
_config.yml 记录了影响整个 Blog 的内容，比如作者名，URL，网页使用的主题（theme）等内容。  
.gitignore 中指示了不需要同步到 Github 的文件和文件夹。  