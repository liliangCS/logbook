## 使用CSS实现一个三角形

利用盒模型边框交界处45°等分的特点，将三个方向的 `border-color` 属性设置成透明。

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    .triangle {
      width: 0;
      height: 0;
      border: 100px solid transparent;
      border-bottom-color: red;
    }
  </style>
</head>

<body>
  <div class="triangle"></div>
</body>

</html>
```
