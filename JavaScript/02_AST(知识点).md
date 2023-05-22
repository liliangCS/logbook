## AST是什么？
> 抽象语法树（Abstract Syntax Tree），简称AST，它是源代码语法结构的一种抽象表示。它以树状的形式表现编程语言的语法结构，树上的每个节点都表示源代码中的一种结构。

## 常见节点类型
1. literal(字面量) : 本身语义代表了一个值。 
2. Identifier(标识符) : 变量名、属性名、参数名等等一系列声明和引用的名字。
3. Statement(语句) : 代码执行的最小单位。
4. Declaration(声明) : 声明语句是一种特殊的 Statement。
5. Expression(表达式) : expression的特点是执行完成后会有返回值，这也是它和语句的区别。
6. Import : 导入模块，属于一种特殊的声明语句，有三种类型 ImportSpecifier | ImportDefaultSpecifier | ImportNamespaceSpecifier。
7. Export : 导出模块，也属于一种特殊的声明，有三种类型 ExportAllDeclaration | ExportDefaultDeclaration | ExportNamedDeclaration。

## 每个 AST 节点都有自己的属性，但是它们也有一些公共的属性：
- pos，AST 节点在代码字符串中索引的起始位置，配合 end 确定节点在代码字符串中的位置（用于唯一性判定）。
- end，AST 节点在代码字符串中索引的结束位置，配合 pos 确定节点在代码字符串中的位置（用于唯一性判定）。
- kind，用来标记当前 AST 节点的类型，上面列举的节点类型都可以通过 ts.SyntaxKind 的定义来查看。
