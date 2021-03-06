#前端插件资源整理
从入坑写代码到现在差不多一年了,当初很菜,现在还是很菜,不过总是每天都比前一天好,很享受这种状态,入坑时先进入的是前端领域,所以记录下自己做开发以来在前端领域发现并试用过的一些在自己看来不错的插件,作为自己一个阶段的集合,仅作为个人参考,如大神们发现坑的地方,欢迎指正!

---
* **[1.font-awesome-最实用的web字体图标库](https://astronautweb.co/snippet/font-awesome/)**
* **[2.chosen-强大的jquery模拟下拉框(select)插件](http://www.vaikan.com/docs/Chosen/Chosen.htm)**
* **[3.Sweet Alert-js超酷消息警告框插件](http://www.dglives.com/demo/sweetalert-master/example/)**
* **[4.echarts-可视化图标插件](http://echarts.baidu.com/echarts2/)**
* ** [5.Swiper-滑动特效插件](http://www.swiper.com.cn/)**(pc)
* **[6.iScroll-实现下拉刷新，滚动翻页特效的JQuery插件](http://iscrolljs.com/)**
* **[7.loader.css-css动画加载特效](https://connoratherton.com/loaders)**
* **[8.VEX-小而美的jquery-css动画消息警告库](http://github.hubspot.com/vex/docs/welcome/)**
* **[9.fancyBox-图片展示插件](http://fancyapps.com/fancybox/)**
* **[10.jPlayer-基于HTML5/Flash的音频、视频播放器-适配移动端](http://www.jplayer.cn/)**
* **[11.Rome-可定制的JS期与时间选择器-PC端](http://bevacqua.github.io/rome/)**
* **[12.Mobiscroll-移动端日期时间滑动、滚动插件-可以各种自定义](http://demo.mobiscroll.com/)**
* **[13.kindeditor-一款可定制性极高的富文本编辑器](https://kindeditor.codeplex.com/)**
* **[14.jPages-强大的客户端分页插件](http://www.jq22.com/yanshi283)**
* **[15.projekktor-UI漂亮的一款HTML5播放器](http://www.projekktor.com/)**
* **[16.touchSlide-滑动特效插件](http://www.superslide2.com/)(mobile)**
* **[17.移动端事件模拟封装库](https://github.com/chenmnkken/monoevent)**
* **[18.elegant_font-炫的飞起的字体图标库](http://www.elegantthemes.com/blog/resources/elegant-icon-font/)**

---

#以下是具体部分

**[1.font-awesome-最实用的web字体图标库](https://astronautweb.co/snippet/font-awesome/)**

**这个东西貌似有html也有css字体,有点蒙圈**

* **github star:41000+**
* **github fork:7000+**


* **[demo](http://fontawesome.io/)**
* **[github](https://github.com/FortAwesome/Font-Awesome)**


---
 
**[2.chosen-强大的jquery模拟下拉框(select)插件](http://www.vaikan.com/docs/Chosen/Chosen.htm)**

* **github star:19000+**
* **github fork:3700+**


**Chosen 是一个JavaScript插件，它能让丑陋的、很长的select选择框变的更好看、更方便。目前，它支持 jQuery 和 Prototype 两种JavaScript引擎。**

1.引入jquery库和脚本
```js
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js" type="text/javascript"></script>
<script src="chosen/chosen.jquery.js" type="text/javascript"></script> 
```

2.选择框html片段
```html
<select class="chzn-select" data-placeholder="Choose a Country" style="width:350px;" tabindex="1">
       <option value=""></option> 
       <option value="United States">United States</option> 
       <option value="United Kingdom">United Kingdom</option> 
       <option value="Afghanistan">Afghanistan</option> 
       <option value="Albania">Albania</option> 
                 ...
</select>
```

3.初始化组件

```js
$(".chzn-select").chosen();
```
* **[demo](http://www.vaikan.com/docs/Chosen/Chosen.htm)**
* **[github地址](https://github.com/harvesthq/chosen/)**


 ---
 
 **[3.Sweet Alert-js超酷消息警告框插件](http://www.dglives.com/demo/sweetalert-master/example/)**

* **github star:13000+**
* **github fork:1600+**


**SweetAlert是一款神奇的javascript弹出消息警告框插件。**

1.要使用该插件，首先要在html的header中引入以下文件
```html
<script src="lib/sweet-alert.min.js"></script>
<link rel="stylesheet" type="text/css" href="lib/sweet-alert.css">

```
2.最基本的调用方法：

```js
sweetAlert("Hello world!");
```

3.带错误图标的警告框：

```js
sweetAlert("Oops...", "Something went wrong!", "error");
```
4.一个带有确认按钮的警告框，点击确认按钮可触发动画：

```js
sweetAlert({
  title: "Are you sure?",
  text: "You will not be able to recover this imaginary file!",
  type: "warning",
  showCancelButton: true,
  confirmButtonColor: "#DD6B55",
  confirmButtonText: "Yes, delete it!",
  closeOnConfirm: false
}, function(){
  swal("Deleted!",
  "Your imaginary file has been deleted.",
  "success");
});
```

* **[demo](http://www.dglives.com/demo/sweetalert-master/example/)**
* **[github](https://github.com/t4t5/sweetalert)**

亲测:UI很漂亮

---

**[4.echarts-可视化图标插件](http://echarts.baidu.com/echarts2/)**

* **github star:11000+**
* **github fork:4000+**

**5分钟上手写ECharts的第一个图表**


1、新建一个echarts.html文件，为ECharts准备一个具备大小（宽高）的Dom。

```html
<!DOCTYPE html>
<head>
    <meta charset="utf-8">
    <title>ECharts</title>
</head>

<body>
    <!-- 为ECharts准备一个具备大小（宽高）的Dom -->
    <div id="main" style="height:400px"></div>
</body>
```
2、新建script标签引入模块化单文件echarts.js.

```html
<!DOCTYPE html>
<head>
    <meta charset="utf-8">
    <title>ECharts</title>
</head>
<body>
    <!-- 为ECharts准备一个具备大小（宽高）的Dom -->
    <div id="main" style="height:400px"></div>
    <!-- ECharts单文件引入 -->
    <script src="http://echarts.baidu.com/build/dist/echarts.js"></script>
</body>
```

3.新建script标签中为模块加载器配置echarts和所需图表的路径（相对路径为从当前页面链接到echarts.js）

```html
<!DOCTYPE html>
<head>
    <meta charset="utf-8">
    <title>ECharts</title>
</head>
<body>
    <!-- 为ECharts准备一个具备大小（宽高）的Dom -->
    <div id="main" style="height:400px"></div>
    <!-- ECharts单文件引入 -->
    <script src="http://echarts.baidu.com/build/dist/echarts.js"></script>
    <script type="text/javascript">
        // 路径配置
        require.config({
            paths: {
                echarts: 'http://echarts.baidu.com/build/dist'
            }
        });
    </script>
</body>
```

4、script标签内动态加载echarts和所需图表，回调函数中可以初始化图表并驱动图表的生成.

```html
<!DOCTYPE html>
<head>
    <meta charset="utf-8">
    <title>ECharts</title>
</head>
<body>
    <!-- 为ECharts准备一个具备大小（宽高）的Dom -->
    <div id="main" style="height:400px"></div>
    <!-- ECharts单文件引入 -->
    <script src="http://echarts.baidu.com/build/dist/echarts.js"></script>
    <script type="text/javascript">
        // 路径配置
        require.config({
            paths: {
                echarts: 'http://echarts.baidu.com/build/dist'
            }
        });
        
        // 使用
        require(
            [
                'echarts',
                'echarts/chart/bar' // 使用柱状图就加载bar模块，按需加载
            ],
            function (ec) {
                // 基于准备好的dom，初始化echarts图表
                var myChart = ec.init(document.getElementById('main')); 
                
                var option = {
                    tooltip: {
                        show: true
                    },
                    legend: {
                        data:['销量']
                    },
                    xAxis : [
                        {
                            type : 'category',
                            data : ["衬衫","羊毛衫","雪纺衫","裤子","高跟鞋","袜子"]
                        }
                    ],
                    yAxis : [
                        {
                            type : 'value'
                        }
                    ],
                    series : [
                        {
                            "name":"销量",
                            "type":"bar",
                            "data":[5, 20, 40, 10, 10, 20]
                        }
                    ]
                };
        
                // 为echarts对象加载数据 
                myChart.setOption(option); 
            }
        );
    </script>
</body>
```


5.浏览器中打开echarts.html,就能看到效果

* **[demo](http://echarts.baidu.com/echarts2/doc/example.html)**
* **[github](https://github.com/ecomfe/echarts)**

---

 **[5.Swiper-滑动特效插件](http://www.swiper.com.cn/)**(pc)

* **github star:7700+**
* **github fork:2800+**


* **Swiper是纯javascript打造的滑动特效插件，面向手机、平板电脑等移动终端。**
* **Swiper能实现触屏焦点图、触屏Tab切换、触屏多图切换等常用效果.**
* **Swiper开源、免费、稳定、使用简单、功能强大，是架构移动终端网站的重要选择！**



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>Swiper demo</title>
    <!-- Link Swiper's CSS -->
    <link rel="stylesheet" href="../dist/css/swiper.min.css">

    <!-- Demo styles -->
    <style>
    body {
        background: #eee;
        font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
        font-size: 14px;
        color:#000;
        margin: 0;
        padding: 0;
    }
    .swiper-container {
        width: 500px;
        height: 300px;
        margin: 20px auto;
    }
    .swiper-slide {
        text-align: center;
        font-size: 18px;
        background: #fff;
        
        /* Center slide text vertically */
        display: -webkit-box;
        display: -ms-flexbox;
        display: -webkit-flex;
        display: flex;
        -webkit-box-pack: center;
        -ms-flex-pack: center;
        -webkit-justify-content: center;
        justify-content: center;
        -webkit-box-align: center;
        -ms-flex-align: center;
        -webkit-align-items: center;
        align-items: center;
    }
    </style>
</head>
<body>
    <!-- Swiper -->
    <div class="swiper-container">
        <div class="swiper-wrapper">
            <div class="swiper-slide">Slide 1</div>
            <div class="swiper-slide">Slide 2</div>
            <div class="swiper-slide">Slide 3</div>
            <div class="swiper-slide">Slide 4</div>
            <div class="swiper-slide">Slide 5</div>
            <div class="swiper-slide">Slide 6</div>
            <div class="swiper-slide">Slide 7</div>
            <div class="swiper-slide">Slide 8</div>
            <div class="swiper-slide">Slide 9</div>
            <div class="swiper-slide">Slide 10</div>
        </div>
    </div>

    <!-- Swiper JS -->
    <script src="../dist/js/swiper.min.js"></script>

    <!-- Initialize Swiper -->
    <script>
    var swiper = new Swiper('.swiper-container');
    </script>
</body>
</html>
```


* ** [demo](http://www.swiper.com.cn/demo/index.html)**
* ** [demo2](http://idangero.us/swiper/#.VwT6zxN94cg)**
* ** [github地址](https://github.com/nolimits4web/Swiper)**


---

**[6.iScroll-实现下拉刷新，滚动翻页特效的JQuery插件](http://iscrolljs.com/)**

**iScroll是一款用于移动设备web开发的一款插件。像缩放、下拉刷新、滑动切换等移动应用上常见的一些效果都可以轻松实现。**

* **github star:7200+**
* **github fork:2100+**

```js
<script type="application/javascript" src="/Admin/News/edit/id/iscroll.js"></script>
<script type="text/javascript">
    var myScroll;
    function loaded() {
        myScroll = new iScroll('wrapper');
    }
    document.addEventListener('DOMContentLoaded', loaded, false);
</script>
```
**曾用iScroll实现在安卓手机上触摸滚动兼容性问题**

* **[demo](http://iscrolljs.com/)**
* **[github](https://github.com/cubiq/iscroll/)**

---


**[7.loader.css-css动画加载特效](https://connoratherton.com/loaders)**

* **github star:6000+**
* **github fork:680+**

**Loaders.css是一款非常出色的加载动画框架，Loaders.css利用纯CSS可以实现很多种样式的Loading加载动画，这些动画并不需要图片来辅助，而是仅仅需要CSS即可实现，因此运行效率比较不错。**

**Loaders.css的特点**

* **基于纯CSS，不需JavaScript脚本，也不需要图片，很干净。
默认提供近30个不同的Loading动画效果，你也可以发挥自己的想象来实现不同的加载动画。**
* **Loaders.css比较轻巧，基本没什么臃肿的文件。
免费、开源，这是必须的。**

1.引入 loaders.min.css 和 loaders.css.js，这个JS仅是为了简化动画的DIV标签，如果不加这个JS，那么你的动画就必须加上对应数量DIV标签才能正常显示动画，所以建议加上，这样语义化好会好些。

```html
<link rel="stylesheet" type="text/css" href="loaders.min.css">
<script type="text/javascript" src="loaders.css.js"></script>
```
2.HTML代码，给loading元素加入动画class

```html
<div class="loader-inner ball-pulse"></div>
```
3.改变加载动画颜色

```css
.ball-grid-pulse > div {
 background: orange;
}
```
* ** [demo](https://connoratherton.com/loaders)**
* ** [github地址](https://github.com/ConnorAtherton/loaders.css)**


---

**[8.VEX-小而美的jquery-css动画消息警告库](http://github.hubspot.com/vex/docs/welcome/)**

* **github star:5000+**
* **github fork:300+**

**可用作幻灯片样式**


1.引入文件

```js
<script src="vex.combined.min.js"></script>
<script>vex.defaultOptions.className = 'vex-theme-os';</script>
<link rel="stylesheet" href="vex.css" />
<link rel="stylesheet" href="vex-theme-os.css" />
```


2  
```js
vex.dialog.confirm
    message: 'Are you absolutely sure you want to destroy the alien planet?'
    callback: (value) ->
        console.log if value then 'Successfully destroyed the planet.' else 'Chicken.'
```

* **[demo](http://github.hubspot.com/vex/docs/welcome/)**
* **[github](https://github.com/HubSpot/vex)**


---

**[9.fancyBox-图片展示插件](http://fancyapps.com/fancybox/) **
  
* **github star:3600+**
* **github fork:1000+**
  
**Fancybox是一款优秀的jquery插件，它能够展示丰富的弹出层效果。前面我们有文章介绍了facybox弹出层效果，相比facybox，fancybox显得功能更为齐全，它除了可以加载DIV，图片、图片集、Ajax数据，还能加载SWF影片，iframe页面等等。**


```js
<!-- Add jQuery library -->
<script type="text/javascript" src="http://code.jquery.com/jquery-latest.min.js"></script>

<!-- Add mousewheel plugin (this is optional) -->
<script type="text/javascript" src="/fancybox/lib/jquery.mousewheel-3.0.6.pack.js"></script>

<!-- Add fancyBox -->
<link rel="stylesheet" href="/fancybox/source/jquery.fancybox.css?v=2.1.5" type="text/css" media="screen" />
<script type="text/javascript" src="/fancybox/source/jquery.fancybox.pack.js?v=2.1.5"></script>

<!-- Optionally add helpers - button, thumbnail and/or media -->
<link rel="stylesheet" href="/fancybox/source/helpers/jquery.fancybox-buttons.css?v=1.0.5" type="text/css" media="screen" />
<script type="text/javascript" src="/fancybox/source/helpers/jquery.fancybox-buttons.js?v=1.0.5"></script>
<script type="text/javascript"![](fancyBox.png) src="/fancybox/source/helpers/jquery.fancybox-media.js?v=1.0.6"></script>

<link rel="stylesheet" href="/fancybox/source/helpers/jquery.fancybox-thumbs.css?v=1.0.7" type="text/css" media="screen" />
<script type="text/javascript" src="/fancybox/source/helpers/jquery.fancybox-thumbs.js?v=1.0.7"></script>
```
```html
<a class="fancybox" rel="group" href="big_image_1.jpg"><img src="small_image_1.jpg" alt="" /></a>
<a class="fancybox" rel="group" href="big_image_2.jpg"><img src="small_image_2.jpg" alt="" /></a>

```
```
<script type="text/javascript">
	$(document).ready(function() {
		$(".fancybox").fancybox();
	});
</script>
```



* ** [demo](http://www.jq22.com/yanshi28)**
* ** [github地址](https://github.com/fancyapps/fancyBox)**



个人试验,适配移动端

---

**[10.jPlayer-基于HTML5/Flash的音频、视频播放器-适配移动端](http://www.jplayer.cn/)**

* **github star:3500+**
* **github fork:1100+**


**jPlayer是一个JavaScript写的完全免费和开源 (MIT) 的jQuery多媒体库插件 (现在也是一个Zepto插件) jPlayer可以让你迅速编写一个跨平台的支持音频和视频播放的网页. jPlayer的丰富API可以让你创建一个个性化多媒体应用，因此也获得越来越多的社区成员的支持和鼓励。**

* **简单:**几分钟就可以上手编码、部署
* **可定制:**可以方便地用HTML和CSS换肤
* **轻量:**压缩的mini版只有12K
* **免费开源:**没有任何许可限制
* **社区支持:**不断增长的活跃社区
* **插件丰富:**主流平台上越来越多的免费插件
* **跨平台:**跨平台跨浏览器多解码器支持
* **文档全面:**完善的文档和入门指南
* **接口统一:**提供兼容浏览器、HTML5和Flash的统一接口
* **扩展性:**拥有高扩展性的架构体系

```js
<script type="text/javascript">
 $(document).ready(function(){
  $("#jquery_jplayer_1").jPlayer({
   ready: function () {
    $(this).jPlayer("setMedia", {
     m4a: "/media/mysound.mp4",
     oga: "/media/mysound.ogg"
    });
   },
   swfPath: "/js",
   supplied: "m4a, oga"
  });
 });
</script>
<div id="jquery_jplayer_1"></div>
<div id="jp_container_1">
 <a href="#" class="jp-play">Play</a>
 <a href="#" class="jp-pause">Pause</a>
</div>
```

* **[demo](http://www.jplayer.cn/demos.html)**
* **[github](https://github.com/happyworm/jPlayer)**

---
 

**[11.Rome-可定制的JS期与时间选择器-PC端](http://bevacqua.github.io/rome/)**

* **github star:2300+**
* **github fork:170+**

**Rome是一个可定制的JS日期与时间选择器。不依赖于第三方库**

```html
<input id='input' class='input' value='2014-12-15 21:00' />
<input id='inputTwo' class='input' />
```
```js
rome(input);
rome(inputTwo, { initialValue: '2014-12-08 08:36' });
```

* **[demo](http://bevacqua.github.io/rome/)**
* **[github](https://github.com/bevacqua/rome)**

---


**[12.Mobiscroll-移动端日期时间滑动、滚动插件-可以各种自定义](http://demo.mobiscroll.com/)**

* **github star:880+**
* **github fork:360+**

### 强烈推荐

**移动端自适应日期时间插件,可以各种自定义,ui 666,不过官网貌似要花钱,不过大天朝,你懂的.**


1.引jquery.js,jquerymobile.js 等等必须的文件


2.

```html
<div data-role="fieldcontain">
      <label for="txtBirthday">出生日期：</label>
      <input type="text" data-role="datebox"   id="txtBirthday" name="birthday" />
</div>
```

3.初始化日期控件

```js
$('input:jqmData(role="datebox")').mobiscroll().date();
```
```js
var opt = {
        preset: 'date', //日期
        theme: 'jqm', //皮肤样式
        display: 'modal', //显示方式 
        mode: 'clickpick', //日期选择模式
        dateFormat: 'yy-mm-dd', // 日期格式
        setText: '确定', //确认按钮名称
        cancelText: '取消',//取消按钮名籍我
        dateOrder: 'yymmdd', //面板中日期排列格式
        dayText: '日', monthText: '月', yearText: '年', //面板中年月日文字
        endYear:2020 //结束年份
    };
    
    $('input:jqmData(role="datebox")').mobiscroll(opt);
```
* **  [demo](demo.mobiscroll.com)**
* ** [github](https://github.com/acidb/mobiscroll)**


---


**[13.kindeditor-一款可定制性极高的富文本编辑器](https://kindeditor.codeplex.com/)**

* **github star:680+**
* **github fork:290+**

**KindEditor是一套开源的HTML可视化编辑器，主要用于让用户在网站上获得所见即所得编辑效果，兼容IE、Firefox、Chrome、Safari、Opera等主流浏览器。
**

1.在需要显示编辑器的位置添加textarea输入框。
```html
<textarea id="editor_id" name="content" style="width:700px;height:300px;">
&lt;strong&gt;HTML内容&lt;/strong&gt;
</textarea>
```
2.在该HTML页面添加以下脚本
```js
<script charset="utf-8" src="/editor/kindeditor.js"></script>
<script charset="utf-8" src="/editor/lang/zh-CN.js"></script>
<script>
        KindEditor.ready(function(K) {
                window.editor = K.create('#editor_id');
        });
</script>
```
3.获取HTML数据
```js
/*取得HTML内容*/
html = editor.html();

/* 同步数据后可以直接取得textarea的value*/
editor.sync();
html = document.getElementById('editor_id').value; /*原生API*/
html = K('#editor_id').val(); /* KindEditor Node API*/
html = $('#editor_id').val(); /*jQuery*/

/*设置HTML内容*/
editor.html('HTML内容');
```


* **[demo](http://kindeditor.net/demo.php)**
* **[github](https://github.com/kindsoft/kindeditor)**

---

**[14.jPages-强大的客户端分页插件](http://www.jq22.com/yanshi283)**
* **github star:590+**
* **github fork:280+**

**jPages是一个客户端分页插件，它比其他大多数插件多了很多功能，比如自动翻页，滚动浏览，显示延迟，完全可定制的导航面板也集成项目与Animate.css和延迟加载。**

1.下面的代码添加到您的网页的<head>部分：

```html
<link rel="stylesheet" href="css/jPages.css">
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script>
<script src="js/jPages.js"></script>
```

2.如果你想使用Animate.css动画你还需要添加的文件：

```html
<link rel="stylesheet" href="css/animate.css">
```

3.示例源代码：

```html
<!-- Future navigation panel -->
<div class="holder"></div>
<!-- Item container (doesn't need to be an UL) -->
<ul id="itemContainer">
<!-- Items -->
    <li>...</li>
    <li>...</li>
    <li>...</li>
    <li>...</li>
    <li>...</li>
    ...
</ul>
```

4.启动插件：

```js
$(function(){
  $("div.holder").jPages({
    containerID : "itemContainer"
  });
});
```

* **[demo](http://www.jq22.com/yanshi283)**
* **[github](https://github.com/luis-almeida/jPages)**
---

**[15.projekktor-UI漂亮的一款HTML5播放器](http://www.projekktor.com/)**
* **github star:160+**
* **github fork:60+**

* **[demo](http://www.projekktor.com/)**
* **[github](https://github.com/frankyghost/projekktor)**

---


**[16.touchSlide-滑动特效插件](http://www.superslide2.com/)(mobile)**

* **github star:100+**
* **github fork:70+**

**TouchSlide 是纯javascript打造的触屏滑动特效插件，面向手机、平板电脑等移动终端，
能实现触屏焦点图、触屏Tab切换、触屏多图切换等常用效果。
插件开源、体积小、简单实用、功能强大，是你架构移动终端网站的重要选择！**

1、引用TouchSlide.js
```js
<script type="text/javascript" src="../TouchSlide.1.0.js"></script>
```
2、编写HTML
```html
<div id="leftTabBox" class="tabBox">
    <div class="hd">
        <ul>
            <li>国内</li>
            <li>国际</li>
            <li>时事</li>
        </ul>
    </div>
    <div class="bd">
            <ul>
                <li><a href="#">官方明确感染H7N9高危人群</a></li>
                ...
            </ul>
            <ul>
                <li><a href="#">日:沈阳军区部队开赴中朝边境</a></li>
                ...
            </ul>
            <ul>
                <li><a href="#">农业占GDP低政府支持力度大</a></li>
                ...
            </ul>
    </div>
</div>
```
3、编写CSS，为HTML赋予样色

```css
.tabBox .hd{ height:40px; line-height:40px; padding:0 10px; font-size:20px; background:#f4f4f4; border-bottom:1px solid #F5AB38; position:relative;  }
.tabBox .hd ul{ position:absolute; height:41px; top:0; overflow:hidden;  }
.tabBox .hd ul li{ float:left; padding:0 10px; color:#666;  }
.tabBox .hd ul .on{ border:2px solid #F5AB38; border-bottom-color:#fff; background:#fff; color:#CF7F21;   }
.tabBox .bd ul{ padding:10px 0 10px 10px;  }
.tabBox .bd li{ height:33px; line-height:33px;   }
.tabBox .bd li a{ color:#666;  }
```
4、调用TouchSlide

```js
<script type="text/javascript">TouchSlide({ slideCell:"#leftTabBox" });</script>
```

* ** [demo](http://www.superslide2.com/TouchSlide/demo.html)**



个人亲测,移动端可高度自适应


---


**[17.移动端事件模拟封装库](https://github.com/chenmnkken/monoevent)**

* **github star:37+**
* **github fork:23+**

* **[demo](http://stylechen.com/touch.html)**
* **[github](https://github.com/chenmnkken/monoevent)**

---

**[18.elegant_font-炫的飞起的字体图标库](http://www.elegantthemes.com/blog/resources/elegant-icon-font/)**

**虽然很炫酷,但我还是没用过,用过的还是上面font-awesome一种**

* **github star:13+**
* **github fork:8+**

* **[demo](http://www.elegantthemes.com/)**
* **[github](https://github.com/pprince/etlinefont-bower)**


---

##以上排序根据github star数据降序排列
---

#以上总结不是特别精准,请以各自官网为准,后续遇到比较实用的插件也会继续更新,各位大神有什么好的推荐也可以私信我,共勉!


---
![](mydddd.png)










