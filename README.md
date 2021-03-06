# Nebula官网发布教程

## 环境准备
### 本地环境安装
[Hugo 安装](https://gohugo.io/getting-started/quick-start/#step-1-install-hugo)

### 本地服务启动命令
>$ hugo server

浏览器打开访问：http://localhost:1313


## 文件结构简介
***初次使用请仔细阅读***
- nebula-website/ -------------------------------------- 官网项目名称
  - content/ ---------------------------------------- 博客文章文件夹
    - en/posts/ --------------------------------- 英文博客文件夹
      - sample/ ---------------------------- 每篇文章需要创建一个文件夹，文件夹名将会决定文章的路径（比如：https://nebula-graph.io/en/posts/sample/）
        - *.(jpg,png,jpeg) --------------- 每篇文章可放一张图片作为头图，请别将文章中图片放在此处引用，避免浏览费用，其他图片放github引用或者oss） 
        - index.md --------------------- 博客文章固定命名
    - cn/posts ---------------------------- 中文博客文件夹
  - config.toml -------------------------------- 官网模板的参数设置（title/meta/文案/连接/导航等）
  - 其他 ---------------------------------------- 大家暂时不需要更新，也避免改动

## 写文章
### 新建分支
写博客文章，都需要先在分支进行修改，然后提[PR](https://github.com/vesoft-inc/nebula-website/pulls)

### 操作目录
> nebula-website/content/

详细信息可参照已有的文章规律

### SEO信息填写
每篇文章文件夹下的index.md，都会有这样一段信息格式：
``` markdown
---
title: "xxx" // 标题meta
data: 2020-10-10 // 日期
// 根据需要后续还会增加，目前暂时只有这两个
---
```
上面这段信息填写是方便进行博客时间线排列及SEO优化的，请务必填写，保证准确简洁。

### 文章编写
我们的文章编写，以makrdown格式来进行，具体排版大家可以拟定一个规则，站点会自动帮你做渲染。

### 实时预览
只要你本地已经通过 `hugo server` 命令启动了服务，每次文章编写进行保存操作后，访问的页面会自动刷新，本地能实时预览效果。

### 发布
本站点已经实现发布自动化，只需要将相应的分支修改提[PR](https://github.com/vesoft-inc/nebula-website/pulls)到主库master，一旦合并完成会自动发布文章到[官网](https://github.com/vesoft-inc/nebula-website/pulls)。

## 总结
以上就是关于文章发布的全部内容，有关官网的反馈，欢迎各位提[issue](https://github.com/vesoft-inc/nebula-website/issues)，当然也鼓励各位通过google搜索关键词能自我解决和学习😬。

