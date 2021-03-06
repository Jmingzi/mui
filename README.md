# mui
> 兼容pc移动端的全局ui

属性目录：

+ [utilities](./src/utilities)
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
    c666: $c666,
    c999: $c999,
    aaa: $aaa,
    ccc: $ccc,
    gray-light: $gray-light,
    gray-lighter: $gray-lighter,
    gray-lightest: $gray-lightest
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
$mpSize: 5 10 15 20 25 30 40 45 50 55 60 70 80 90 100 !default;
```

圆角
```sass
// [radius]
$radius: 2 3 4 5 6 10 15 20 25 !default;
```

## 边框
> 移动端有前缀m-，实现利用的伪元素边框缩放

+ bd-[color]
+ m-bd-[borderType]
+ bd-[color]-[borderType]
+ bd-none
+ m-bd-none
+ radius-[radius]
+ no-outline

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

+ font-0
+ [前缀]-font-[fontSize]

## 内外边距
> 涉及尺寸的前缀均为 `px-/rem-`

```sass
// [mpType]
$mpType: t r b l lr tb;
```

+ margin-auto
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

> 对齐方式

+ ib-top
+ ib-middle
+ ib-bottom

## 阴影

+ shadow-block
+ shadow-bottom
+ inner-shadow
+ shadow-block-big

## 手势

+ cursor-p
+ cursor-m

## 透明度

+ opacity-0
+ opacity-1

## 定位

+ fixed-top
+ fixed-bottom
+ top-0
+ left-0
+ right-0
+ bottom-0
+ z-index-[5 ~ 10]
+ [px/rem]-[top/left/right/bottom]-[mapSize]

更多请点击查看 [utilities](./src/utilities)

## 编译

``` bash
# compile
sass --watch _index.scss:../dist/mui.css --style compressed
```