# My Homepage
This is an academic homepage of Baixin Li, powered by GitHub Pages.   
Homepage: [baixinli.github.io](https://baixinli.github.io/)


## 简介
我正在尝试制作一个尽可能简单的个人学术主页。  
我称之为 An academic homepage that is as simple as possible (Homepage-ASAP).  

我希望这个网站在满足下面的条件的基础上，尽可能减少代码：  
- 可以显示数学公式
- 可以包含多层网页
- 可以方便更新内容

如果你有更ASAP的方法，欢迎分享。  

## 网站风格样式
这个网站基于 [Jekyll](https://jekyllrb.com/) 构造，但是并未使用任何 [Jekyll Themes](https://jekyllrb.com/docs/themes/) 主题，比如常见的 Minima 和 Minimal。  
本网站使用近似于 Github 默认的 [Markdown](https://www.markdownguide.org/) 渲染风格作为网站风格样式。  

Github 默认的 Markdown 渲染格式中，并不支持用 [Latex](https://www.latex-project.org/) 写法的数学公式。  
所以尽管网站可以正常渲染，但是其中的数学公式并不会正确显示。  
为了正确渲染数学公式，不使用 Github 默认风格，使用自定义的近似于 Github 默认风格的样式。  

网站风格样式被写在 _layouts/default.html 文件中。  
这个文件中使用 Gemini（一种人工智能AI服务）和Copilot（另一种人工智能AI服务）写了网页风格样式。并追加了 MathJax 来正确渲染数学公式。  

## 网站构造方法
[Jekyll](https://jekyllrb.com/) 是将 Markdown 文件自动转换为 Html 文件，以便于创建静态网站的一种服务。  

本网站可在 VScode 的 Container 中运行，也可以忽视 .devcontainer 中的文件。  
本网站使用本地 Jeklly 服务来测试构造，本地测试需要 Ruby。  
Ruby 是一种计算机语言，Jekyll 是一个基于 Ruby 语言的 静态网站生成器 (Static Site Generator)。   
Bundler 是 Ruby 的 依赖管理工具。类似于Python 的 pip 的工具。     
网站主页写在 index.md 等文件中，由 Jeklly 自动转换为 Html 类型的静态网站。  
产生的 _site 文件夹是使用本地 Jeklly 服务构造的静态网站。  

但是本网站并不使用构造好的 _site 文件夹中的 html 文件来作为网站的源文件。  
本网站使用 Markdown 文件和 Github 默认的 Jekyll 转译服务来构造网站。  
也就是在 Github 仓库中上传 Markdown 文件，利用 [Github Pages](https://pages.github.com/) 内置转译服务来构造网站。  
因此，即便是 _site 文件夹不上传到仓库中，Github 一样可以根据 Markdown 文件来自动构造网站。


## 文件说明
Gemfile 和 _config.yml 是 Jekyll 配置的重要文件。  

Gemfile 记录了 Jekyll 版本，Github Pages 等信息。  
_config.yml 记录了影响整个 Blog 的内容，比如作者名，URL，网页使用的主题（themes）等内容。  
.gitignore 中指示了不需要同步到 Github 的文件和文件夹。  

## Resources
- [RealFaviconGenerator](https://realfavicongenerator.net/)
- [Emojipedia](https://emojipedia.org/)  

