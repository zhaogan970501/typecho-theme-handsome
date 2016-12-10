![pic.png][1]

# 版本： 1.3.1

11月份的时候就一直开始写这个主题了，主题原型来自收费静态html模板angulr，是一套国外开发的主题。界面十分友好，扁平化设计。主要css来自于静态html模板，自己写了部分js和php代码。功能十分强大，**总体积除去图片不足400K**。


## 主题特色

1. 主题使用instantclick.js ，鼠标悬浮在链接上即可预加载页面，速度提升。
2. 主题使用bootstrap框架,自适应任何屏幕尺寸。在手机端仍然界面友好。
3. 主题内置**3套自定义页面模板**，**4种布局**、**14种风格**，每一处的颜色，随意改变，随心打造你想要的风格界面。
4. 主题内置三套自定义页面模板——“时光机”和“文章归档”和“友情链接”。
5. “时光机”——类似于 **说说**，方便记录生活的一言一语，并且在首页会显示最新三条。
6. “文章归档”——页面使用时间线的css风格，美观好看
7. 全站有各种小部件，如“热门文章”、“最新评论”、“随机文章”、“标签云”，满足大多数的需求。
7. 前台可以登录，注销，操作方便。
8. 首页文章缩略图功能，输出顺序分别书:thumb字段——附件第一个图片——文章插入第一张图片——随机输出缩略图
9. 使用`links`插件，管理友情链接更简单！
10. 强大的后台功能，在这里，设置一切你想改动的。
11. 使用阿里妈妈iconfont图标，简单轻巧。

![2.png][2]

## <span style="color: rgb(255, 0, 0);">使用必看</span>

一定要看的哦！不然，百分百会出错！

1. 主题文件夹重命名成“handsome”哦！
2. 启用主题后必须要新建"时光机"独立页面（具体设置方法见`使用攻略`第三点），否则，启用后，页面是错位的！
3. 使用`原生评论`，请关闭后台的**反垃圾保护**和**检查评论来源页 URL 是否与文章链接一致**（后台设置——评论）
4. 添加第三方统计代码（如CNZZ、google analysis）不需要`<script></script>` 标签，直接把js代码复制到设置框就可以！否则会发生错误！！
5. 请设置**合适的**评论回复层数（由于每回复一次，都会向右缩进一定距离，设置太多，手机端会有样式问题）：后台——设置——评论——回复层数（建议4—6）。
6. 建议开启伪静态，否则可能出现未知错误：后台——设置——永久链接——是否使用地址重写功能（选择是）
7. 不提供QQ自定义服务，有任何问题或者bug或者建议可以提交issue、评论或者email（ihewro@163.com）,十分欢迎~


## 使用攻略

首先，从github上面下载最新版本的[handsome](https://github.com/ihewro/typecho-theme-handsome/)主题！重命名主题文件夹为`handsome`。你会看到一个**`插件`**的文件夹。把里面的两个插件文件夹复制到usr\plugins目录下。最后删除主题文件夹下面的**`插件`**文件夹即可。

> 独立页面的自定义模板

主题内置了三套自定义模板`时光机`、`文章归档`、`友情链接`。在后台了**撰写——创建页面**的右下角的`自定义模板`的下拉框里就可以看到哦！简单介绍一些使用方法：

* 时光机: 填写地址的时候，必须填写为 <span style="color: rgb(255, 255, 255); background-color: rgb(250, 192, 143);">cross</span>.html 。内容框里面不用填任何东西，这个页面在前台就可以发布“说说”，用来记录你的日常和心情的~
* 文章归档： 地址随意填写。内容框不用填任何内容。这个页面会自动把你所有文章用时间树的形式显示出来。
* 友情链接：地址随意填写。这个页面自动输出`links`插件里面设置的友情链接。（**links插件用法**见下第三点）如果你还想输出额外内容（比如友链要求等等），直接在内容框中填写就行。该页面会一起输出这部分内容。


> 插件设置

handsome的完整使用依赖了两个外部插件（插件后续版本会精简不必要的功能，并整合成一个插件，目前，先这样用着吧~）：BufannaoCms 和 Links。简单介绍一些用法。

* BufannaoCms：是用来调用右侧边栏的`热门文章`和`随机文章`这两个功能的。启用后，进入插件设置里面，只需要设置**`随机文章数量`** 和 **`热评文章数量`** 这两项即可。其他项不用设置的。

* Links：是一个管理友情链接的插件。首页的左侧边栏的`友链`栏目和独立页面中的自定义模板`友情链接`会调用这里面设置的友情链接。启用该插件后，`后台`——`管理`栏目下会多一个`友情链接`的栏目，进入后，添加一个链接，只需要填写`链接名称`、`链接地址`、`链接分类`、 `链接描述`这四个项目的内容。关于`链接分类`的说明：

    * `ten`：是全站链接，就是在首页的左侧边栏展示的
    * `one`：是内页链接，在独立页面中的自定义模板`友情链接`中显示


## 推荐插件

除了主题必须使用的两个插件外，以下插件与本主题完全兼容。我也一直在使用啦~

1. [AutoTags](https://dt27.org/php/autotags-for-typecho/)：标签自动生成插件
2. [CommentToMail](http://typecho.byends.com/post/CommentToMail-v2-0-0.html)：评论邮件提醒插件
3. [QNUpload](http://ysido.com/qnupload_v_1_2_0.html)：七牛 附件上传插件，来自兜兜的BAE插件...
4. [SmartSpam](http://www.yovisun.com/archive/typecho-plugin-smartspam.html)：智能评论过滤器，让机器人彻底远离你！


## 下载地址

<https://github.com/ihewro/typecho-theme-handsome/>（**使用版**）

<https://github.com/ihewro/typecho-theme-handsome-dev/>（**开发版**）

主题分为两个版本：**开发版**和**使用版**。
两者**功能完全相同**，但是**开发版**完全保留了未压缩代码并且使用npm配置了grunt自动压缩任务，更方便修改代码。**使用版**文件精简到极致，更适合正式使用！为了减轻负担，**开发版**只会在版本号`x.y.z`的`y`位变动时候才会同步更新。

## 版权声明

1. 在主题代码注释中尽量把引用代码来源注明清楚，一并感谢。
    * 主题后台界面风格来自[`material主题`](https://viosey.com/)
    * 主题function.php部分代码来自 [`qqdie`](http://qqdie.com)
    * 感谢 links插件作者 [`寒泥`](http://www.imhan.com/)
    * 主题cross自定义模板代码来自 [`breeze主题`](https://shansing.com/)by闪闪的星
2. 主题只会在电脑版的右下页脚有一个版权信息，手机端是是隐藏掉的，所以希望保留页脚版权信息啦，否则我会伤心


  [1]: http://7xlk7n.com1.z0.glb.clouddn.com/2016/12/2960973115.png
  [2]: http://7xlk7n.com1.z0.glb.clouddn.com/2016/12/2223020222.png
