# WxRead-WebAutoReader

使用**微读自动阅读器**，帮助你解放生产力 *（双手）* ，该干啥干啥去，书币照样拿！

## 做这个的原因

闲的蛋疼！

当然不是！

实际上是因为在微信读书周阅读排行榜里看到了一个132小时的bug一般的存在，然后向网络求证了一下，发现知乎下有个人问了这个问题，求证之后顺手答了，大家可以在这里看我的回答：[微信读书时长究竟如何计算?](https://www.zhihu.com/question/349487832/answer/1020412380)。

主要还是现行的**挂机方法**太次，所以动手写了这个程序。

其实，我还连夜写了个Chrome扩展，本来想发布的，但是Chome发布要$，而我实在懒(非)得(常)折(的)腾(穷)，所以就没发了。如果您愿意拿一点小小的心意资助，请扫下方二维码，鄙人不胜感激。

## 微读自动阅读器实现原理

- 开启一个定时器，模拟页面滚动阅读
- 当滚动到底部后判定为章节已读完
- 章节完成后自动跳转到下个章节 *（查找下一章节点，模拟点击，就可以跳转了）*
- 当找不到下一章时判定为**本书已读完**，并发送通知给用户

## 使用说明

1. 打开浏览器 _（目前仅在Chrome下测试OK，其他浏览器还没来得及测试）_
2. 复制 [wx_auto_reader.min.js](./wx_auto_reader.min.js) 内容
3. 在浏览器新建一份书签，名称任意，如：`微信读书自动阅读器`，网址改为`javascript:步骤一的复制内容`
4. 打开微信读书网页版，打开任意一本书，点击书签栏 `微信读书自动阅读器`，启动阅读程序，挂机就完了

## 声明

本仓库仅提供代码，一切责任由使用者自行承担。


<p align="center">
	<img src="./WechatIMG10.jpeg" alt="Sample"  width="360" height="494">
	<p align="center">
		<em>微信收款码</em>
	</p>
</p>
