/*Title: youkuPlayerDescription: youkuPlayer*/<ul id="tab" class="clearfix">	<li class="active"><a href="#method-content">Method</a></li>	<li><a href="#const-content">Constant</a></li></ul><div id="method-content"><div class="outline">[playVid](#playVid)[closePlayer](#closePlayer)</div># 概述youkuPlayer，通过调用此模块可以使用优酷的手机播放器播放优酷网的视频资源。#**playVid**<div id="playVid"></div>播放当前vid所指的视频。##paramsy:- 类型：数值- 默认值：0- 描述：此为android开发用户选项，播放器纵坐标（距页面顶端距离）。vid:- 类型：字符串- 默认值：XOTI4ODEwMTYw- 描述：视频的Video id为视频的唯一标识。

clientId：- 类型：字符串- 描述：优酷开放平台中所创建应用的APP ID


clientSecret：

- 类型：字符串- 描述：优酷开放平台中所创建应用的APP SECRET

isHD:

- 类型：数值
- 默认值：0
- 描述：此为android开发用户选项，只有0、1两个值。0为悬浮播放器窗口模式，1为弹出单独页面可支持高标清切换模式。

##示例代码```javascript// 使用者调用playVid方法传入视频的id，即可播放优酷网视频            var player = api.require('youkuPlayer');    var params = {		        clientId : "2231a6ec*******", //优酷开放平台中所创建应用的APP ID                clientSecret : "847005e8a1666ebfedf*******", //优酷开放平台中所创建应用的APP SECRET                vid : "XMTM0Mz*****", //视频id		};        player.playVid(params, function(ret, err){});```##可用性iOS系统，Android系统可提供的1.0.0及更高版本#**closePlayer**<div id="playVid"></div>关闭播放器。##示例代码```javascript// 使用者调用playVid方法传入视频的id，即可播放优酷网视频            var player = api.require(‘youkuPlayer’);        player.closePlayer();```##可用性Android系统