
#### 09.03
昨天第一次坐uber，今天早上又坐了一次差价还蛮大差不多10元估计是算在时间上的价格
http://chabudai.org/blog/?p=59，这个网站承载了年轻时候的我一个思念
其实刚到杭州的时候25－26间，我还是愤日的思想，尤记得当时店里有个大学生学日语准备毕业去日本恰逢日本大海啸，当时还极力诋毁劝阻这样的行为，虽然在28左右有发过一次留言给她鼓励她去这样

#### 09.02
习惯哦，要命，近日总是稍晚才睡各种youtube很晚
cabasicanimation 主要是受限于两个点，开始和结束点，有layer隐式动画和uiview animation 可以替代
cakeyframeanimation强大没有相关的uikit接口可以代替 

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
