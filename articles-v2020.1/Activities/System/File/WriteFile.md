# 写入文件

将&quot;写入内容&quot;，覆盖写入到指定文件；若文件不存在，则新建

## 属性

输入

- **文件路径** ：将&quot;写入内容&quot;，覆盖写入到此文件。支持相对和绝对路径。可在组件面板点击弹出对话框，选择目标文件；亦支持手动输入路径，若路径不存在，则新建。仅支持字符串变量和字符串
- **写入内容** ：写入目标文件的内容。仅支持字符串变量和字符串

可选

- **编码方式** ：文件的编码方式。可以在 [此处](../../../articles/附录.md) 找到每个字符编码的完整代码列表。要指定要使用的编码类型，请使用&quot; 名称&quot;字段中的值。如果未指定编码类型，则活动将搜索文件的字节顺序标记以检测编码。如果未检测到字节顺序标记，则默认选择系统ANSI代码页。仅支持字符串变量和字符串
/