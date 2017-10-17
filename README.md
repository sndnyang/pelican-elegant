# Elegant介绍

Elegant 是 Pelican静态博客生成使用的一种 主题模式theme.

## 新功能

- 左侧自动移动、高亮的目录 left side a table of content can automove to proper position
- 响应式 Responsive by Bootstrap
- 响应式目录 Responsive table of content in mobile phone and PC and pad
- 友言 加 disqus， 后者国内用不上
- 微博动态
- 多处引用图片 自动popover效果

没错， 光这点小功能就花了我很长时间改， 不过改下来， 对前端也多了点了解。

## 希望的新效果

- 标签云 tag cloud
- 拓扑关系图 topo relationship graph

## 图片popover

读PDF时，有点很烦人就是涉及到的图片在别处需要翻页， PDF我搞不定， 但写笔记时的markdown+html可以搞， 一张图片如果有多处引用， 每处都显示，多不好， 照论文的风格， 只使用并显示一次

    ![描述替换文本](链接地址)
    或参考式
    ![描述替换文本][id]
    [id]: 地址 文本

别的地方只要全词匹配上 描述替换文本， 就自动生成该图片的 popover

代码在 stat/js/index.js 的 renderQuoteTip() 函数

调用方式： templates/article.html

    <script>
        $(function (){
            renderQuoteTip();
        });
    </script>


[示例](http://blog.zhimind.com/lifetime-aware-regression-model-for-video-popularity.html) 的 “类似 Figure-2 每个数据集”

# 原版Origin
Please visit [Elegant - a theme for Pelican](http://oncrashreboot.com/pelican-elegant) at my blog for detailed features and documentation.

Elegant offers several unique features including search, live filter, collapsible comments, Mailchimp, custom 404 page, etc. It is a minimal, and stylish theme that looks amazing across all screen resolutions and devices.  

Here is an example search result

![Search result screenshot](https://raw.github.com/talha131/pelican-elegant/master/search-result-screenshot.png)

Here is how the home page looks like

![Home page screenshot](https://raw.github.com/talha131/pelican-elegant/master/home-page-screenshot.png)

This is how a generated article looks like

![Article screenshot](https://raw.github.com/talha131/pelican-elegant/master/article-screenshot.png)

[![githalytics.com alpha](https://cruel-carlota.pagodabox.com/c71132a529c1c5d7eb8dc5ea4825a851 "githalytics.com")](http://githalytics.com/talha131/pelican-elegant)

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/talha131/pelican-elegant/trend.png)](https://bitdeli.com/free "Bitdeli Badge")
