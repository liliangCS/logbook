## 编译配置：`isolatedModules`

`isolatedModules` 是 `TypeScript` 中的一个编译选项，用于限制单个 `TypeScript` 模块文件的作用域，以防止变量泄漏。当你将 `isolatedModules` 选项设置为 `true` 时，`TypeScript` 编译器会将每个模块都视为独立的文件，并将其放入单独的闭包中。

这个选项通常用于帮助开发者避免在全局作用域中定义变量，从而减少命名冲突和代码错误。当你开启 `isolatedModules` 选项后，编译器会在编译期间检查变量声明是否存在重复。

需要注意的是，当你开启 `isolatedModules` 选项时，`TypeScript` 编译器不会将多个 `TypeScript` 模块文件合并成一个 `JavaScript` 文件。因此，你需要使用其他工具（如 `webpack` 或 `Rollup`）将多个 `JavaScript` 文件打包成单个文件。
