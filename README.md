为 sublime text 2&amp;3 准备的微信应用号/小程序 snippet,方便大家使用
-----
### 简介

刚接触微信小程序开发,尝试着使用了一下微信开发调试工具 v0.9版的代码编辑功能,感觉好鸡肋有木有!?于是果断回到 ST.但是,ST 不认微信"发明"出来的这个WXML,这个WXML 可以说是 html 和 xml 的变异结合体.

不过还好ST有自定义 snippet 的功能,于是我就动手把 WXML 里的组件和部分其他内容都整成了 snippet 分享出来方便大家使用,提升大家的开发效率.

废话不多说,开撸~

### 安装部署

将下载好的代码片段放入 Sublime text安装目录/Packages/User 目录中即可.

### snippet 列表

为了防止和其他 snippet 冲突,本 snippet 中的所有WXML 标签触发命令都以'w'开头,所有 API相关命令都以'api'开头.

#### WXML snippet

| 命令 | 对应组件或命令 |
| -----|----:|
| wapp | [注册小程序](https://mp.weixin.qq.com/debug/wxadoc/dev/framework/app-service/app.html) |
| wblockif | [block wx:if](https://mp.weixin.qq.com/debug/wxadoc/dev/framework/view/wxml/conditional.html)  |
| wbutton | [button](https://mp.weixin.qq.com/debug/wxadoc/dev/component/button.html) |
| wcheckbox | [checkbox][2] |
| wcheckboxgroup | [checkbox-group][2] |
| wactionsheet | [action-sheet](https://mp.weixin.qq.com/debug/wxadoc/dev/component/action-sheet.html) |
| wcanvas | [canvas](https://mp.weixin.qq.com/debug/wxadoc/dev/component/canvas.html#canvas) |
| wimage |[image](https://mp.weixin.qq.com/debug/wxadoc/dev/component/image.html)|
| wtext | [text](https://mp.weixin.qq.com/debug/wxadoc/dev/component/text.html) |
| wview | [view][4] |
| wviewbind | [view 事件](https://mp.weixin.qq.com/debug/wxadoc/dev/framework/view/wxml/event.html) |
| wmap | [map](https://mp.weixin.qq.com/debug/wxadoc/dev/component/map.html)|
| wmodal | [modal](https://mp.weixin.qq.com/debug/wxadoc/dev/component/modal.html)|
| wnavigator |[navigator](https://mp.weixin.qq.com/debug/wxadoc/dev/component/navigator.html)|
| wexport | [模块化](https://mp.weixin.qq.com/debug/wxadoc/dev/framework/app-service/module.html)|
| wfor | [for](https://mp.weixin.qq.com/debug/wxadoc/dev/view/wxml/data.html) |
| wform |[form](https://mp.weixin.qq.com/debug/wxadoc/dev/component/form.html)|
| wradio|[radio][5]|
| wradiogroup|[radio-group][5]|
| wslider|[slider](https://mp.weixin.qq.com/debug/wxadoc/dev/component/slider.html)|
| wicon|[icon](https://mp.weixin.qq.com/debug/wxadoc/dev/component/icon.html)|
| winput|[input][3]|
| winfutautofocus|[input][3]|
| wtoast|[toast](https://mp.weixin.qq.com/debug/wxadoc/dev/component/toast.html)|
| wvideo|[video](https://mp.weixin.qq.com/debug/wxadoc/dev/component/video.html)|
| winputfocus|[input][3]|
| wlabel|[label](https://mp.weixin.qq.com/debug/wxadoc/dev/component/label.html)|
| wloading|[loading](https://mp.weixin.qq.com/debug/wxadoc/dev/component/loading.html)|
| wpage|[Page()](https://mp.weixin.qq.com/debug/wxadoc/dev/framework/app-service/page.html)|
| wprogress|[progress](https://mp.weixin.qq.com/debug/wxadoc/dev/component/progress.html)|
| wscrollview|[scroll-view](https://mp.weixin.qq.com/debug/wxadoc/dev/component/scroll-view.html)|
| wswitch|[switch](https://mp.weixin.qq.com/debug/wxadoc/dev/component/switch.html)|
| wtemplate|[template](https://mp.weixin.qq.com/debug/wxadoc/dev/framework/view/wxml/template.html)|
| wswiper|[swiper](https://mp.weixin.qq.com/debug/wxadoc/dev/component/swiper.html)|
|wviewelif|[view][4]|
|wviewelse|[view][4]|
|wviewif|[view][4]|


#### 小程序API snippet

| 命令 | 对应组件或命令 |
| -----|----:|
| apirequest| [网络请求](https://mp.weixin.qq.com/debug/wxadoc/dev/api/network-request.html) | 
| apiuploadfile| [上传文件][15] | 
| apidownloadfile| [下载文件][15] | 
| apiconnskt| [创建 WebSocket 链接][14] | 
| apionsktopen| [监听WebSocket连接打开][14] | 
| apionskterr| [监听WebSocket错误][14] | 
| apisendsktmsg| [使用 WebSocket发送数据][14] | 
| apionsktmsg| [接受消息推送][14] | 
| apicloseskt| [关闭WebSocket连接][14] | 
| apionsktclose| [监听WebSocket关闭](14) | 
| apichooseimg| [选额图片](13) | 
| apipreviewimg| [预览图片][13] | 
| apistartrecord| [开始录音][12] | 
| apistoprecord| [结束录音][12] | 
| apiplayvoice| [播放语音][1] | 
| apipausevoice| [暂停播放语音][1] | 
| apistopvoice| [结束播放语音][1] | 
| apigetbgaudioplayerstate| [获取音乐播放状态][6] | 
| apiplaybgaudio| [播放音乐][6] | 
| apipausebgaudio| [播放暂停音乐][6] | 
| apiseekbgaudio| [控制音乐播放进度][6] | 
| apistopbgaudio| [停止播放音乐][6] | 
| apionbgaudioplay| [监听音乐播放][6] | 
| apionbgaudiopause| [监听音乐暂停][6] | 
| apionbgaudiostop| [监听音乐停止][6] | 
| apisavefile| [文件](https://mp.weixin.qq.com/debug/wxadoc/dev/api/file.html) | 
| apichoosevideo| [视频](https://mp.weixin.qq.com/debug/wxadoc/dev/api/media-video.html) | 
| apisetstorage| [覆盖本地内容][7] | 
| apisetstoragesync| [同步覆盖本地内容][7] | 
| apigetstorage| [获取指定 key 对应的内容][7] | 
| apigetstoragesync| [同步获取指定 key 对应的内容][7]  | 
| apiclearstorage| [清理本地数据][7] | 
| apiclearstoragesync| [同步清理本地数据][7]| 
| apigetlocation| [获取位置][8] | 
| apiopenlocation| [查看位置][8] | 
| apigetnetworktype| [网络状态][9] | 
| apigetsysinfo| [系统消息][9] | 
| apiaccelerometerchange| [重力感应][9] | 
| apicompasschange| [罗盘][9] | 
| apisetnavbartitle| [动态设置导航条文字]() | 
| apishownavbarloading| [显示导航条加载动画][10] | 
| apihidenavbarloading| [隐藏导航条加载动画][10] | 
| apihidekeyboard| [收起键盘](https://mp.weixin.qq.com/debug/wxadoc/dev/api/ui-other.html) | 
| apinavigateto| [保留当前页面并跳转][11] | 
| apiredirectto| [关闭当前页面并跳转][11] | 
| apinavigateback| [返回上一个页面][11] | 
| apilogin| [登录](https://mp.weixin.qq.com/debug/wxadoc/dev/api/api-login.html) | 
| apigetuserinfo| [用户信息](https://mp.weixin.qq.com/debug/wxadoc/dev/api/open.html) | 
| apipayment| [微信支付](https://mp.weixin.qq.com/debug/wxadoc/dev/api/api-pay.html) | 


[1]: https://mp.weixin.qq.com/debug/wxadoc/dev/api/media-voice.html "语音"
[2]: https://mp.weixin.qq.com/debug/wxadoc/dev/component/checkbox.html "多选"
[3]: https://mp.weixin.qq.com/debug/wxadoc/dev/component/input.html "文本框"
[4]: https://mp.weixin.qq.com/debug/wxadoc/dev/component/view.html "视图"
[5]: https://mp.weixin.qq.com/debug/wxadoc/dev/component/view.html "单选"
[6]: https://mp.weixin.qq.com/debug/wxadoc/dev/api/media-background-audio.html "音乐播放控制"
[7]: https://mp.weixin.qq.com/debug/wxadoc/dev/api/data.html "本地数据"
[8]: https://mp.weixin.qq.com/debug/wxadoc/dev/api/location.html  "地理位置"
[9]: https://mp.weixin.qq.com/debug/wxadoc/dev/api/device.html "设备信息"
[10]: https://mp.weixin.qq.com/debug/wxadoc/dev/api/ui.html "导航条动画"
[11]: https://mp.weixin.qq.com/debug/wxadoc/dev/api/ui-navigate.html "跳转"
[12]: https://mp.weixin.qq.com/debug/wxadoc/dev/api/media-record.html "录音"
[13]: https://mp.weixin.qq.com/debug/wxadoc/dev/api/media-picture.html "预览选择图片"
[14]: https://mp.weixin.qq.com/debug/wxadoc/dev/api/network-socket.html "socket"
[15]: https://mp.weixin.qq.com/debug/wxadoc/dev/api/network-file.html "上传下载文件"

### 未添加的 snippet 列表

由于下列标签或 api 参数过多,并且使用方法多种多样,所以暂未添加到仓库中,建议小伙伴们如有用到下列标签,还请查阅官方文档,以免被我坑了;-)

[动画](https://mp.weixin.qq.com/debug/wxadoc/dev/api/api-animation.html).
[绘图](https://mp.weixin.qq.com/debug/wxadoc/dev/api/api-canvas.html).
[模板消息](https://mp.weixin.qq.com/debug/wxadoc/dev/api/notice.html).

### enjoy && give me a star. ;-D
