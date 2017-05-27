# mui
> 兼容pc移动端的全局ui

属性目录：

+ [utilities](./src/basic/utilities)
+ [边框](#边框)
+ [按钮](#按钮)
+ [颜色](#颜色)
+ [字体](#字体)
+ [内外边距](#内外边距)
+ [标签](#标签)
+ [文本](#文本)

---------

## 变量说明

颜色值
``` sass
// [color]
$color: (
    success: $green,
    error: $red,
    info: $blue,
    dark: $gray-dark,
    warning: $orange,
    fff: #ffffff
) !default;
```

边框方向类型
``` sass
// [borderType]
$borderType: (
        l: 0 0 0 1px,
        r: 0 1px 0 0,
        t: 1px 0 0 0,
        b: 0 0 1px 0,
        lr: 0 1px,
        tb: 1px 0
);
```

## 边框
> 移动端有前缀m-，实现利用的伪元素边框缩放

+ bd-[color]
+ bd-[color]-[borderType]

## 按钮

## 颜色

## 字体

## 内外边距

## 标签

## 文本

---------

``` bash
# compile
sass --watch _index.scss:../../dist/mui.css --style compressed
```