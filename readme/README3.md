# UI组件

## 实验三

### 一、Android ListView的用法

#### （1）将要用到的图片导入到drawable下

1.1:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/1.1.png)

#### （2）新建布局作为ListView控件

1.2:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/1.2.png)

#### （3）再添加一个布局item用来接收我们的文字和图片

1.3:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/1.3.png)

#### （4）主函数内先定义我们和文字和图片数组，放入动态数组中，绑定ListView

1.4:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/1.4.png)

1.5:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/1.5.png)

#### （5）设置点击反馈，使点击时能够获取列表提示并用toast显示列表内容

1.6:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/1.6.png)

#### （6）测试布局，出来的效果就是这样

1.7:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/1.7.png)

### 二、创建自定义布局的AlertDialog

#### （1）新建一个布局用来对应用户的账号和密码

2.1:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/2.1.png)

#### （2）在main.xml布局里定义了一个按钮来对应弹出窗口

2.2:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/2.2.png)

#### （3）在主函数中载入main布局，绑定按键，设计点击反馈

2.3:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/2.3.png)

#### （4）内部是我们用alertdialog制作的弹窗

2.4:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/2.4.png)

2.5:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/2.5.png)

#### （5）测试结果，点击应用中的弹窗跳出按钮，可以输入文本，sign in会返回输入内容

2.6:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/2.6.png)

2.7:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/2.7.png)

2.8:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/2.8.png)

### 三、使用XML定义菜单

#### （1）定义一些接下来要用的标识

3.1:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/3.1.png)

#### （2）设置点击menu键（右上角三个点，无法显示的话建议换个模拟机）时的反馈，添加子菜单

3.2:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/3.2.png)

#### （3）设置被单击菜单项后的反馈

3.3:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/3.3.png)

#### （4）测试的主页面，点击右上角菜单键，显示菜单页面，子菜单内容都已实现

3.4:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/3.4.png)

3.5:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/3.5.png)

3.6:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/3.6.png)

3.7:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/3.7.png)

3.8:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/3.8.png)

3.9:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/3.9.png)

### 三、创建上下文操作模式(ActionMode)的上下文菜单

#### （1）首先创建一个main布局，用来做主界面，将listView设置为多选

4.1:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.1.png)

#### （2）接着是checkbox.xml，描述每个ListView的选项，其中都带有一张图加一个文本（安卓机器人我偷懒用了之前的cat）

4.2:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.2.png)

#### （3）menu下的菜单布局，用来设置选项菜单，这里有全选和删除两个选项（图标也可以自定义）

4.3:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.3.png)

#### （4）item类，每个选项对应的类，用来记录是否被选中

4.4:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.4.png)

#### （5）为listView自定义了一个相应的适配器，假如了notifyDataSetChanged方法用来记录实时更新，ViewHolder则是用来改变选项颜色的

4.5:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.5.png)

4.6:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.6.png)

4.7:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.7.png)

#### （6）主函数，先加载布局文件，定义相应的变量，在listView设置适配器

4.8:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.8.png)

#### （7）设置多选事件监听及动作

4.9:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.9.png)

4.10:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.10.png)

#### （8）对按钮设置各个点击事件

4.11:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.11.png)

#### （9）调用刷新方法

4.12:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.12.png)

#### （10）此时测试，我们可以看见六个选项，多选后悔显示标题并改变选项颜色

4.13:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.13.png)

4.14:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/third/4.14.png)

### 参考文献：

1.https://developer.android.google.cn/guide/topics/ui/menus.html#java

2.https://blog.csdn.net/qq_39824472/article/details/90549797

