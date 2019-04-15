# datalist

## 标签定义

* `<datalist>` 标签规定了 `<input>` 元素可选的选项列表。

* `<datalist>` 标签被用来在为 `<input>` 元素提供"自动完成"的特性。简单来说就是可以在 `input` 里面进行简单的模糊搜索。

## 兼容性
=> [兼容性](https://caniuse.com/#feat=datalist&search=datalist)


## 举个🌰：
```html
<input list="browsers" id="myBrowser" name="myBrowser" placeholder="请选择对应浏览器"/>
<datalist id="browsers">
    <option value="Chrome" label="Blink">
    <option value="Firefox" label="Gecko">
    <option value="Internet Explorer" label="Trident">
    <option value="Safari" label="Webkit">
    <option value="" label="other"></option>
</datalist>
```

例子里：
1. `input` 的 `list` 和 `datalist` 的 `id`需要对应，
2. `datalist` 的 `value` 属性，是显示在下拉选项的左侧内容，`label` 属性是显示在下拉右侧的内容，
3. 如果只有 `label` 没有 `value` 属性，将不会显示在下拉选项中，这时候哪怕给 `value` 一个空格，也能在下拉选项中显示出来。


---

## 温馨提示：
`datalist` 标签是不支持自定义样式的，也就是说，你最多只能控制一下 `input` 的样式，如果想把 `datalist` 改成项目中需要的样子，是不大可能的，只能自己用其他方式来模拟代替，例如 `ul li`、`div`。当然，如果没有样式需求默认就行，那这个标签还是挺好用的。 