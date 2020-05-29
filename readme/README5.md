# NotePad笔记本应用

## 期中作业

### 前提：**本实验将基于**NotePad应用做功能扩展（源码地址：https://github.com/llfjfz/NotePad）

### 一、NoteList中显示条目增加时间戳显示

#### （1）在noteslist_item.xml中添加TextView作为修改时间的显示布局

1.1:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/1.1.png)

#### （2）注意nodepad.java中是否有声明时间变量，没有则添加

1.2:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/1.2.png)

#### （3）在NotesEditor.java中添加函数以获取当前时间，再修改NotesEditor.java中的updateNote，调用时间函数后将参数添加

1.21:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/1.21.png)

1.3:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/1.3.png)

#### （4）对NoteList.java里的PROJECTION进行修改，添加我们的时间对象

1.4:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/1.4.png)

#### （5）修改对应的dataColumns和viewIDs，添加我们的时间参数和布局元素

1.5:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/1.5.png)

1.6:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/1.6.png)

#### （6）此时就可以显示时间戳了

1.9:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/1.9.png)

### 二、添加笔记查询功能（根据标题查询）

#### （1）新建一个布局main.xml用来显示搜索列表

2.1:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/2.1.png)

#### （2）为了改写listview，将NoteList.java的继承类修改，并声明list

2.2:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/2.2.png)

#### （3）将设置list的方法进行修改

2.3:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/2.3.png)

2.4:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/2.4.png)

#### （4）先调用SearchView定义，为接下来的改写用，随后在OnCreate类下加载main.xml，然后用findviewbyid获取

2.5:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/2.5.png)

2.6:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/2.6.png)

#### （5）万事俱备，在下面添加SearchView函数

2.7:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/2.7.png)

2.8:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/2.8.png)

#### （6）一输入就匹配了

2.9:![Alt](https://github.com/wxchentao/AndroidStudio/blob/master/images/mid/2.9.png)

### 参考文献：

1.https://github.com/helang0616/Android-develop/tree/master/

2.https://stackoverflow.com/questions/32061365/crash-compile-attempt-to-invoke-virtual-method-void-android-widget-listview-se

3.https://developer.android.google.cn/guide/topics/data/data-storage

