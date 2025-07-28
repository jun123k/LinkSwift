<details>
<summary>【置顶】【Q&A】为啥本脚本不能破解百度网盘限速？</summary>
<p>你可能见过一些需要完成特定 “任务” 才能 “加速下载” 或 “不限速解析” 的工具。<br/>它们是怎么做到的？为什么本脚本却做不到？</p>
<p>主流网盘对非会员用户的限速是由客户端与服务端共同控制的。<br/>即使你在浏览器中访问，也依然会受到服务端的限速策略影响。<br/>所以，仅靠前端脚本是无法绕过这一机制的。</p>
<p>那些所谓的 “不限速解析” 的工作原理如下：（流程已适当简化）</p>
<ol>
<li>工具 “帮” 你生成文件的分享链接；</li>
<li>工具将分享链接发到作者的私有服务器；</li>
<li>服务器返回公众号或小程序的二维码；</li>
<li>关注公众号或看广告后，服务器会从作者购买的会员号池中选一个账号；（类似 ChatGPT 共享账号）</li>
<li>用这个账号转存你的文件并获取直链；</li>
<li>最后把会员账号的不限速下载链接返回给你。</li>
</ol>
<p>也就是说，<strong>这些工具其实是 “借用” 别人的会员权限来实现不限速</strong>。</p>
<p>但使用这类服务时，你也可能面临以下风险：</p>
<ul>
<li><strong>账号安全</strong>：由于依赖分享链接实现功能，如果你分享的文件曾被举报，可能会导致对方账号和你的账号一同被封禁。</li>
<li><strong>隐私泄露</strong>：如果分享的是私密资源，第三方也有可能看到你的文件内容（懂的都懂，比如 “冠希哥” 事件）。</li>
<li><strong>依赖服务</strong>：一旦这些工具背后的会员账号被平台批量封禁（业内俗称 “烧号”），而作者停止维护，工具就彻底失效。</li>
</ul>
<p>而本脚本虽然运行在浏览器中，但不会访问任何第三方服务器。<br/>它通过调用网盘的官方接口来获取对应文件的下载直链。</p>
<p><strong>你通过直链能获得的下载速度，完全取决于你自己账号的权限</strong>。<br/>如果你不是会员，下载依然会被限速。</p>
<p>如果你希望获得更快的下载速度，也可以尝试安装网盘官方客户端，加入其 PCDN 分布式下载网络。<br/>但需要注意的是，这种方式可能导致你的家庭宽带流量异常，引发 ISP（网络服务商）的关注，甚至限制你的网络连接。</p>
</details>
<center>
	<p>
		搭配使用，效果更佳！👋扩展脚本
		<br/>
		<a href="https://scriptcat.org/script-show-page/2385" target="_blank">123 云盘会员青春版</a> | <a href="https://scriptcat.org/script-show-page/2236" target="_blank">百度网盘会员青春版</a> | <a href="https://scriptcat.org/script-show-page/2470" target="_blank">阿里云盘会员青春版</a>
		<br/>
		↓&nbsp;&nbsp;↓&nbsp;&nbsp;↓&nbsp;&nbsp;↓&nbsp;&nbsp;↓
	</p>
	<p>
		<img alt="Github Stargazers" src="https://img.shields.io/github/stars/hmjz100/LinkSwift?label=星标&logo=github&logoColor=white&labelColor=black&color=gold&style=for-the-badge&cacheSeconds=10">
		<img alt="Github Forks" src="https://img.shields.io/github/forks/hmjz100/LinkSwift?label=复刻&logo=github&logoColor=white&labelColor=black&color=grey&style=for-the-badge&cacheSeconds=10">
		<br/>
		<img alt="Github Licence" src="https://img.shields.io/github/license/hmjz100/LinkSwift?label=许可&logo=github&logoColor=white&labelColor=black&color=grey&style=for-the-badge&cacheSeconds=10">
		<br/>
		<img src="https://img.shields.io/chrome-web-store/v/gcalenpjmijncebpfijmoaglllgpjagf.svg?label=Tampermonkey%20BETA%20篡改猴测试版&logo=tampermonkey&logoColor=red&color=red&style=for-the-badge" alt="Tampermonkey BETA 篡改猴测试版">
		<img src="https://img.shields.io/chrome-web-store/v/dhdgffkkebhmkfjojejmpbldmpobfkfo.svg?label=Tampermonkey%20篡改猴&logo=tampermonkey&logoColor=white&color=brightgreen&style=for-the-badge" alt="TamperMonkey 篡改猴">
		<br>
		<img src="https://img.shields.io/badge/Google_Chrome-≥76.0-yellow.svg?style=for-the-badge" alt="Google Chrome-≥76.0">
		<img src="https://img.shields.io/badge/Microsoft_Edge-≥88.0-blue.svg?style=for-the-badge" alt="Microsoft Edge-≥88.0">
		<img src="https://img.shields.io/badge/支持平台-Windows_|_Mac_|_Linux_|_Android-blueviolet.svg?style=for-the-badge" alt="支持平台">
	</p>
</center>

## 说明

基于[【网盘直链下载助手】](https://www.baiduyun.wiki/install.html)修改

* 原作者：[油小猴](https://www.youxiaohu.com/)
* 原脚本 Github 仓库：[https://github.com/syhyz1990/baiduyun](https://github.com/syhyz1990/baiduyun)
* 本脚本开源至 Github：[https://github.com/hmjz100/LinkSwift](https://github.com/hmjz100/LinkSwift)
* 特别声明：已在遵守原脚本许可证的情况下对原脚本做出有意义的改进。

<center>
<img src="https://starchart.cc/hmjz100/LinkSwift.svg?variant=adaptive&amp;line=%23574ab8" alt="Starchart"><br/>Github 星标历史
</center>

#### 卑微的小标题

这个脚本只有一个人在修改\~如果喜欢的话还请留个 [好评](https://scriptcat.org/zh-CN/script-show-page/1604/comment) 和 [星标](https://github.com/hmjz100/LinkSwift) 哦\~或者随便给脚本评个分也行的(>\_<)，还可以来[看看我的其他脚本!](https://scriptcat.org/users/114812)

* 如有 bug 等问题请前往 Github 发 [issues 反馈](https://github.com/hmjz100/LinkSwift/issues)

***

<center><p>这是给认真阅读完README文件的人的赞美</p></center>
<center><p>个人博客: <a target="_blank" href="https://hmjz100blog.rf.gd">https://hmjz100blog.rf.gd</a></p></center>
