# 关闭标签页

关闭网站内特定标签页。
有两种使用场景：
1. 不指定标签页，即选择器属性为空时，默认关闭当前活动标签页
2. 指定标签页，即使用“指定标签页”功能时，将关闭指定的特定标签页。使用“指定标签页”功能时，在指定过程中，指定标签页内任一元素即可选中标签页

## 属性

目标
- **选择器** ：通过提供的选择器表达式来定位目标标签页，亦可通过&quot;指定标签页&quot;自动获取，并可以进行编辑实现自定义。当此项为空时，默认关闭当前活动标签页；当通过“指定标签页”自动生成此值后，关闭指定标签页。仅支持字符串变量和字符串
- **匹配超时(毫秒)** ：定位 **选择器** 属性指定的标签页的时间，毫秒为单位。若超过此时间还未匹配到指定标签页则会抛出错误。仅支持整形变量和整形