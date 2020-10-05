博客：https://www.7i24.xyz/
https://7i24.xyz/post/2020/24.xhtml

# 说在前面
VeCore验证码一小部分来自网络，如有侵权请评论联系。


# 使用
Demo:[https://cdn.7i24.xyz/vecore/][1]

## 引用
### 1.本地文件
你可以下载https://cdn.7i24.xyz/vecore/vecore.js 来在本地引用
或者下载本仓库vecore.js

### 2.CDN
您可直接使用本站的香港线路CDN 来使用VeCore
```URL
https://cdn.7i24.xyz/vecore/vecore.js
```

## 基础使用
在需要显示验证码框的地方，添加
```HTML
<div id="yz">
<noscript>
<p>请启用JavaScript来验证你是否是人类</p>
</noscript>
<script>
startver();
</script>
</div>
```

## 判断是否验证成功
VeCore使用了一个变量：`yfvenum`
如果`yfvenum`的数值为`0`，则表示还未验证或失败
如果`yfvenum`的数值为`1`，则表示已经验证成功
JS代码大致可以写成这样
```JavaScript
if(yfvenum=="1"){
alert('验证成功')
}else{
alert('验证失败')
}
}
```

## 输出成功或失败的数值
你可以给需要输出数值的地方给一个id：num
比如：
```HTML
<span id="num"><noscript>请启用js</noscript></span>
```
这样，js会在这个位置输出yfvenum的数值


  [1]: https://cdn.7i24.xyz/vecore/
