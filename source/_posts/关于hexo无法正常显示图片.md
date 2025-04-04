---
title: 关于hexo无法正常显示图片的解决方案
date: 2025-04-04 22:18:02
author: 暗宵
cover: true
tags:
  - 编程
  - 教程
categories: 技术随笔
---

# 本篇为hexo教程篇
## 关于图片路径问题
##### 本博客已*暂时*解决此问题（但愿不会**复发**）

原版的hexo-generator对image的路径处理似乎有些问题
即使在帮助文档中更新了插入图片的方法仍然容易出现下图情况
![md我回家啥都没干就 重新生成 了一下文章就这样了](./关于hexo无法正常显示图片/1.png)

***

## 解决方案
原理：使用 **[github大佬的image插件](https://github.com/CodeFalling/hexo-asset-image)** 进行图片路径处理

```
npm install https://github.com/CodeFalling/hexo-asset-image
hexo clean
hexo g
hexo s

```

检查日志中的**update link as**字样 后面跟着的应该是使用public文件夹路径（应包括以文章日期为文件夹名称的路径）
![示例](./关于hexo无法正常显示图片/2.png)
在本地博客里图片也应正常显示
![](./关于hexo无法正常显示图片/5.png)
教程结束！感谢阅读
  
  
  
  
附上偷窥别人睡觉的蜘蛛🕷
![](./关于hexo无法正常显示图片/3.png)
![](./关于hexo无法正常显示图片/4.png)
