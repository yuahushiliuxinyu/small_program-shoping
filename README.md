
# small_program-shoping商城微信小程序        
:blush

## 一：参考地址
1.接口来源：https://www.showdoc.com.cn/128719739414963  
2.微信工作平台：https://mp.weixin.qq.com/  
3.微信官方文档：https://developers.weixin.qq.com/doc/  
4.图标获取：https://www.iconfont.cn/  
5.图床：https://imgurl.org/  

## 二：其他  
1.使用了的插件：JSON-handle_0.6.1、Generate CSS tree  
2.关于商家的AppID获取实现支付功能：【关注微信小程序商家助、申请店铺、点击我的、点击店铺信息、、点击基础信息】这里就会出现商家AppID  
3.token错误获取不到值等问题可以参考我的方法  
4.不能授权等问题可以点击授权之后退出去再试  

## 三：优势  
小程序框架的目标是通过尽可能简单、高效的方式让开发者 可以在微信中开发具有原生APP体验的服务  
1.微信有海量用户，而且粘性很高，在微信里开发产品更容易触达用户  
2.推广app或公众号的成本太高  
3.开发适配成本低  
4.容易小规模试错，然后快速迭代  
5.跨平台  
6.微信明活已经达到10.82亿。中55岁以上的用户也达到6300万  
7.信息传达数达到450亿，较去年增长1 8%;视频通话4.1亿次增长100%  
8.小程序覆盖超过200+行业，交易额增长超过6倍，服务1000亿+人次创造出了5000亿+的商业价值  


## 四：技术工具  
1.系统：windows10  
2.框架：原生框架MINA   
3.技术：HTML5+CSS3+JavaScript+es6  
4.工具：微信开发者工具、Visual StudioCode  
5.其他了解：.json 后缀的 JSON 配置文件，页面配置  
	.wxml 后缀的 WXML 模板文件，页面结构  
	.wxss 后缀的 WXSS 样式文件，页面样式  
	.js 后缀的 JS 脚本逻辑文件，页面逻辑  
	.less后缀的LESS样式文件  

## 五：基本项目目录  
vscode 第三方软件配置文件  
Components 组件  
	SearchInput 搜索框组件  
	Tabs 导航栏组件  
	UpImg 自定义图片图片  
icons 保存图片  
Pages 页面文件夹  
	auth 支付授权  
	cart 购物车  
	category 商品分类  
	collect 收藏  
	feedback 意见反馈  
	goods_detail 商品详情  
	goods_list 商品列表  
	index 销售首页  
	login 登录  
	order 订单查询  
	pay 商品支付  
	search 搜索中心  
	user 个人中心  
	logs 日志  
request 异步请求  
styles 外部标签图片  
Utils 第三方工具  
app.js 项目的全局入口文件  
app.json 全局配置文件  
app.wxss 全局样式文件  
project.config 项目的配置文件  
sitemap.json 微信索引配置文件	  
 
## 六：主要页面  
主要页面：  
	销售首页、商品分类、购物车、个人中心、  
	商品列表、商品详细、商品支付、授权页面、  
	订单页面、商品收藏、搜索中心、意见反馈     

---
页面介绍：  
	1.销售首页  
		搜索框：点击进入搜索中心  
		滚动图、分类、超市购、母婴品：点击进入商品分类  
		时尚女装、户外运动、箱包配饰：点击进入商品列表  
	2.商品分类  
		搜索框：点击进入搜索中心  
		一级分类：点击出现对应一级分类  
		二级分类：点击出现三级分类  
		三级分类：点击进入商品列表  
	3.商品列表  
		搜索框：点击进入收索中心  
		综合、销量、价格：点击进入商品详细  
		下拉：下拉会进行刷新，到底会提示  
	4.搜索中心	 
		输入框：输入完进行检索，出现取消按钮，出现检索信息  
		检索信息：点击进入商品详细  
	5.商品详细  
		收藏：可以进行收藏和取消收藏进个人中心  
		客户：模拟进入客服会话  
		分享：分享给虚拟好友  
		加入购物车：点击进入购物车页面  
		立即购买：购买之前需要加入购物车  
	6.购物车  
		收货地址：没有就获取收索地址  
		购买的宝贝：可以进行勾选和取消，可以对购买物品数量进行加减和删除  
		结算按钮：显示购买的数量、显示购买的价钱，选择框可以对全部物品进行勾选  
			如果地址和物品之一没有没法进行购买，点击进入商品支付  
	7.商品支付  
		显示收获地址  
		购买物品的数量和价钱  
		点击支付：进入授权页面，再次点击弹出二维码，会对支付成功失败进行提示  
	8.授权页面  
		分为两个；支付授权，登录授权  
		授权按钮：点击进行授权  
	9.个人中心  
		登录按钮：没有进行登录授权  
		全部订单、收藏商品、关注商品、我的足迹：显示数量  
		我的订单：全部订单、待付款、待收货、退款退货  
		收货地址管理  
		联系客服、意见反馈、关于我们、推荐小程序  
	10.商品收藏  
		商品收藏、品牌收藏、店铺收藏、浏览足迹、全部收藏、正在热卖、即将上线  
		点击收藏商品：进入对应的商品详细  
	11.订单查询  
		全部订单、待付款、待发货、退款退货：显示订单编号、订单价格、订单日期  
	12.意见反馈  
		体验问题、商品商家投诉  
		问题总类：功能建议、购买遇到的困难、性能问题、其他  
		描述问题框：可以输入反馈的商品问题，可以对物品照片进行添加取消  
		提交按钮：点击把反馈的信息和照片上传到后台  
[回到顶部](#readme)  
