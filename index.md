## 欢迎来到DJ的博客

<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>钟表</title>
        <script type="text/javascript">
            function getDou(number) {
                if(number < 10) {
                    return '0' + number;
                } else {
                    return number;
                }
            }

            function getWeek(week) {
                var sWeek = null;
                switch(week) {
                    case 0:
                        sWeek = '星期日'
                        break;
                    case 1:
                        sWeek = '星期一'
                        break;
                    case 2:
                        sWeek = '星期二'
                        break;
                    case 3:
                        sWeek = '星期三'
                        break;
                    case 4:
                        sWeek = '星期四'
                        break;
                    case 5:
                        sWeek = '星期五'
                        break;
                    case 6:
                        sWeek = '星期六'
                        break;
                    default:
                        break;
                }
                return ' ' + sWeek;
            }
            window.onload = function() {
                var oDate = document.getElementsByTagName("p")[0];
                var oTime = document.getElementsByTagName("p")[1];

                function tick() {
                    var date = new Date();
                    var sDate = null;
                    var sTime = null;
                    var hours = date.getHours();
                    if(hours > 12) {
                        hours %= 12;
                        sTime = '下午 ';
                    } else {
                        sTime = '上午 ';
                    }
                    sTime += getDou(hours) + ':' + getDou(date.getMinutes()) + ':' + getDou(date.getSeconds());
                    sTime += getWeek(date.getUTCDay());
                    oTime.innerHTML = sTime;

                    sDate = date.getUTCFullYear() + "年";
                    if(date.getUTCMonth() < 9) {
                        sDate += '0' + (date.getUTCMonth() + 1) + "月";
                    } else {
                        sDate += (date.getUTCMonth() + 1) + "月";
                    }
                    sDate += date.getUTCDate() + "日";
                    oDate.innerHTML = sDate;
                }

                setInterval(tick, 1000);
                tick();
            }
        </script>
        <style type="text/css">
            body {
                width: 200px;
                height: 200px;
                background: #323332;
                vertical-align: middle;
                display: table-cell;
            }

            .date {
                text-align: center;
                color: yellow;
                font-size: 30px;
            }

            .time {
                text-align: center;
                color: yellow;
                font-size: 30px;
            }
        </style>
    </head>
    <body>
        <div>
            <p class="date">
                日期
            </p>
            <p class="time">
              
            </p>
        </div>
   




<audio autoplay="autoplay" height="100" width="100">
  <source src="小果 - 蒲公英的梦想.mp3" type="audio/mp3" />
  <source src="小果 - 蒲公英的梦想.ogg" type="audio/ogg" />
  <embed height="100" width="100" src="小果 - 蒲公英的梦想.mp3" />
</audio>
     </body>
</html>

<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <link rel="canonical" href="https://blog.csdn.net/dongjian2"/>
    <meta http-equiv="content-type" content="text/html; charset=utf-8">
    <meta name="renderer" content="webkit"/>
    <meta name="force-rendering" content="webkit"/>
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"/>
    <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <meta name="apple-mobile-web-app-status-bar-style" content="black">
    <meta name="referrer" content="always">
    <meta http-equiv="Cache-Control" content="no-siteapp" /><link rel="alternate" media="handheld" href="#" />
    <meta name="shenma-site-verification" content="5a59773ab8077d4a62bf469ab966a63b_1497598848">
        <meta name="csdn-baidu-search"  content='{"autorun":true,"install":true,"keyword":"【爱敲代码的小赤佬】2019放下包袱，开始崭新的代码之旅。"}'>
    
    <link href="https://csdnimg.cn/public/favicon.ico" rel="SHORTCUT ICON">
    <title>【爱敲代码的小赤佬】2019放下包袱，开始崭新的代码之旅。 - CSDN博客</title>

        
                    <link rel="stylesheet" href="https://csdnimg.cn/release/phoenix/template/css/list-50947b4ae9.min.css">
            
        
          <link rel="stylesheet" href="https://csdnimg.cn/release/phoenix/themes/skin-blue/skin-blue-b7967eb1c8.min.css">
        <script type="text/javascript">
        var username = "dongjian2";
        var blog_address = "https://blog.csdn.net/dongjian2";
        var static_host = "https://csdnimg.cn/release/phoenix/";
        var currentUserName = "dongjian2";
        var isShowAds = true;
        var isOwner = true;
        var loginUrl = "http://passport.csdn.net/account/login?from=https://blog.csdn.net/dongjian2"
        var blogUrl = "https://blog.csdn.net/";
        //页面皮肤样式
        var curSkin = "skin-blue";
        // 第四范式所需数据
        var articleTitles = "【爱敲代码的小赤佬】2019放下包袱，开始崭新的代码之旅。";
        var articleID = "";
        
        var nickName = "董建的博客";
        var isCorporate = false;
        var subDomainBlogUrl = "https://blog.csdn.net/"
    </script>
    <script type="text/javascript">
        // Traffic Stats of the entire Web site By baidu
        var _hmt = _hmt || [];
        (function() {
            var hm = document.createElement("script");
            hm.src = "https://hm.baidu.com/hm.js?6bcd52f51e9b3dce32bec4a3997715ac";
            var s = document.getElementsByTagName("script")[0];
            s.parentNode.insertBefore(hm, s);
        })();
        // Traffic Stats of the entire Web site By baidu end
    </script>
    <script src="https://csdnimg.cn/public/common/libs/jquery/jquery-1.9.1.min.js" type="text/javascript"></script>
    <script src="https://csdnimg.cn/rabbit/exposure-click/main-1.0.6.js"></script>
    <script src="//g.csdnimg.cn/fixed-sidebar/1.1.3/fixed-sidebar.js" type="text/javascript"></script>
    <!-- 新版上报 -->
    <script src="//g.csdnimg.cn/track/1.2.4/track.js" type="text/javascript"></script>
    <!-- 新版上报end -->
        <link rel="stylesheet" href="https://csdnimg.cn/public/sandalstrap/1.4/css/sandalstrap.min.css">
    <style>
        .MathJax, .MathJax_Message, .MathJax_Preview{
            display: none
        }
    </style>
</head>
<!-- nodata 第三栏接口无数据时样式不变 -->
<body class="nodata " > 
    <link rel="stylesheet" href="https://csdnimg.cn/public/common/toolbar/content_toolbar_css/content_toolbar.css">
    <script id="toolbar-tpl-scriptId" src="https://csdnimg.cn/public/common/toolbar/js/content_toolbar.js" type="text/javascript" domain="https://blog.csdn.net/"></script>
<link rel="stylesheet" href="https://csdnimg.cn/release/phoenix/vendor/pagination/paging.css">
<header>
	<div class="container d-flex clearfix" style="background-image: ">
		<div class="title-box">
			<h1 class="title-blog">
				<a href="https://blog.csdn.net/dongjian2">爱敲代码的小赤佬</a>
			</h1>
			<p class="description ">2019放下包袱，开始崭新的代码之旅。</p>
		</div>
		<div class="opt-box d-flex justify-content-end">
						<a class="btn btn-sm" href="https://mp.csdn.net/postlist">
				<svg class="icon" aria-hidden="true">
					<use xlink:href="#csdnc-cog"></use>
				</svg>管理博客</a>
					</div>
	</div>
	</header>
<script src="https://dup.baidustatic.com/js/ds.js"></script>
<div class="container clearfix pt0" id="mainBox">
    <main>
      <div class="filter-box d-flex align-items-center">
      <form action="" id=seeOriginal>
    <label class="chk-box" for="chkOriginal">
      <input onchange="this.checked ? document.getElementById('seeOriginal').submit() : location.href = 'https://blog.csdn.net/dongjian2'" type="checkbox" name="t" value="1"  id="chkOriginal">只看原创</label></form>
    <dl class="filter-sort-box d-flex align-items-center">
    <dt>排序：</dt>
    <dd><a href="javascript:void(0);" class="btn-filter-sort active" target="_self">默认</a></dd>
    <dd><a href="https://blog.csdn.net/dongjian2?orderby=UpdateTime" class="btn-filter-sort " target="_self">按更新时间</a></dd>
    <dd><a href="https://blog.csdn.net/dongjian2?orderby=ViewCount" class="btn-filter-sort " target="_self">按访问量</a></dd>
    <dd><a class="btn btn-sm rss" href="https://blog.csdn.net/dongjian2/rss/list">
		<svg class="icon" aria-hidden="true">
			<use xlink:href="#csdnc-rss"></use>
		</svg>RSS订阅</a>
    </dd>
  </dl>
</div>



<div class="article-list">
    
    <div class="article-item-box csdn-tracking-statistics" style="display: none;" data-articleid="82762601">
        <h4 class="">
            <a href="https://blog.csdn.net/yoyo_liyy/article/details/82762601" target="_blank">
            <span class="article-type type-1">原</span>帝都的凛冬</a>
        </h4>
        <p class="content">
            <a href="https://blog.csdn.net/yoyo_liyy/article/details/82762601" target="_blank">
                各种AI、人工智能、大数据如秋日凉爽的风，杳然erzhi；区块链的风头得到短暂的下降。

                此次山竹台风造成了多少伤亡和破坏？人民的生命和财产遭受重大损失
            </a>
        </p>
        <div class="info-box d-flex align-content-center">
            <p>
                <span class="date">2019-02-20 14:21:47</span>
            </p>
            <p>
                <span class="read-num">阅读数：13</span>
            </p>
            <p>
                <span class="read-num">评论数：2</span>
            </p>
        </div>
    </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87647721">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87647721" target="_blank">
        <span class="article-type type-1">
            原        </span>
        进制转换      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87647721" target="_blank">
        数据结构实验之栈与队列一：进制转换
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
输入一个十进制非负整数，将其转换成对应的 R (2 &amp;amp;lt;= R ...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-18 21:30:39</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">4</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87647721">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87452216">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87452216" target="_blank">
        <span class="article-type type-1">
            原        </span>
        多项式求和      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87452216" target="_blank">
        多项式求和
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
多项式描述如下：
1 - 1/2 + 1/3 - 1/4 + 1/5 - 1/6 ……
先请你求出多项式前n...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-16 15:26:10</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">7</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87452216">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87448236">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87448236" target="_blank">
        <span class="article-type type-1">
            原        </span>
        不敢死队问题      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87448236" target="_blank">
        不敢死队问题
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
说到“敢死队”，大家不要以为我来介绍电影了，因为数据结构里真有这么道程序设计题目，原题如下：
有M个敢死队...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-16 14:26:28</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">8</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87448236">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87437016">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87437016" target="_blank">
        <span class="article-type type-1">
            原        </span>
        约瑟夫问题      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87437016" target="_blank">
        约瑟夫问题
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
n个人想玩残酷的死亡游戏，游戏规则如下：
n个人进行编号，分别从1到n，排成一个圈，顺时针从1开始数到m，数...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-16 11:27:02</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">11</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87437016">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87429774">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87429774" target="_blank">
        <span class="article-type type-1">
            原        </span>
        双向链表      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87429774" target="_blank">
        数据结构实验之链表九：双向链表
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
学会了单向链表，我们又多了一种解决问题的能力，单链表利用一个指针就能在内存中找到下一个位...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-16 09:34:00</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">18</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87429774">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87366569">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87366569" target="_blank">
        <span class="article-type type-1">
            原        </span>
        有序链表的建立      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87366569" target="_blank">
        输入：5
2 3 4 1 5
输出：1 2 3 4 5
#include &amp;amp;lt;iostream&amp;amp;gt;
#include &amp;amp;lt;bits/stdc++.h&amp;amp;gt;
using namespace std;
typedef str...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-15 15:53:16</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">9</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87366569">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87289911">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87289911" target="_blank">
        <span class="article-type type-1">
            原        </span>
        单链表的拆分      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87289911" target="_blank">
        数据结构实验之链表五：单链表的拆分
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
输入N个整数顺序建立一个单链表，将该单链表拆分成两个子链表，第一个子链表存放了所有的...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-14 18:40:17</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">14</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87289911">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87289834">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87289834" target="_blank">
        <span class="article-type type-1">
            原        </span>
        有序链表的归并      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87289834" target="_blank">
        数据结构实验之链表四：有序链表的归并
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
分别输入两个有序的整数序列（分别包含M和N个数据），建立两个有序的单链表，将这两个...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-14 18:39:01</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">27</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87289834">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87289744">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87289744" target="_blank">
        <span class="article-type type-1">
            原        </span>
        链表的逆置      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87289744" target="_blank">
        数据结构实验之链表三：链表的逆置
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
输入多个整数，以-1作为结束标志，顺序建立一个带头结点的单链表，之后对该单链表的数据进...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-14 18:37:31</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">9</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87289744">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87289665">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87289665" target="_blank">
        <span class="article-type type-1">
            原        </span>
        逆序建立链表      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87289665" target="_blank">
        数据结构实验之链表二：逆序建立链表
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
输入整数个数N，再输入N个整数，按照这些整数输入的相反顺序建立单链表，并依次遍历输出...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-14 18:36:06</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">13</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87289665">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87289453">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87289453" target="_blank">
        <span class="article-type type-1">
            原        </span>
        数据结构实验之链表一：顺序建立链表      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87289453" target="_blank">
        数据结构实验之链表一：顺序建立链表
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
输入N个整数，按照输入的顺序建立单链表存储，并遍历所建立的单链表，输出这些数...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-14 18:32:42</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">18</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87289453">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87289107">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87289107" target="_blank">
        <span class="article-type type-1">
            原        </span>
        数据结构上机测试2-2:单链表操作B      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87289107" target="_blank">
        数据结构上机测试2-2:单链表操作B
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
按照数据输入的相反顺序（逆位序）建立一个单链表，并将单链表中重复的元素删除（值相同...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-14 18:26:49</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">14</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87289107">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="87288917">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/87288917" target="_blank">
        <span class="article-type type-1">
            原        </span>
        数据结构上机测试2-1:单链表操作A      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/87288917" target="_blank">
        数据结构上机测试2-1:单链表操作A
Time Limit: 1000 ms Memory Limit: 4096 KiB
Submit Statistic Discuss
Problem Description
输入n个整数，先按照数据输入的顺序建立一个带头结点的单链表，再输入一个数据m,将单链...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-14 18:24:02</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">12</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/87288917">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="86746264">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/86746264" target="_blank">
        <span class="article-type type-1">
            原        </span>
        顺序表应用6：有序顺序表查询      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/86746264" target="_blank">
        顺序表应用6：有序顺序表查询
Time Limit: 1000 ms Memory Limit: 4096 KiB
Submit Statistic Discuss
Problem Description
顺序表内按照由小到大的次序存放着n个互不相同的整数，任意输入一个整数，判断该整数在顺序表中是...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-01 23:05:48</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">13</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/86746264">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="86745763">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/86745763" target="_blank">
        <span class="article-type type-1">
            原        </span>
        顺序表应用5：有序顺序表归并      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/86745763" target="_blank">
        顺序表应用5：有序顺序表归并
Time Limit: 100 ms Memory Limit: 880 KiB
Submit Statistic Discuss
Problem Description
已知顺序表A与B是两个有序的顺序表，其中存放的数据元素皆为普通整型，将A与B表归并为C表，要求C...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-01 22:23:48</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">12</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/86745763">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="86744912">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/86744912" target="_blank">
        <span class="article-type type-1">
            原        </span>
        顺序表应用3：元素位置互换之移位算法      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/86744912" target="_blank">
        顺序表应用3：元素位置互换之移位算法
Time Limit: 1000 ms Memory Limit: 570 KiB
Submit Statistic Discuss
Problem Description
一个长度为len(1&amp;amp;lt;=len&amp;amp;lt;=1000...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-01 21:19:11</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">36</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/86744912">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="86743902">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/86743902" target="_blank">
        <span class="article-type type-1">
            原        </span>
        顺序表应用4：元素位置互换之逆置算法      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/86743902" target="_blank">
        顺序表应用4：元素位置互换之逆置算法
Time Limit: 10 ms Memory Limit: 570 KiB
Submit Statistic Discuss
Problem Description
一个长度为len(1&amp;amp;lt;=len&amp;amp;lt;=100000...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-01 18:56:41</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">40</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/86743902">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="86742959">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/86742959" target="_blank">
        <span class="article-type type-1">
            原        </span>
        顺序表应用2：多余元素删除之建表算法      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/86742959" target="_blank">
        顺序表应用2：多余元素删除之建表算法
Time Limit: 3 ms Memory Limit: 600 KiB
Submit Statistic Discuss
Problem Description
一个长度不超过10000数据的顺序表，可能存在着一些值相同的“多余”数据元素（类型为整型），...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-02-01 17:06:30</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">20</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/86742959">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="86698948">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/86698948" target="_blank">
        <span class="article-type type-1">
            原        </span>
        顺序表应用1：多余元素删除之移位算法      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/86698948" target="_blank">
        顺序表应用1：多余元素删除之移位算法
Time Limit: 1000 ms Memory Limit: 650 KiB
Submit Statistic Discuss
Problem Description
一个长度不超过10000数据的顺序表，可能存在着一些值相同的“多余”数据元素（...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-01-30 09:29:21</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">18</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">3</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/86698948">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="article-item-box csdn-tracking-statistics" data-articleid="86669628">
        <h4 class="">
        <a href="https://blog.csdn.net/dongjian2/article/details/86669628" target="_blank">
        <span class="article-type type-1">
            原        </span>
        顺序表的应用      </a>
    </h4>
    <p class="content">
      <a href="https://blog.csdn.net/dongjian2/article/details/86669628" target="_blank">
        顺序表的应用
Time Limit: 1000 ms Memory Limit: 65536 KiB
Submit Statistic Discuss
Problem Description
在长度为n（n&amp;amp;amp;amp;lt;1000)的顺序表中可能存在着一些值相同的“...      </a>
    </p>
    <div class="info-box d-flex align-content-center">
      <p>
        <span class="date">2019-01-27 21:03:32</span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">阅读数 <span class="num">60</span> </span>
      </p>
      <p class="point"></p>
      <p>
        <span class="read-num">评论数 <span class="num">0</span> </span>
      </p>
    </div>
          <div class="opt-box">
  		<button class="btn-opt" data-type="top">置顶</button>
  		<a class="btn-opt" data-type="edit" href="https://mp.csdn.net/postedit/86669628">编辑</a>
  		<button class="btn-opt" data-type="delete">删除</button>
      </div>
      </div>
  <div class="pagination-box" id="pageBox"></div>
</div>
    </main>
    <aside>
		    <div id="asideProfile" class="aside-box">
    <!-- <h3 class="aside-title">个人资料</h3> -->
    <div class="profile-intro d-flex">
        <div class="avatar-box d-flex justify-content-center flex-column">
            <a href="https://me.csdn.net/dongjian2">
                <img src="https://avatar.csdn.net/B/2/A/3_dongjian2.jpg" class="avatar_pic">
            </a>
            
        </div>
        <div class="user-info d-flex justify-content-center flex-column">
            <p class="name csdn-tracking-statistics tracking-click" data-mod="popu_379">
                <a href="https://me.csdn.net/dongjian2" target="_blank" class="" id="uid">董建的博客</a>
            </p>
                    </div>
            </div>
    <div class="data-info d-flex item-tiling">
                <dl class="text-center" title="66">
                        <dt><a href="https://blog.csdn.net/dongjian2?t=1">原创</a></dt>
            <dd><a href="https://blog.csdn.net/dongjian2?t=1"><span class="count">66</span></a></dd>
                    </dl>
        <dl class="text-center" id="fanBox" title="3">
            <dt>粉丝</dt>
            <dd><span class="count" id="fan">3</span></dd>
        </dl>
        <dl class="text-center" title="8">
            <dt>喜欢</dt>
            <dd><span class="count">8</span></dd>
        </dl>
        <dl class="text-center" title="8">
            <dt>评论</dt>
            <dd><span class="count">8</span></dd>
        </dl>
    </div>
    <div class="grade-box clearfix">
        <dl>
            <dt>等级：</dt>
            <dd>
                <a href="https://blog.csdn.net/home/help.html#level" title="3级,点击查看等级说明" target="_blank">
                    <svg class="icon icon-level" aria-hidden="true">
                        <use xlink:href="#csdnc-bloglevel-3"></use>
                    </svg>
                </a>
            </dd>
        </dl>
        <dl>
            <dt>访问：</dt>
            <dd title="3303">
                3303            </dd>
        </dl>
        <dl>
            <dt>积分：</dt>
            <dd title="683">
                683            </dd>
        </dl>
        <dl title="94369">
            <dt>排名：</dt>
            <dd>9万+</dd>
        </dl>
    </div>
        <div class="badge-box d-flex">
        <span>勋章：</span>
                        <div class="icon-badge" title="持之以恒">
            <div class="mouse-box">
                <svg class="icon" aria-hidden="true">
                    <use xlink:href="#csdnc-m-lasting"></use>
                </svg>
                <div class="icon-arrow"></div>
            </div>
            <div class="grade-detail-box">
                <div class="pos-box">
                    <div class="left-box d-flex justify-content-center align-items-center flex-column">
                        <svg class="icon" aria-hidden="true">
                            <use xlink:href="#csdnc-m-lasting"></use>
                        </svg>
                        <p>持之以恒</p>
                    </div>
                    <div class="right-box d-flex justify-content-center align-items-center">
                        授予每个自然月内发布4篇或4篇以上原创或翻译IT博文的用户。不积跬步无以至千里，不积小流无以成江海，程序人生的精彩需要坚持不懈地积累！
                    </div>
                </div>
            </div>
        </div>
                                                <script>
            (function ($) {
                setTimeout(function(){
                    $('div.icon-badge.show-moment').removeClass('show-moment');
                }, 5000);
            })(window.jQuery)
        </script>
    </div>
    </div>
		    <div class="csdn-tracking-statistics mb8 box-shadow" data-pid="blog" data-mod="popu_4" style="height:250px;">
    <div class="aside-content text-center" id="cpro_u2734133">
      <script type="text/javascript" src="//rabc1.iteye.com/production/openjs/d9o6b.js?bwo=coltly"></script>    </div>
</div>
		    		    		    <div id="asideCategory" class="aside-box flexible-box">
    <h3 class="aside-title">个人分类</h3>
    <div class="aside-content">
        <ul>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/7933088">
                    <span class="title oneline">二叉树</span>
                    <span class="count float-right">1篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/7938276">
                    <span class="title oneline">二维数组与指针</span>
                    <span class="count float-right">1篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/7945036">
                    <span class="title oneline">字符应用</span>
                    <span class="count float-right">2篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/7957870">
                    <span class="title oneline">暑假集训</span>
                    <span class="count float-right">1篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/7961359">
                    <span class="title oneline">链表</span>
                    <span class="count float-right">5篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/7964294">
                    <span class="title oneline">我的体会总结</span>
                    <span class="count float-right">3篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8071303">
                    <span class="title oneline">数据结构之顺序表</span>
                    <span class="count float-right">8篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8104927">
                    <span class="title oneline">数据结构之链表</span>
                    <span class="count float-right">8篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8225068">
                    <span class="title oneline">数据结构之串数组</span>
                    <span class="count float-right">4篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8273205">
                    <span class="title oneline">数据结构之树与二叉树</span>
                    <span class="count float-right">8篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8339902">
                    <span class="title oneline">程序设计基础</span>
                    <span class="count float-right">3篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8501187">
                    <span class="title oneline">称设----函数</span>
                    <span class="count float-right">1篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8546248">
                    <span class="title oneline">数据结构之排序</span>
                    <span class="count float-right">1篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8645403">
                    <span class="title oneline">寒假训练计划day1</span>
                    <span class="count float-right">1篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8650377">
                    <span class="title oneline">day2</span>
                    <span class="count float-right">1篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8655306">
                    <span class="title oneline">day3</span>
                    <span class="count float-right">5篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8670081">
                    <span class="title oneline">day4</span>
                    <span class="count float-right">7篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8672083">
                    <span class="title oneline">day5</span>
                    <span class="count float-right">2篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8673591">
                    <span class="title oneline">day6</span>
                    <span class="count float-right">3篇</span>
                </a>
            </li>
                        <li>
                <a class="clearfix" href="https://blog.csdn.net/dongjian2/article/category/8679520">
                    <span class="title oneline">day7</span>
                    <span class="count float-right">1篇</span>
                </a>
            </li>
                    </ul>
    </div>
        <p class="text-center">
        <a class="btn btn-link-blue flexible-btn" data-fbox="aside-archive">展开</a>
    </p>
    </div>
		    <div id="asideArchive" class="aside-box flexible-box">
    <h3 class="aside-title">归档</h3>
    <div class="aside-content">
        <ul class="archive-list">
                        <!--归档统计-->
            <li>
                <a href="https://blog.csdn.net/dongjian2/article/month/2019/02">
                    2019年2月                    <span class="count float-right">18篇</span>
                </a>
            </li>
                        <!--归档统计-->
            <li>
                <a href="https://blog.csdn.net/dongjian2/article/month/2019/01">
                    2019年1月                    <span class="count float-right">2篇</span>
                </a>
            </li>
                        <!--归档统计-->
            <li>
                <a href="https://blog.csdn.net/dongjian2/article/month/2018/12">
                    2018年12月                    <span class="count float-right">4篇</span>
                </a>
            </li>
                        <!--归档统计-->
            <li>
                <a href="https://blog.csdn.net/dongjian2/article/month/2018/11">
                    2018年11月                    <span class="count float-right">9篇</span>
                </a>
            </li>
                        <!--归档统计-->
            <li>
                <a href="https://blog.csdn.net/dongjian2/article/month/2018/10">
                    2018年10月                    <span class="count float-right">17篇</span>
                </a>
            </li>
                        <!--归档统计-->
            <li>
                <a href="https://blog.csdn.net/dongjian2/article/month/2018/09">
                    2018年9月                    <span class="count float-right">4篇</span>
                </a>
            </li>
                        <!--归档统计-->
            <li>
                <a href="https://blog.csdn.net/dongjian2/article/month/2018/08">
                    2018年8月                    <span class="count float-right">14篇</span>
                </a>
            </li>
                    </ul>
    </div>
        <p class="text-center">
        <a class="btn btn-link-blue flexible-btn" data-fbox="aside-archive">展开</a>
    </p>
    </div>
		    <div id="asideHotArticle" class="aside-box">
	<h3 class="aside-title">热门文章</h3>
	<div class="aside-content">
		<ul class="hotArticle-list csdn-tracking-statistics tracking-click" data-mod="popu_521">
							<li>
					<a href="https://blog.csdn.net/dongjian2/article/details/83960469">数据结构实验之二叉树一：树的同构</a>
					<p class="read">阅读数 <span>386</span></p>
				</li>
							<li>
					<a href="https://blog.csdn.net/dongjian2/article/details/83097870">数据结构实验之数组一：矩阵转置</a>
					<p class="read">阅读数 <span>156</span></p>
				</li>
							<li>
					<a href="https://blog.csdn.net/dongjian2/article/details/81983014">链表知识体会总结（仅供参考）</a>
					<p class="read">阅读数 <span>111</span></p>
				</li>
							<li>
					<a href="https://blog.csdn.net/dongjian2/article/details/83929222">数据结构实验之二叉树六：哈夫曼编码</a>
					<p class="read">阅读数 <span>110</span></p>
				</li>
							<li>
					<a href="https://blog.csdn.net/dongjian2/article/details/81975240">链表删除</a>
					<p class="read">阅读数 <span>109</span></p>
				</li>
					</ul>
	</div>
</div>
		    <div id="asideNewComments" class="aside-box">
    <h3 class="aside-title">最新评论</h3>
    <div class="aside-content">
        <ul class="newcomment-list">
                        <li>
                <a class="title text-truncate" target="_blank" href="https://blog.csdn.net/dongjian2/article/details/85458379#comments">矩阵的舞蹈</a>
                <p class="comment">
                    <a href="https://my.csdn.net/liuzhixiong_521" class="user-name" target="_blank">liuzhixiong_521</a>：[reply]dongjian2[/reply]
不好意思，打扰一下。
博客之星: 请投 003 ...                </p>
            </li>
                        <li>
                <a class="title text-truncate" target="_blank" href="https://blog.csdn.net/dongjian2/article/details/86698948#comments">顺序表应用1：多余元素删除之移位算法</a>
                <p class="comment">
                    <a href="https://my.csdn.net/chen_zan_yu_" class="user-name" target="_blank">chen_zan_yu_</a>：[reply]dongjian2[/reply]
加油咯，希望开学看到帅帅的你！                </p>
            </li>
                        <li>
                <a class="title text-truncate" target="_blank" href="https://blog.csdn.net/dongjian2/article/details/85458379#comments">矩阵的舞蹈</a>
                <p class="comment">
                    <a href="https://my.csdn.net/dongjian2" class="user-name" target="_blank">dongjian2</a>：[reply]liuzhixiong_521[/reply]
哈哈                </p>
            </li>
                        <li>
                <a class="title text-truncate" target="_blank" href="https://blog.csdn.net/dongjian2/article/details/86698948#comments">顺序表应用1：多余元素删除之移位算法</a>
                <p class="comment">
                    <a href="https://my.csdn.net/dongjian2" class="user-name" target="_blank">dongjian2</a>：小伙子学c++呢                </p>
            </li>
                        <li>
                <a class="title text-truncate" target="_blank" href="https://blog.csdn.net/dongjian2/article/details/86698948#comments">顺序表应用1：多余元素删除之移位算法</a>
                <p class="comment">
                    <a href="https://my.csdn.net/chen_zan_yu_" class="user-name" target="_blank">chen_zan_yu_</a>：小伙纸                </p>
            </li>
                    </ul>
    </div>
</div>
		<div id="asideFooter">
			
		<div class="aside-box">
			<script type="text/javascript" src="//rabc1.iteye.com/source/h751.js?avneunkw=b"></script>		</div>
				<div class="aside-box">
			<div class="persion_article">
			</div>
		</div>
	</div>
</aside>
<script src="https://csdnimg.cn/pubfooter/js/publib_footer-1.0.3.js" data-isfootertrack="false" type="text/javascript"></script>
<script>
	$("a.flexible-btn").click(function(){
		$(this).parents('div.aside-box').removeClass('flexible-box');
		$(this).remove();
	})
</script>
</div>
<div class="mask"></div>
<div class="promptBox clearfix">
    <div class="title clearfix bottom-dis-16">
        <span class="float-left">提示</span>
        <a class="float-right Boxclose">
            <svg class="icon" aria-hidden="true">
                <use xlink:href="#csdnc-times"></use>
            </svg>
        </a>
    </div>
    <div class="text">确定要删除当前文章？</div>
    <div class="pro-btn float-right">
        <a class="clickNo">取消</a>
        <a class="clickYes">删除</a>
    </div>
</div>
<script>
    var currentPage = 1;
    var baseUrl = 'https://blog.csdn.net/dongjian2/article/list' ;
    var pageSize = 20 ;
    var listTotal = 68 ;
    var pageQueryStr = '?';
    function getAllUrl(page) {
        return baseUrl + "/" + page + pageQueryStr;
    }
</script>
<script src="https://g.csdnimg.cn/login-box/1.0.4/??login-box.js,login-auto.js?t=20190103145208"></script>
<script src="https://csdnimg.cn/release/phoenix/vendor/pagination/paging.js"></script>
<script src='https://csdnimg.cn/public/common/gotop/js/goTop-v1.0.min.js?v201811201455'></script>
<script src="https://csdnimg.cn/release/phoenix/template/js/common-2dfea49d18.min.js"></script>
<script src="https://csdnimg.cn/release/phoenix/template/js/list-5988ce7495.min.js"></script>


<script>
    GoTop({
        right: 8
    })
</script>
<div class="box-box-default">
    <a class="btn-remove">
        关闭
    </a>
    <script type="text/javascript" src="//cee1.iteye.com/mhzzjepzz.js"></script>
</div>
<div class="box-box-large">
    <a class="btn-remove">
        关闭
    </a>
    <script type="text/javascript" src="//cee1.iteye.com/idvveasfs.js"></script>
</div>
</body>
</html>


