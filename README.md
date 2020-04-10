<h1 align="center">一款Hexo端优美的MaterialDesign风格主题 MDM</h1>

<h3 align="center">简洁，轻巧，麻麻再也不用担心打开博客速度慢了</h3>
<br><br>

# 推荐
1. [Hexo 博文管理工具，麻麻再也不用担心忘记管理hexo博文的命令啦](https://github.com/TonyChenn/HexoBlogWriteTool)
2. [CSDN博文导出工具](https://github.com/TonyChenn/BlogExportTool)

# 更新介绍：
- 2020-4-10 : 
1. 添加站点地图
2. 添加灰色(哀悼)模式
3. 添加谷歌广告开关
4. 支持Emoji表情
5. 添加Gitalk 评论方式

- 2020-1-14 : 添加图片预览，优化夜间模式，文章代码排版。

# :art:演示
[tonychenn.cn](https://tonychenn.cn) 觉得不错，点个Star

# :pushpin:介绍
1. 响应式布局，适配移动端和PC端
2. 优美MaterialDesign设计
3. 轻巧极速加载
# 实现的功能
1. 基本的博客展示，首页，标签页，归档页，关于页
2. 一言随机内容展示
3. 使用Valine文章评论，新增Gitalk
4. 开启访问人数，次数统计
5. 视频博文的展示播放
6. 全局灰色模式，白天/夜晚模式

# :computer:PC端

![](https://raw.githubusercontent.com/TonyChenn/BlogPicture/master/2019/0406/img1.jpg)
![](https://raw.githubusercontent.com/TonyChenn/BlogPicture/master/2019/0406/img2.jpg)
![](https://raw.githubusercontent.com/TonyChenn/BlogPicture/master/2019/0406/about.jpg)

# :iphone:移动端

![](https://raw.githubusercontent.com/TonyChenn/BlogPicture/master/2019/0406/phone_main.jpg)
![](https://raw.githubusercontent.com/TonyChenn/BlogPicture/master/2019/0406/phone_tag.jpg)
![](https://raw.githubusercontent.com/TonyChenn/BlogPicture/master/2019/0406/phone_archives.jpg)

# 案例
本博客使用mdm主题，更多细节，自行查看[TonyChenn.cn](Tonychenn.cn)

# :cd:安装

## 下载
```bash
$ git clone https://github.com/TonyChenn/hexo-theme-mdm
```

## 更新
```bash
$ cd themes/mdm
$ git pull
```

## 开启站点地图模块
1. 安装sitemap
```bash
//google
$ npm install hexo-generator-sitemap --save

//baidu
$ npm install hexo-generator-baidu-sitemap --save
```
2. 配置sitemap
主题根目录下_config.yml文件中启用下面
```
# 站点地图
sitemap:
  path: sitemap.xml
baidusitemap:
  path: baidusitemap.xml
```
3. 重新生成部署
```bash
$ hexo clean && hexo g && hexo s
```

## 开启Emoji表情支持
1. 需要卸载旧的渲染器 & 安装新的渲染器
```bash
$ npm un hexo-renderer-marked --save 
$ npm i hexo-renderer-markdown-it --save
$ npm install markdown-it-emoji --save
```
2. heox配置文件中添加
``` bash
# Markdown-it config
markdown:
  render:
    html: true
    xhtmlOut: false
    breaks: true
    linkify: true
    typographer: true
    quotes: '“”‘’'
  plugins:
    - markdown-it-abbr
    - markdown-it-footnote
    - markdown-it-ins
    - markdown-it-sub
    - markdown-it-sup
    - markdown-it-emoji
  anchors:
    level: 2
    collisionSuffix: 'v'
    permalink: true
    permalinkClass: header-anchor
    permalinkSymbol: ¶
```

# 下载
Github: https://github.com/TonyChenn/hexo-theme-mdm
觉得不错？点个小星星给我个鼓励吧 (*_*)
![](https://cdn.jsdelivr.net/gh/TonyChenn/BlogPicture/2019/0406/star.jpg)
