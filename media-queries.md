Media queries 是在原有的 media type 外，加上「media feature」的篩選條件，如下例，請注意 media feature 需要用括號表示：

```css
@media (max-width: 600px) {...//styles}
@media screen and (max-width: 600px) {...//styles}
@media screen and (min-width: 600px) and (max-width: 1000px) {...//styles}
```

* `<min-width>`
用於任何寬度_大於或等於_設定值的瀏覽器。

* `<max-width>`
用於任何寬度_小於或等於_設定值的瀏覽器。

* `<min-height>`
用於任何高度_大於或等於_設定值的瀏覽器。

* `<max-height>`
用於任何高度_小於或等於_設定值的瀏覽器。

* `<orientation=portrait>`
用於任何高度_大於或等於_寬度的瀏覽器。

* `<orientation=landscape>`
用於任何寬度_大於_高度的瀏覽器。

行動優先

```css
/* default mobile styles go here first before media queries */

@media screen and (min-width: 400px)  {...}
@media screen and (min-width: 600px)  {...}
@media screen and (min-width: 1000px) {...}
@media screen and (min-width: 1400px) {...}
```

補充：@import 其他文件
寫法如下，運用 `url()` 來載入文件，而且仍然可以串接 media type and feature：

```css
@import url('styles.css') screen and (max-width: 670px);
```

ex:  media queries 是針對大於 575px ，不超過 992px 的螢幕尺寸

```css
@media screen and (min-width: 576px) and (max-width: 992px) {...} 
```
