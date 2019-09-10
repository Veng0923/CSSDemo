# 定位position

position 属性指定了元素的定位类型

## static定位

HTML 元素的默认值，即没有定位，遵循正常的文档流对象。

静态定位的元素不会受到 top, bottom, left, right影响。

```css
 position: static;
```

## fixed定位

元素的位置相对于浏览器窗口是固定位置。

即使窗口是滚动的它也不会移动。

```css
 position: fixed;
```

### relative定位

相对定位元素的定位是相对其正常位置。

```css
 position: relative;
```

## absolute 定位

绝对定位的元素的位置相对于最近的已定位父元素，如果元素没有已定位的父元素，那么它的位置相对于`<html>`.

```css
position: absolute;
```

## sticky 定位

sticky 英文字面意思是粘，粘贴，所以可以把它称之为粘性定位。

它的行为就像 **position:relative;** 而当页面滚动超出目标区域时，它的表现就像 **position:fixed;**，它会固定在目标位置。

## 重叠的元素

元素的定位与文档流无关，所以它们可以覆盖页面上的其它元素

z-index属性指定了一个元素的堆叠顺序（哪个元素应该放在前面，或后面）

一个元素可以有正数或负数的堆叠顺序：

```css
z-index:-1;
```

