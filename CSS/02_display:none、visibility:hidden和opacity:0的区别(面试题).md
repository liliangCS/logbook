## 说一下 `display: none` 、`visibility: hidden` 和 `opacity: 0` 之间的区别

三者都起到隐藏元素的作用，其区别如下：
- `display: none`：元素不占据文档流，无法进行 DOM 事件监听；
- `visibility: hidden`：元素仍占据文档流，无法进行 DOM 事件监听；
- `opacity: 0`：元素仍占据文档流，可以进行 DOM 事件监听。
