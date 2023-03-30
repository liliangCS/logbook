## 说一下你对BFC的理解

BFC是 Block Formatting Context 的简写，翻译过来就是块格式化上下文的意思。它是一个独立的布局环境，其中的元素布局不受外界的影响。
其常见的触发方式有：
- 浮动元素（float 值不为 none）；
- 绝对定位元素（position 值为 absolute 或 fixed）；
- 行内块元素（display 值为 inline-block）；
- overflow 值不为 visible、clip 的块元素；
- 弹性元素（display 值为 flex 或 inline-flex 元素的直接子元素），如果它们本身既不是 flex、grid 也不是 table 容器。


其特性：
- 包含内部浮动；
- 排除外部浮动；
- 阻止外边距重叠。
