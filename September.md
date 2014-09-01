#### 09.01
遇到这个问题
Popovers cannot be presented from a view which does not have a window
so上面看到收藏

[CABasicAnimation animationWithKeyPath:@"position"];

animationWithKeyPath后面的属性不能随便填，它必须是CALayer的某项属性，你下面写的代码才会对应的去执行改变该属性的效果。

animationWithKeyPath的值：

opacity
margin
zPosition
backgroundColor
cornerRadius
borderWidth 
bounds
contents
contentsRect
cornerRadius
frame
hidden
mask
masksToBounds
opacity
position
shadowColor
shadowOffset
shadowOpacity
shadowRadius
