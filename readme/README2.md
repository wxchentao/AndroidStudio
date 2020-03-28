# Android布局

## 实验二

## 前提：已经安装AndroidStudio3.5

### 一、利用线性布局实现实验要求中的界面

#### （1）新建一个虚拟设备用于测试

1.1:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/1.1.png)

#### （2）查看一下能否正常登陆，我的是系统4.1的x86模拟器

1.2:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/1.2.png)

#### （3）在主函数中找到这个，注意activity_main，等会要修改成我们要显示的布局

1.3:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/1.3.png)

#### （4）新建一个线性布局，我命名为layout

1.4:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/1.4.png)

1.5:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/1.5.png)

#### （5）我的写法是将按钮一个一个的实现，并且命名（也有使用数组动态输入的方法，但是太麻烦了）。而线性布局是只有垂直和水平分布，所以要做到整齐排列要用到两种布局交叉嵌套（比如外面是垂直，每行加个水平），和等比权重layout_weight（都设成1就能保证布局齐整）。

1.7:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/1.7.png)

#### （6）准备测试布局，在主函数中修改成要测试的布局layout

1.8:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/1.8.png)

#### （7）这是我们模拟器上跑出来的画面，虽然字体大了一点，但是其他都没有问题，测试完成

1.9:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/1.9.png)

### 二、利用ConstraintLayout实现实验要求中界面

#### （1）constrainlayout同样是基于线性布局，新建一个布局

2.1:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/2.1.png)

#### （2）排版上仍旧套用了一里的交叉嵌套，与其不同的是这里加入了background背景板颜色，参数是RGB颜色值。使用padding和margin可以适当的调节按钮位置。

2.2:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/2.2.png)

#### （3）实验要求中最后一行的按钮贴合底部，这时候就要把height参数改成match_parent，即最大尺寸了。

2.3:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/2.3.png)

#### （4）准备测试constrainlaylout

2.4:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/2.4.png)

#### （5）测试结果~很漂亮。

2.5:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/2.5.png)

### 三、利用表格布局实现实验要求中界面

#### （1）表格布局也是基于线性布局，新建一个tablelayout

3.1:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/3.1.png)

#### （2）先是基础的填充完表格。表格布局的API中是不提供行着色的方法的，所以为了在行中分割，我的做法是添加一行灰色的细线。然后对于左边的空余，使用marginLeft函数来调整距离。

3.2:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/3.2.png)

#### （3）这是在预览中的图像，看起来大致都完成了

3.3:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/3.3.png)

#### （4）准备测试

3.4:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/3.4.png)

#### （5）测试出来的结果差别太大了……我的字体太大了，即使我已经使用了dp这个像素单位

3.5:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/3.5.png)

#### （6）重新调整了一下字体

3.6:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/3.6.png)

#### （7）现在显示的就正常多了，至于X import的不对齐，是因为我是手动对齐的，字体一改又变了……不管了，是小问题。

3.7:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/second/3.7.png)



### 参考文献：

1.https://developer.android.google.cn/guide/topics/ui/declaring-layout.html#java

2.https://blog.csdn.net/u013372185/article/details/29186301

