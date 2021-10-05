main axis: [横着的] 	cross axis: [竖着的]  方向有变动的

main size					cross size

flex 容器：`display: flex`

1. `flex-direction: row |row-reverse|column|column-reverse`主轴方向; main axis in row is horizontal; main axis in column is vertical

2. `flex-wrap: nowrap|wrap|wrap-reverse` 是否可以换行

3. `flex-flow: <flex-direction> <flex-wrap>`

4. `justify-content` 项目在主轴的对齐方式：

   1. flex-start 左对齐    flex-end 右对齐    center 对着主轴居中
   2. space-between 两端对齐，项目间的间隔相等
   3. space-around 项目之间的间隔比项目对边缘的间隔大一倍，项目间的间隔相等

5. `align-items` 项目在cross axis上的对齐方式

   1. stretch/ auto: 假设容器高度设置为 100px，而项目都没有设置高度的情况下，则项目的高度也为 100px；

      假如设置了容器高度 以及项目高度，根据项目高度走

   2. `flex-start` `flex-end` `center`

   3. `baseline` 项目第一行文字的基线对齐

      ![img](https://pic3.zhimg.com/80/v2-abf7ac4776302ad078986f7cd0dddaee_1440w.jpg)

6. `align-content` 

   当`flex-wrap: nowrap`时候， 容器仅存在一根轴线，就不会产生多条轴线。
   当`flex-wrap: wrap` 时候，需要调整各个轴线的对齐方式

   1. `flex-start` `flex-end` `center`
   2. `space-between`   `space-around`

flex项目属性

1. `order：<int>` 项目在容器中的排列顺序，数值越小，排列越靠前

2. `flex-basis` `flex-grow` `flex-shrink` 配合使用;

3. `flex-grow: <int>` 定义项目的放大比例。项宽度和不及父容器宽度时，flex-grow 会起作用

   当此值为0时，空间足够时，不放大

   1. `flex-shrink` 定义项目的缩小比例，负值无效；

      当此值为0时，空间不足时，不缩小

4. `flex: <flex-grow> <flex-shrink> <flex-basis>`

5. `align-self:` 允许单个项目与其他项目有不一样的对齐方式

   1. `auto` `flex-start` `flex-end` `center`
   2. `baseline` `stretch`