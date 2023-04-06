## 使用TS实现一个栈（Stack）

```typescript
class Stack {
  private items: Array<any>
  constructor(items: Array<any>) {
    this.items = items
  }
  // 向栈中添加一个元素
  public push(element: any) {
    this.items.push(element)
  }
  // 从栈中弹出栈顶元素，并返回其值。如果栈为空，则返回undefined
  public pop() {
    if (this.isEmpty()) return undefined
    return this.items.pop()
  }
  // 返回栈顶元素的值，但不弹出。如果栈为空，则返回undefined
  public peek() {
    if (this.isEmpty()) return undefined
    return this.items[this.items.length - 1]
  }
  // 返回栈中元素的个数
  public size() {
    return this.items.length
  }
  // 清空栈中所有元素
  public clear() {
    this.items = []
  }
  // 判断栈是否为空
  public isEmpty() {
    return this.items.length === 0
  }
}
```
