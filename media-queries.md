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
