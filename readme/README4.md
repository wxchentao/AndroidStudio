# Intent

## 实验四

### 一、获取URL地址并启动Intent的调用

#### （1）先在main.java里定义好视图main.xml里的按钮和EditText组件

1.1:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/1.1.png)

#### （2）在按钮里设置点击监听，动作就是获取editText的内容，解析为uri对象传入隐式intent来调用

1.2:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/1.2.png)

#### （3）这就是运行后的界面

1.3:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/1.3.png)

#### （4）点击按钮能看到隐式intent自动匹配了多个浏览器供人选择

1.4:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/1.4.png)

#### （5）此时选择谷歌浏览器，可以看见出现的百度界面（记得打开模拟器的WiFi）

1.5:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/1.5.png)

### 二、新建一个工程使用WebView来加载URL 

#### （1）新建一个工程，在新布局中定义webview组件

2.1:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/2.1.png)

#### （2）在新工程里创建browsersActivity.java，加载新布局，新建intent，data参数和url

2.2:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/2.2.png)

#### （3）将获得参数传入url对象中，设置了捕获错误，然后重写方法使其用webview加载网页

2.3:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/2.3.png)

#### （4）回到上一个工程里，在AndroidManifest.xml文件中设置intent过滤器，为了让选择浏览器时能看到我们的自定义browser。其中一个uses-permission用来使用网络，usesCleartextTraffic设为true。然后安装应用

2.4:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/2.4.png)

2.5:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/2.5.png)

#### （5）测试结果，点击按钮可以出现多个浏览器选择，选择了自定义的浏览器，但是没显示，是网络没设置好的原因，我上次有用，这会不知道怎么没法显示了，据说清除一下模拟器的数据就好

2.6:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/2.6.png)

2.7:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/fourth/2.7.png)

### 参考文献：

1.https://blog.csdn.net/warmandfull/article/details/105885905

