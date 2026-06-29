# [0028. 使用属性 stroke、stroke-width、stroke-opacity、stroke-linecap 设置描边样式](https://github.com/tnotesjs/TNotes.svg/tree/main/notes/0028.%20%E4%BD%BF%E7%94%A8%E5%B1%9E%E6%80%A7%20stroke%E3%80%81stroke-width%E3%80%81stroke-opacity%E3%80%81stroke-linecap%20%E8%AE%BE%E7%BD%AE%E6%8F%8F%E8%BE%B9%E6%A0%B7%E5%BC%8F)

<!-- region:toc -->

- [1. demos.1 - 使用 stroke 相关属性设置描边样式](#1-demos1---使用-stroke-相关属性设置描边样式)

<!-- endregion:toc -->

- stroke：设置描边颜色（边框）
- stroke-width：设置描边粗细
- stroke-opacity：设置描边颜色的透明度
- stroke-linecap：设置线段两端的形状

## 1. demos.1 - 使用 stroke 相关属性设置描边样式

```xml
<!--
stroke：设置描边颜色（边框）
stroke-width：设置描边粗细
stroke-opacity：设置描边颜色的透明度
stroke-linecap：设置线段两端的形状
  butt 直边（默认）
  round 圆角边
  square 矩形边
    视觉效果与 butt 类似。
    两端使用了矩形形状，与 butt 效果相比会长出一块。
-->
<svg style="margin: 3rem;" width="500px" height="500px" viewBox="0 0 120 120" xmlns="http://www.w3.org/2000/svg">
  <line x1="30" y1="20" x2="80" y2="20" stroke="red" stroke-width="3" stroke-opacity=".5" stroke-linecap="butt" />
  <line x1="30" y1="50" x2="80" y2="50" stroke="red" stroke-width="3" stroke-opacity=".5" stroke-linecap="round" />
  <line x1="30" y1="80" x2="80" y2="80" stroke="red" stroke-width="3" stroke-opacity=".5" stroke-linecap="square" />
</svg>
```

![](assets/2024-12-10-11-05-57.png)
