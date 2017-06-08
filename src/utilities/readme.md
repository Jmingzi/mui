### utility 包含的类有

变量说明
```sass
// [display]
$display: (i: inline, b: block, ib: inline-block, n: none);

// [position]
$position: (s: static, r: relative, a: absolute, f: fixed);

// 宽度／高度／行高
// [size]
$size: 5 10 15 20 30 40 45 50 55 60 70 80 90 100;

// [align]
$align: top middle bottom text-bottom text-top;
```

+ display-[display]
+ select-none
+ highlight-none
+ touch-scroll
+ fl/fr/fn
+ cl
+ align-[align]
+ position-[position]
+ fixed-top
+ fixed-bottom
+ px-width-[size]
+ px-height-[size]
+ px-line-[size]    // line-height
+ rem-width-[size]
+ rem-height-[size]
+ rem-line-[size]   // line-height
+ width-100     // 100%
+ height-100    // 100%
+ max-width-100 
+ max-height-100
+ min-width-100
+ min-height-100

@mixin

```
_position.scss
absolute-middle($width, $height, $top, $left)
```