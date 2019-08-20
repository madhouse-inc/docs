请在每一个需要分析的页面复制下列代码
```
<body>
<!-- 您的网页代码  -->
</body>
//复制下列代码到您的网页文件
<script type="text/javascript" >
    (function (document,url, jssrc, dom) {
      jssrc = document.createElement('script'),
      dom = document.getElementsByTagName('script')[0];
      jssrc.async = 1;
      jssrc.src = url;
      dom.parentNode.insertBefore(jssrc, dom)
    })(document,'http://www.madhouse.com/madAnalytics.js');
</script>
```
在您的需要添加分析的页面逻辑中，调用madAnalytics方法，参数为您需要分析的事件信息。
```
<body>
<!-- ...  -->
<button onclick="clickAd()">play</button>
</body>
//...
<script type="text/javascript" >
  function clickAd(){
  //..
    madAnalytics('yourAnalyticsEvent');
  }
</script>
```
这样就能在您的页面中使用受众行为轨迹了。
