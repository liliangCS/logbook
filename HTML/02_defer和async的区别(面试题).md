## 说一下script标签中defer属性和async属性的区别

当浏览器解析script标签时，默认情况下会阻塞后续dom元素的解析。添加defer属性和async属性都会使解析script标签这个操作异步进行，即不阻塞后续dom元素的解析，在具体表现上区别如下：
- 在script标签上添加async属性，`解析script标签` 和 `解析后续dom元素` 同步进行；
- 在script标签上添加defer属性，`解析后续dom元素` 完成之后再 `解析script标签`。
