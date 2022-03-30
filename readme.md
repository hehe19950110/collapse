collapse折叠面板（手风琴效果）

1、overflow这个选项包含剪切，显示滚动条，或者显示从容器溢出到周围区域的内容。
指定除visible(默认值)以外的值将创建一个新的块级格式化上下文。这在技术层面上是必须的：如果一个浮动元素和滚动条相交，它会在每个滚动步骤后强行重新包装内容，从而导致慢滚动体验。
为使 overflow 有效果，块级容器必须有一个指定的高度！！！（height或者max-height）或者将white-space设置为nowrap。

 { overflow: hidden; /* 内容将被剪裁以适合填充框；不显示滚动条 */  }
 
 { overflow: scroll; /* 内容将被剪裁以适合填充框；浏览器显示滚动条，无论是否实际剪切了任何内容，始终显示滚动条 */  }
 
 2、小标题右边的^
 先画出两条线构成的一个直角，而后再旋转，得到想要的图案。
```
border-top: 1px solid #666;
border-right: 1px solid #666;
 
transform: rotate(45deg); /* 旋转45度 */ 
```
rotate()函数定义了一种将元素围绕一个定点（由transform-origin属性指定）旋转而不变形的转换。
指定的角度定义了旋转的量度。若角度为正，则顺时针方向旋转，否则逆时针方向旋转。
