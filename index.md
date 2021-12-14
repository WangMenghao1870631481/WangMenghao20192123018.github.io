## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/WangMenghao1870631481/WangMenghao20192123018.github.io/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/WangMenghao1870631481/WangMenghao20192123018.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
#####  github创建过程
首先你需要注册一个 GitHub 账号，并在个人主界面里选择创建一个新的 Repository
![image](https://user-images.githubusercontent.com/83194177/142753045-3107dbac-8c64-4dc6-ba9c-dfaeeb5cedd0.png)

注意：进入页面后，在 Repository name 的位置填写域名，格式是 username.GitHub.io. ；例如：WangMenghao1870631481.github.io
![image](https://user-images.githubusercontent.com/83194177/142753185-e2d57883-86b6-41c4-80e5-1642a3a53bfd.png)
然后对仓库信息进行设置，仓库名必须是username.github.io的形式。

创建成功之后，点击右上角的 Settings
![image](https://user-images.githubusercontent.com/83194177/142753217-e9e4de49-45da-45c2-a442-70ca0cd14ef4.png)

注意：找到Rename下的前面的框内的内容，要改成与我们自己的github一样的；一定要记得用户名与仓库名要一致

找到 GitHub Pages 选项
![image](https://user-images.githubusercontent.com/83194177/142974681-9bf11daa-3085-497e-bd1d-b84d01d5c918.png)

注意点击黄色标记的Check it out here!按钮，进入之后会出现如下图片所示的页面
![image](https://user-images.githubusercontent.com/83194177/142753250-e4075b93-9767-484b-9469-2762b11857a9.png)

点击Change theme按钮会跳转到如下页面，这里我们就随意选择一个主题 Cayman，来看看他的效果是什么样的
![image](https://user-images.githubusercontent.com/83194177/142753293-44e90d05-5e94-4c1f-bfe3-60553bdbaccc.png)

选择完毕之后点击Select theme, GitHub Pages就会自动帮你生成好网站，在他跳转的界面点击 Commit changes按钮，网站就可以访问了。
![image](https://user-images.githubusercontent.com/83194177/142753393-5c18feb5-4a9f-4b02-957c-01c75090124c.png)

在浏览器里输入你的博客地址，比如 https://wangmenghao1870631481.github.io/WangMenghao20192123018.github.io 就可以看到，你刚刚选择的主题的个人网站的页面了。
![image](https://user-images.githubusercontent.com/83194177/142753519-9e8374c2-9367-4097-8557-708cbfb11260.png)
Thanks!
//github代码查询功能顺序图的建模说明//
顺序图建模思路：
1.按照当前交互的意图，详细地审阅相关资料(例如用例描述)，设置交互的语境，确定将要建模的工作流

2.通过识别对象在交互中扮演的角色，在顺序图的上部列出所选定的一组对象，并为每个对象设置生命线。一般把发起交互的对象放在左边。这些对象是在结构
建模中建立类图时分析得到的结果。它们可以是一般类，边界类，控制类，实体类。这里，一般类就是完成一个具体功能的类

3.对于那些在交互期间要被创建和撤销的对象，在适当的时刻，用消息箭线在它们的生命线上显式地予以说明。发送消息的对象将创建消息箭线指向被创建对象的
图标符号上。发送消息的对象将撤销消息箭线指向被撤销对象的生命线上，并标记X符号

4.在各个对象下方的生命线上，按照使用该对象操作的先后顺序排列各个代表操作的窄矩形条。从引发这个交互过程的初始消息开始，在生命线之间自顶向下依次
画出随后的各个消息

5.决定消息将怎么样或以什么样的顺序在对象之间传递。通过发起对象发出的消息，分析它需要哪些对象为它提供操作，它需要哪些对象提供操作。注意选择适当
的消息类型(调用，异步，返回，阻止，超时)，画出消息箭线，并在其上标明消息名。追踪相关的对象，直到分析完与当前语境有关的全部对象

6.两个对象的操作执行如果属于同一个控制线程，则接收者操作的执行应在发送者发出消息之后进行，并在发送消息结束之前结束。不同控制线程之间的消息有
可能在接收者的某个操作的执行过程中到达
如果需要表示消息的嵌套，或/和表示消息发生时的时间点，则采用控制焦点；如果需要，则可以对对象所执行的操作的功能及时间或空间约束进行描述；如果需要，则可以为每个消息附上前置条件和后置条件如果需要可视化消息的迭代或分支，则使用迭代或分支表示法

代码查找功能顺序图建模说明：
1.设置交互的语境，代码查询属于查询系统，包含用户，Sreach界面，Code类，code对象
2.用户是代码查询的发起者，应放在最左边，其次是搜索页面Sreach，中间包含一层逻辑层搜索的代码是要在代码库中寻找的，所以最后设置代码库
3. 在各个对象下方的生命线上，按照使用该对象操作的先后顺序排列各个代表操作的窄矩形条。从引发这个交互过程的初始消息开始，在生命线之间自顶向下依次画出随后的各个消息
4. 决定消息将怎么样或以什么样的顺序在对象之间传递。通过发起对象发出的消息，分析它需要哪些对象为它提供操作，它需要哪些对象提供操作。发起者用户要查询代码首先需要与Sreach界面之间有信息的交互，Sreach收到请求向逻辑层传递调用代码的函数，代码查询是要在代码库Code完成，Code与逻辑层应有一个消息传递调用查询代码（）
![image](https://user-images.githubusercontent.com/83194177/145943706-71a7ec78-97fc-4f33-8a88-a2a0250b91d8.png)




