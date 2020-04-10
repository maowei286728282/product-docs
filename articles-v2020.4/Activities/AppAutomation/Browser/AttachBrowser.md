# 绑定浏览器

提供Scope容器，使你可以附加到已打开的浏览器并在其中执行多个操作。使用录屏时，将自动生成此组件

## 属性
基本
- **显示名称** ：默认为该组件的名称。支持更改，用户自定义此组件的显示名称
- **失败后继续** ：设置当此组件运行失败时，是否忽略此错误继续运行下一个组件。下拉框选择，当选择"是"时，如果该组件运行时遇到错误，该流程也会继续执行下一个组件，并不会停止；当选择"否"时，如果该组件运行时遇到错误，该流程将会停止执行并抛出错误
- **前延时(毫秒)** ：指定在此组件执行前的等待时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为上一个组件执行完毕后，等待一秒钟后执行此组件
- **后延时(毫秒)** ：指定在此组件执行后的延迟时间。单位为毫秒（ms）,1000ms = 1s。若此处填写1000，意为此组件执行完毕后，等待一秒钟后执行下一个组件

输入

- **浏览器类型** ：绑定的目标浏览器类型，例Chrome，IE
- **浏览器** ：通过此变量来指定需要绑定的浏览器，此项输入可为其他浏览器活动的输出（当此项被填充时，浏览器类型和选择器不产生效力）

目标
- **[选择器](../../Appendix/Selector.md)** ：通过提供的选择器表达式来定位目标浏览器，可通过"指定浏览器"自动获取，并可以进行编辑实现自定义。仅支持字符串变量和字符串
- **匹配超时(毫秒)** ：限定查找目标元素时间，超出指定时间后将不再等待。若超过此时间还未匹配到指定元素则会抛出错误。单位为毫秒（ms）,1000ms = 1s。仅支持整型变量和整型

输出

- **浏览器** ：将绑定的浏览器类型对象存储到此变量，可作为下一浏览器活动的输入

可选项

- **最大化** ：勾选时，可以自动将你指定的浏览器最大化进行后续操作
- **结束后关闭** ：勾选时，将在此组件结束后自动关闭浏览器