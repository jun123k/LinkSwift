<details>
<summary>【置顶】【Q&A】为啥本脚本不能破解百度网盘限速？其他脚本又能？</summary>
<p>你在本站内可能见过一些脚本，标着 “不限制下载” “不限速解析” “无视黑号” ，实则安装后又需要完成特定【任务】才给【加速下载链接】的脚本。<br/>它们是怎么做到的？为什么我这脚本却做不到？</p>
<p>主流网盘对非会员用户的限速是由客户端与服务端共同控制的。<br/>所以，即使有通过 CE 修改客户端速度的 “歪门邪道” 绕过客户端限速，那么也会被服务端检测到直接黑号。<br/>这样，我们就得出了【仅靠前端脚本无法绕过限速机制】这一结论。</p>
<p>那些脚本的工作原理大致如下：</p>
<ol>
<li>首先，脚本会先调用官方 API 接口，无感 “帮” 你生成文件的分享链接；</li>
<li>然后，脚本将生成的分享链接发到作者的服务器；</li>
<li>之后，服务器返回权限不足或者别的啥的提示，脚本显示公众号或小程序的二维码；</li>
<li>此时，脚本在完成任务前会不停向服务器确认任务是否完成；</li>
<li>扫码关注公众号或看广告后，服务器检测到完成了，然后会从作者购买的会员号 Cookie 池中选一个账号；（类似 ChatGPT 共享账号）</li>
<li>然后服务器调用官方 API 接口，用选出的账号转存你的文件，并调用官方 API 接口获取直链；</li>
<li>最后，把会员账号的不限速下载链接返回给脚本，脚本一般会将下载链接发送到指定的下载器中。（这样能够方便很多不会操作的用户）</li>
</ol>
<p>也就是说，这些工具其实是【借用的】别人的会员权限来实现不限速。</p>
<p>但使用这类服务时，你也可能面临以下风险：</p>
<ul>
<li>账号 - 由于依赖分享链接实现功能，如果你分享的文件曾被举报过，可能会导致对方账号和你的账号一同被封禁。</li>
<li>隐私 - 如果分享的是私密资源，第三方也有可能看到你的文件内容（懂的都懂，比如 “冠希哥” 事件）。</li>
<li>依赖 - 一旦这些工具背后的会员账号被平台批量封禁（业内俗称 “烧号”），而作者停止维护，工具就彻底失效。</li>
</ul>
<p>而这脚本，不会访问任何第三方服务器，<br/>只会通过调用网盘的官方接口来获取对应文件的下载直链，并且允许您选择您喜欢的下载器用于下载直链。</p>
<p>所以，您通过直链能获得的下载速度，完全取决于您自己账号的权限。<br/>如果你不是会员，下载依然会被限速。</p>
<p>如果你希望获得更快的下载速度，也可以尝试安装网盘官方客户端，把你的机子变成 PCDN，用上传换下载速度，为他们省点存储经费。</p>
</details>
<center>
	<p>“出淤泥而不染，濯清涟而不妖”</p>
	<hr>
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
		<a href="https://trendshift.io/repositories/13630" target="_blank"><img src="https://trendshift.io/api/badge/repositories/13630" alt="hmjz100%2FLinkSwift | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
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
