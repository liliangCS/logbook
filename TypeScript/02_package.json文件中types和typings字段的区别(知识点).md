## package.json文件中types和typings字段的区别

在 `package.json` 文件中，可以使用 `types` 和 `typings` 字段来指定模块的类型声明文件路径，其区别如下：

- `types`: 这个字段指定的是主类型声明文件的路径。主类型声明文件必须命名为 `index.d.ts`，并且位于模块的根目录下。当其他人使用这个模块时，`TypeScript` 会自动加载这个文件，以便进行类型检查。
- `typings`: 这个字段也用来指定模块的类型声明文件路径，但它不限定主类型声明文件的名称，也不要求放在根目录下。如果同时指定了 `types` 和 `typings` 字段，`TypeScript` 会优先使用 `types` 字段指定的文件路径。
