## 说一下你对 `flex: 1` 的理解

- flex属性是 `flex-grow` 、`flex-shrink` 和 `flex-basis` 这三个属性的简写形式;
- 对于一个flex布局中的子项，其flex属性的默认值为 `flex: 0 1 auto`;
- 而 `flex: 1`代表的含义其实是 `flex: 1 1 auto`，即将 `flex-grow` 属性设置为1。
