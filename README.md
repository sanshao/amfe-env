#lib.env

## 最新版本

**1.3.0**

## 安装依赖

运行 `npm install`，来安装所需的依赖模块。关于NPM的知识，请参见[nodejs](http://nodejs.org/);

## 用Grunt打包

运行 `grunt`，来对项目进行打包。关于Grunt的知识，请参见[gruntjs](http://gruntjs.com/);

## 如何使用

* lib.env.params - url中search参数的对象，例如有ttid参数可以通过lib.env.params['ttid']来获取
* lib.version(strVersion) - 返回一个版本号的对象
	* gt(strVersion) - 大于指定版本号
	* gte(strVersion) - 大于等于指定版本号
	* lt(strVersion) - 小于指定版本号
	* lte(strVersion) - 小于等于指定版本号
	* eq(strVersion) - 等于指定版本号
	* compare(strVersion) - 比较指定版本号，返回-1表示小于，返回0表示等于，返回1表示大于
* lib.env.os - 操作系统的对象
	* os.name - Android/iOS/Windows Phone/unknown
	* os.version - 相应的版本号(Version对象实例)
	* os.isWindowsPhone - 是否是Windows Phone
	* os.isIPhone - 是否是iPhone/iPod Touch
	* os.isIPad - 是否是iPad
	* os.isIOS - 是否是iOS
	* os.isAndroid - 是否是Android
* lib.env.browser - 浏览器的对象
	* browser.name - UC/QQ/Chrome/Android/Safari/iOS Webview/IE/unknown
	* browser.version - 相应的版本号(Version对象实例)
	* browser.isUC - 是否是UC浏览器
	* browser.isQQ - 是否是QQ浏览器
	* browser.isIE - 是否是IE浏览器
	* browser.isIEMobile - 是否是IE移动版浏览器
	* browser.isIELikeWebkit - 是否是IE兼容了Webkit特性的浏览器
	* browser.isChrome - 是否是Chrome浏览器
	* browser.isAndroid - 是否是Android的原生浏览器
	* browser.isSafari - 是否是Safari浏览器
	* browser.isWebview - 是否是iOS下的Webview
* lib.env.aliapp - 客户端的对象，如果没有，表示不在客户端里
	* aliapp.windvane - windvane的版本
	* aliapp.appname - App的名称，比如TB,TM等
	* aliapp.version - 客户端的版本
	* aliapp.platform - iPhone/iPad/Android
* lib.env.taobaoApp - 兼容老版本，等同于lib.env.aliapp

### aliapp.appname对应的值（供参考）

![appname](http://gtms01.alicdn.com/tps/i1/TB1FskDGXXXXXboXpXXVUdOQFXX-300-684.jpg)