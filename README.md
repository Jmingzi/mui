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
) !default;
```

字体大小
``` sass
// [fontSize]
$font: 8 10 12 14 16 18 20 24 28 32 40 45 !default;
```

边距大小
``` sass
// [mpSize]
$mpSize: 5 10 15 20 25 30 40 !default;
```


## 边框
> 移动端有前缀m-，实现利用的伪元素边框缩放

+ bd-[color]
+ bd-[color]-[borderType]
+ bd-none
+ bd-radius-[mpSize]

## 按钮
> 涉及尺寸的前缀均为 `px-/rem-`

+ [前缀]-btn
+ btn
+ btn-disabled
+ btn-[color]
+ btn-inverse
+ btn-block

## 颜色
> 颜色分为色值／背景色／边框色

+ color-[color]
+ bg-[color]
+ bd-[color]

## 字体
> 涉及尺寸的前缀均为 `px-/rem-`

+ [前缀]-font-[fontSize]

## 内外边距
> 涉及尺寸的前缀均为 `px-/rem-`

```sass
// [mpType]
$mpType: t r b l lr tb;
```

+ [前缀]-margin-[fontSize]-[mpType][mpSize]
+ [前缀]-padding-[fontSize]-[mpType][mpSize]


## 标签
> 涉及尺寸的前缀均为 `px-/rem-`

+ [前缀]-tag-[color]
+ [前缀]-tag-bg-[color]
+ tag-small

## 文本
```sass
// [align]
$align: left right center;
```

+ text-[align]
+ no-wrap
+ over-text
+ line-through
+ line-none

## 编译

``` bash
# compile
sass --watch _index.scss:../../dist/mui.css --style compressed
```