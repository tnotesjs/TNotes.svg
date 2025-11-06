# svg

- 如果你学习过 html、css，那么 svg 的很多笔记只需要搂一眼就行了。快速把笔记内容给过一遍，对 svg 中的一些元素有个初步的认识，知道不同元素之间分别可以用来绘制什么图形，当在项目中需要手写 svg 的时候，然后在线搜即可。

<!-- region:toc -->

  - [1. svg 起步](#1-svg-起步)
  - [2. 基本图形绘制](#2-基本图形绘制)
  - [3. path 路径](#3-path-路径)
  - [4. stroke 描边和 fill 填充](#4-stroke-描边和-fill-填充)
  - [5. 复用](#5-复用)
  - [6. svg 与传统前端技术相结合](#6-svg-与传统前端技术相结合)
    - [6.1. svg + html](#61-svg--html)
    - [6.2. svg + css](#62-svg--css)
    - [6.3. svg + js](#63-svg--js)
  - [7. 练习](#7-练习)
  - [8. ⏰ empty](#8--empty)

<!-- endregion:toc -->


<!-- ## 1. svg 在线免费教程 -->

## 1. svg 起步

- [x] [0043. 理解 svg 是什么](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0043.%20%E7%90%86%E8%A7%A3%20svg%20%E6%98%AF%E4%BB%80%E4%B9%88/README.md)
- [x] [0044. 对比 svg 和 canvas](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0044.%20%E5%AF%B9%E6%AF%94%20svg%20%E5%92%8C%20canvas/README.md)
- [x] [0045. 区分 Image 和 Graphic](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0045.%20%E5%8C%BA%E5%88%86%20Image%20%E5%92%8C%20Graphic/README.md)
- [x] [0046. 理解 svg 的 xmlns 属性](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0046.%20%E7%90%86%E8%A7%A3%20svg%20%E7%9A%84%20xmlns%20%E5%B1%9E%E6%80%A7/README.md)
- [x] [0047. 理解 svg 的 version 属性](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0047.%20%E7%90%86%E8%A7%A3%20svg%20%E7%9A%84%20version%20%E5%B1%9E%E6%80%A7/README.md)
- [x] [0009. vscode svg 相关插件](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0009.%20vscode%20svg%20%E7%9B%B8%E5%85%B3%E6%8F%92%E4%BB%B6/README.md)
- [x] [0001. 在 html 中嵌入 svg](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0001.%20%E5%9C%A8%20html%20%E4%B8%AD%E5%B5%8C%E5%85%A5%20svg/README.md)
- [x] [0002. 在 .html 和 .svg 文件中，根元素 svg 的数量](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0002.%20%E5%9C%A8%20.html%20%E5%92%8C%20.svg%20%E6%96%87%E4%BB%B6%E4%B8%AD%EF%BC%8C%E6%A0%B9%E5%85%83%E7%B4%A0%20svg%20%E7%9A%84%E6%95%B0%E9%87%8F/README.md)
- [x] [0035. 绘制坐标系网格](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0035.%20%E7%BB%98%E5%88%B6%E5%9D%90%E6%A0%87%E7%B3%BB%E7%BD%91%E6%A0%BC/README.md)
- [x] [0034. 理解 viewBox 视口](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0034.%20%E7%90%86%E8%A7%A3%20viewBox%20%E8%A7%86%E5%8F%A3/README.md)

## 2. 基本图形绘制

- [x] [0005. 使用 line 绘制直线](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0005.%20%E4%BD%BF%E7%94%A8%20line%20%E7%BB%98%E5%88%B6%E7%9B%B4%E7%BA%BF/README.md)
- [x] [0007. 使用 polyline 绘制折线](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0007.%20%E4%BD%BF%E7%94%A8%20polyline%20%E7%BB%98%E5%88%B6%E6%8A%98%E7%BA%BF/README.md)
- [x] [0008. 使用 rect 绘制矩形](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0008.%20%E4%BD%BF%E7%94%A8%20rect%20%E7%BB%98%E5%88%B6%E7%9F%A9%E5%BD%A2/README.md)
- [x] [0006. 使用 polygon 绘制多边形](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0006.%20%E4%BD%BF%E7%94%A8%20polygon%20%E7%BB%98%E5%88%B6%E5%A4%9A%E8%BE%B9%E5%BD%A2/README.md)
- [x] [0003. 使用 circle 绘制圆形](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0003.%20%E4%BD%BF%E7%94%A8%20circle%20%E7%BB%98%E5%88%B6%E5%9C%86%E5%BD%A2/README.md)
- [x] [0004. 使用 ellipse 绘制椭圆形](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0004.%20%E4%BD%BF%E7%94%A8%20ellipse%20%E7%BB%98%E5%88%B6%E6%A4%AD%E5%9C%86%E5%BD%A2/README.md)
- [x] [0031. 使用属性 x、y、dx、dy 控制文本的绘制位置](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0031.%20%E4%BD%BF%E7%94%A8%E5%B1%9E%E6%80%A7%20x%E3%80%81y%E3%80%81dx%E3%80%81dy%20%E6%8E%A7%E5%88%B6%E6%96%87%E6%9C%AC%E7%9A%84%E7%BB%98%E5%88%B6%E4%BD%8D%E7%BD%AE/README.md)
- [x] [0029. 使用属性 text-anchor 设置文本的水平对齐方式](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0029.%20%E4%BD%BF%E7%94%A8%E5%B1%9E%E6%80%A7%20text-anchor%20%E8%AE%BE%E7%BD%AE%E6%96%87%E6%9C%AC%E7%9A%84%E6%B0%B4%E5%B9%B3%E5%AF%B9%E9%BD%90%E6%96%B9%E5%BC%8F/README.md)
- [x] [0030. 使用属性 textLength 约束文本长度](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0030.%20%E4%BD%BF%E7%94%A8%E5%B1%9E%E6%80%A7%20textLength%20%E7%BA%A6%E6%9D%9F%E6%96%87%E6%9C%AC%E9%95%BF%E5%BA%A6/README.md)
- [x] [0032. 通过 text 的其他属性来控制文本样式](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0032.%20%E9%80%9A%E8%BF%87%20text%20%E7%9A%84%E5%85%B6%E4%BB%96%E5%B1%9E%E6%80%A7%E6%9D%A5%E6%8E%A7%E5%88%B6%E6%96%87%E6%9C%AC%E6%A0%B7%E5%BC%8F/README.md)
- [x] [0019. 使用 tspan 更细粒度地控制 text 中的内容](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0019.%20%E4%BD%BF%E7%94%A8%20tspan%20%E6%9B%B4%E7%BB%86%E7%B2%92%E5%BA%A6%E5%9C%B0%E6%8E%A7%E5%88%B6%20text%20%E4%B8%AD%E7%9A%84%E5%86%85%E5%AE%B9/README.md)
- [x] [0018. 使用 textPath 实现按照指定路径绘制文本](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0018.%20%E4%BD%BF%E7%94%A8%20textPath%20%E5%AE%9E%E7%8E%B0%E6%8C%89%E7%85%A7%E6%8C%87%E5%AE%9A%E8%B7%AF%E5%BE%84%E7%BB%98%E5%88%B6%E6%96%87%E6%9C%AC/README.md)

## 3. path 路径

- [x] [0048. 认识 path 元素](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0048.%20%E8%AE%A4%E8%AF%86%20path%20%E5%85%83%E7%B4%A0/README.md)
- [x] [0012. 使用 path 绘制直线](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0012.%20%E4%BD%BF%E7%94%A8%20path%20%E7%BB%98%E5%88%B6%E7%9B%B4%E7%BA%BF/README.md)
- [x] [0013. 绘制【扫码】图标](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0013.%20%E7%BB%98%E5%88%B6%E3%80%90%E6%89%AB%E7%A0%81%E3%80%91%E5%9B%BE%E6%A0%87/README.md)
- [x] [0011. 使用 path 绘制弧](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0011.%20%E4%BD%BF%E7%94%A8%20path%20%E7%BB%98%E5%88%B6%E5%BC%A7/README.md)
- [x] [0036. 绘制【群】图标](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0036.%20%E7%BB%98%E5%88%B6%E3%80%90%E7%BE%A4%E3%80%91%E5%9B%BE%E6%A0%87/README.md)
- [x] [0010. 使用 path 绘制二次贝塞尔曲线](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0010.%20%E4%BD%BF%E7%94%A8%20path%20%E7%BB%98%E5%88%B6%E4%BA%8C%E6%AC%A1%E8%B4%9D%E5%A1%9E%E5%B0%94%E6%9B%B2%E7%BA%BF/README.md)
- [x] [0014. 使用 path 绘制三次贝塞尔曲线](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0014.%20%E4%BD%BF%E7%94%A8%20path%20%E7%BB%98%E5%88%B6%E4%B8%89%E6%AC%A1%E8%B4%9D%E5%A1%9E%E5%B0%94%E6%9B%B2%E7%BA%BF/README.md)

## 4. stroke 描边和 fill 填充

- [x] [0028. 使用属性 stroke、stroke-width、stroke-opacity、stroke-linecap 设置描边样式](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0028.%20%E4%BD%BF%E7%94%A8%E5%B1%9E%E6%80%A7%20stroke%E3%80%81stroke-width%E3%80%81stroke-opacity%E3%80%81stroke-linecap%20%E8%AE%BE%E7%BD%AE%E6%8F%8F%E8%BE%B9%E6%A0%B7%E5%BC%8F/README.md)
- [x] [0027. 使用属性 stroke-linejoin 设置线条连接处样式](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0027.%20%E4%BD%BF%E7%94%A8%E5%B1%9E%E6%80%A7%20stroke-linejoin%20%E8%AE%BE%E7%BD%AE%E7%BA%BF%E6%9D%A1%E8%BF%9E%E6%8E%A5%E5%A4%84%E6%A0%B7%E5%BC%8F/README.md)
- [x] [0025. 使用属性 stroke-dasharray 设置虚线](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0025.%20%E4%BD%BF%E7%94%A8%E5%B1%9E%E6%80%A7%20stroke-dasharray%20%E8%AE%BE%E7%BD%AE%E8%99%9A%E7%BA%BF/README.md)
- [x] [0026. 使用属性 stroke-dashoffset 设置虚线的偏移](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0026.%20%E4%BD%BF%E7%94%A8%E5%B1%9E%E6%80%A7%20stroke-dashoffset%20%E8%AE%BE%E7%BD%AE%E8%99%9A%E7%BA%BF%E7%9A%84%E5%81%8F%E7%A7%BB/README.md)
- [x] [0023. 【练习】使用 stroke-dasharray 模拟加载中动画效果](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0023.%20%E3%80%90%E7%BB%83%E4%B9%A0%E3%80%91%E4%BD%BF%E7%94%A8%20stroke-dasharray%20%E6%A8%A1%E6%8B%9F%E5%8A%A0%E8%BD%BD%E4%B8%AD%E5%8A%A8%E7%94%BB%E6%95%88%E6%9E%9C/README.md)
- [ ] [0015. 使用属性 fill、fill-opacity 设置填充样式](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0015.%20%E4%BD%BF%E7%94%A8%E5%B1%9E%E6%80%A7%20fill%E3%80%81fill-opacity%20%E8%AE%BE%E7%BD%AE%E5%A1%AB%E5%85%85%E6%A0%B7%E5%BC%8F/README.md)
- [ ] [0024. 使用属性 fill-rule 设置填充规则](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0024.%20%E4%BD%BF%E7%94%A8%E5%B1%9E%E6%80%A7%20fill-rule%20%E8%AE%BE%E7%BD%AE%E5%A1%AB%E5%85%85%E8%A7%84%E5%88%99/README.md)
- [ ] [0037. 绘制【眼睛】图标](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0037.%20%E7%BB%98%E5%88%B6%E3%80%90%E7%9C%BC%E7%9D%9B%E3%80%91%E5%9B%BE%E6%A0%87/README.md)

## 5. 复用

- [ ] [0020. 使用 use 引用图形](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0020.%20%E4%BD%BF%E7%94%A8%20use%20%E5%BC%95%E7%94%A8%E5%9B%BE%E5%BD%A2/README.md)
- [ ] [0017. 使用 g 作为容器](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0017.%20%E4%BD%BF%E7%94%A8%20g%20%E4%BD%9C%E4%B8%BA%E5%AE%B9%E5%99%A8/README.md)
- [ ] [0016. 使用 defs 定义图形](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0016.%20%E4%BD%BF%E7%94%A8%20defs%20%E5%AE%9A%E4%B9%89%E5%9B%BE%E5%BD%A2/README.md)

## 6. svg 与传统前端技术相结合

### 6.1. svg + html

- [x] [0001. 在 html 中嵌入 svg](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0001.%20%E5%9C%A8%20html%20%E4%B8%AD%E5%B5%8C%E5%85%A5%20svg/README.md)

### 6.2. svg + css

- [ ] [0021. 使用 css 控制 svg 样式](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0021.%20%E4%BD%BF%E7%94%A8%20css%20%E6%8E%A7%E5%88%B6%20svg%20%E6%A0%B7%E5%BC%8F/README.md)

### 6.3. svg + js

- [ ] [0022. 使用 js 控制 svg 实现 CRUD 操作](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0022.%20%E4%BD%BF%E7%94%A8%20js%20%E6%8E%A7%E5%88%B6%20svg%20%E5%AE%9E%E7%8E%B0%20CRUD%20%E6%93%8D%E4%BD%9C/README.md)

## 7. 练习

- 0013
- 0023
- 0036
- 0037


- [ ] [0033. 简易动态坐标系制作](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0033.%20%E7%AE%80%E6%98%93%E5%8A%A8%E6%80%81%E5%9D%90%E6%A0%87%E7%B3%BB%E5%88%B6%E4%BD%9C/README.md)
- [ ] [0039. 【练习】绘制静态折线图](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0039.%20%E3%80%90%E7%BB%83%E4%B9%A0%E3%80%91%E7%BB%98%E5%88%B6%E9%9D%99%E6%80%81%E6%8A%98%E7%BA%BF%E5%9B%BE/README.md)
- [ ] [0038. 【练习】绘制动态折线图](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0038.%20%E3%80%90%E7%BB%83%E4%B9%A0%E3%80%91%E7%BB%98%E5%88%B6%E5%8A%A8%E6%80%81%E6%8A%98%E7%BA%BF%E5%9B%BE/README.md)
- [ ] [0040. 【练习】绘制柱状图](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0040.%20%E3%80%90%E7%BB%83%E4%B9%A0%E3%80%91%E7%BB%98%E5%88%B6%E6%9F%B1%E7%8A%B6%E5%9B%BE/README.md)
- [ ] [0042. 【练习】绘制静态的饼图](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0042.%20%E3%80%90%E7%BB%83%E4%B9%A0%E3%80%91%E7%BB%98%E5%88%B6%E9%9D%99%E6%80%81%E7%9A%84%E9%A5%BC%E5%9B%BE/README.md)
- [ ] [0041. 【练习】绘制动态饼图](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0041.%20%E3%80%90%E7%BB%83%E4%B9%A0%E3%80%91%E7%BB%98%E5%88%B6%E5%8A%A8%E6%80%81%E9%A5%BC%E5%9B%BE/README.md)

## 8. ⏰ empty

- [ ] [0049. empty](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0049.%20empty/README.md)
