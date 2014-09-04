
#### 09.03
昨天第一次坐uber，今天早上又坐了一次差价还蛮大差不多10元估计是算在时间上的价格
http://chabudai.org/blog/?p=59，这个网站承载了年轻时候的我一个思念
其实刚到杭州的时候25－26间，我还是愤日的思想，尤记得当时店里有个大学生学日语准备毕业去日本恰逢日本大海啸，当时还极力诋毁劝阻这样的行为，虽然在28左右有发过一次留言给她鼓励她去这样

CABasicAnimation fillMode和removedOnCompletion 这两个参数的区别
rotationAnimation.removedOnCompletion = NO;
rotationAnimation.fillMode = kCAFillModeForwards;
fillMode的作用就是决定当前对象过了非active时间段的行为. 比如动画开始之前,动画结束之后。如果是一个动画CAAnimation,则需要将其removedOnCompletion设置为NO,要不然fillMode不起作用.

下面来讲各个fillMode的意义 
kCAFillModeRemoved 这个是默认值,也就是说当动画开始前和动画结束后,动画对layer都没有影响,动画结束后,layer会恢复到之前的状态 
kCAFillModeForwards 当动画结束后,layer会一直保持着动画最后的状态 
kCAFillModeBackwards 这个和kCAFillModeForwards是相对的,就是在动画开始前,你只要将动画加入了一个layer,layer便立即进入动画的初始状态并等待动画开始.你可以这样设定测试代码,将一个动画加入一个layer的时候延迟5秒执行.然后就会发现在动画没有开始的时候,只要动画被加入了layer,layer便处于动画初始状态 
kCAFillModeBoth 理解了上面两个,这个就很好理解了,这个其实就是上面两个的合成.动画加入后开始之前,layer便处于动画初始状态,动画结束后layer保持动画最后的状态.

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
