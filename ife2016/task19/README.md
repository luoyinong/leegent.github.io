# 任务十九

有一个任务要求用竖条高度表示数字大小，即画一幅条形图。

### 碰到的困难
如何让竖条从表示作图区域div的底边向上延长？因为正常文档流，以及float，都是从上向下排列的，即竖条都是顶对齐。
### 解决思路
给每个竖条套一个宽度与竖条相同、高度与作图区域相同的div（称为“竖框”），将竖条放在里面，竖框float布局，竖条relative布局，并向下移动 竖框高度-自身高度 的距离。搞定！
### 后来得知
用flex布局可以轻松解决这个问题！