##1.0.0##
###类库###
增加3D引擎【新】

增加时间轴动画支持【新】

增加对LayaPlayer，Flash版本的支持【新】

优化UI组件，减少对callter的调用次数

Sprite类增加hitTestPrior属性，用来优化鼠标事件点击效率

弹出对话框位置进行四舍五入，防止变虚

改进Log类，禁用鼠标点击，增加toggle方法方便控制

Event增加keyCode属性代码提示 【感谢：易先森】

优化加载队列，防止最后一个加载内容被引用

增加HttpRequest和Loader的扩展适应性【感谢：zhuliping】

增加webgl设备丢失事件及相关处理

更改Node的displayInStage属性为displayedInStage

修复2D粒子资源释放问题

修复List在没有滚动条时变化大小子对象不会跟着改变

修复双层cacheAs导致的异常

修复drawTexture设置矩阵后无效的bug

修复遮罩位置显示不及时的bug

###LayaAirIDE###
增加时间轴动画功能

增加App测试工具(beta)【新】

增加App打包工具(beta)【新】

增加App构建工具(beta)【新】

创建嵌套页面失败时显示一个失败图片

当box对象有pivotX pivotY时，转到父容器时不自动调整坐标

修复锁定tip不对的问题

修复输入名字验证没生效的问题

修复节点树面板无数据刷新时卡死的问题

修复窗口大小改变时的布局算法

修复点中增加修改pivot的点

修复有时选中对象不能拖动大小的问题

修复UIView在代码模式改变数据之后，source丢失的问题


##1.0.0 RC2##
###类库###
优化引擎，性能又得到10%的提升

改进帧率统计信息在手机上显示变清晰了

Text新增underline属性，用于显示文字下划线

Label增加对overflow的支持

加载器增加对jpeg后缀的识别

增加对console函数的支持

clearRes时，如果是Texture，会自动调用销毁

改进对话框发虚的现象

对话框弹出增加轴心点的影响

修复缓动结束结果值不对的bug 【感谢：男人不需大名鼎鼎づ 】

修复精灵被销毁后，异步加载图片可能会导致的报错

修复webgl文字内存泄漏bug

修复画圆设置边框为0时仍然显示边框的bug

修复设置Sprite的hitArea无效的bug 【感谢：中文IM】

修复Clip播放时，第一帧间隔过长的bug 【感谢：豆子狐狸】

###LayaAirIDE###
更改编辑器皮肤，更加统一美观了

改进颜色选择器，增加快速输入框，方便快速修改（知道颜色值的情况下）

解决Panel中的Tab用节点树选取编辑器卡死的问题

解决节点树过滤结果不对的问题

解决提示信息重叠的问题

##1.0.0 RC1##
###类库###
调整引擎API,使其更简单，统一，易懂（为了今后更好的体验，1.0会对api做最后调整，1.0正式版之后不再做调整）

调整API:

	调整movieClip动画相关API，增加label设置及事件触发
	
	调整时间轴动画API，增加label标签及label事件触发
	
	调整粒子相关API，使其更容易使用
	
	调整骨骼动画相关API，使其更容易使用，增加更多功能
	

UI库所有组件增加anchorX，anchorY属性，增加百分比的锚点设置

Animation新增addLabel，removeLabel方法，方便注册label到关键帧，并派发对应的label事件 

Animation的loadImages和loadAtlas新增cacheName属性，方便缓存动画模板，减少对象创建

UI组件增加gray属性，区分disabled属性

修复iphone下，设置全屏显示导致无法显示的问题

修复List拖动时，selecteIndex显示状态更新错误的bug 【感谢：小文】

修复在某些手机上drawText大小为负数时报错bug 【感谢：JAyDeN】

修复Tween的update函数最后一次没有正确执行的bug 【感谢：┐X  ⌒X】

修复WEBGL下HTML文本对不齐的问题

修复MovieClip在从Stage上移除时没有停止播放的问题

修复地图动画，帧间隔时间太长，引起的跳动问题

修复修改颜色只有最后一行生效的bug

###LayaAirIDE###

LayaAirIde实现自动IDE更新功能，无需再去网站重新下载

增加LayaAir类库管理，可以下载，更改使用的类库，简化类库更换操作

资源属性面板增加是否打包进图集选项

资源增加可视化九宫格的设置面板

编辑器增加位图字体的支持

调整属性间距，使属性显示更完整

增加删除资源时未选中资源时的提示

拖动图标时增加修改鼠标样式

模板UI截取过长的字符串

属性面板增加不打包图集的标识

增加旧MornUI项目的sizeGrid属性转换

修复HtmlText显示不了图片的问题

修复编辑器某些选择框没有更新的问题

修复替换功能失效的bug


##1.0.0 beta##
###类库###

调整引擎API,使其更简单，易懂（为了今后更好的体验，1.0会对api做最后调整，1.0正式版之后不再做调整）

调整API:
	更改Browser.ctx为Browser.context
	
	更改Rectangle的equal为equals
	
	更改URL类的getName为getFileName
	
	更改Dictionary的elements为values
	
	更改Sprite的optimizeFloat为optimizeScrollRect
	
	更改骨骼动画相关API
	
	其他API更改

增加45度交错地图及缩放功能

增加停止所有声音的接口

改进骨骼动画，增加换装及插槽支持

Stage增加fullscreenEnabled属性exitFullscreen方法和fullscreenchange事件，方便实现全屏游戏

Loader类增加parserMap资源解析函数对应表，用来扩展更多类型的资源加载解析

优化文字渲染

Loader增加part粒子后缀的自动识别 【感谢：现舞/ty】

改变算法，让ShowAll更清晰

MovieClip支持重复加载不同动画的模式

增加粒子参数，更新canvas粒子与3d粒子一致

改善图集加载进度信息，使其更平滑 【感谢：Rekc@h】

Animation的loadAtlas增加加载完成回调 

改善设置9宫格增加容错机制

优化粒子生存时间小于等于0的情况

改进移动端输入框显示方式

修复滤镜显示异常 【感谢：遥远的豆】

修复WebGL下文字偏移的bug 【感谢：谷主】

修复手机模式双击失效的bug

修复staticCache不对的问题

修复缓存时，父对象缩放导致缓存模糊

修复缩放图片后，会出现灰色阴影 【感谢：幻宇】

修复高清屏下滤镜不清晰的问题

修复html文本图片不显示的问题

修复Image多次设置皮肤后，剧中对齐不对的bug 【感谢：红尘轮回】

修复Stage的frameRate="mouse"模式不正确的bug

修复Loader加载类型JSOn为JSON

修复渲染区选取区域不准的问题

修复动画有alpha时，复用对象时没有重置alpha的问题

修复Tween回收对象池后，update没能及时清理的bug 【感谢：谷主】

修复Sprite的startDrag跟随鼠标有偏差

修复Byte写文件时一直在创建缓冲区的问题

修复list设置为cacheAs后，拖动停止后不能正常恢复

修复粒子混合模式BUG

###LayaAirIDE###

优化编辑器性能，性能提升一倍

增加TS，JS内置调试模式

增加AS3语法高亮

优化编辑器失去焦点时的cpu占用【感谢：JAyDeN】

增加var命名重复提示

去除编辑区在mouseOver时获取焦点的行为

当选中的对象有旋转时，选择框和对象一起旋转

属性面板鼠标提示增加属性字段显示

树右键时若鼠标下方无选中对象取消选中

增加自动适配UI大小功能，快捷键（Ctrl+L）

属性面板在设置相同类型的面板时不清理

改进ts导出代码的格式，引用的引擎类都使用全路径，去除简写引入

改进编辑面板拖动时鼠标图标

修复移动多级目录时卡死的问题 【感谢：陈健，hello word】

修复有些页面数据不对的时候导致死循环的问题

修复状态栏宽高数据有时显示不对的问题

修复ctrl+上下键移动节点层级不对的问题

修复输入框切换输入法时可能导致ctrl状态不对的问题

修复新建粒子文件时没有清空上一次名字的问题

修复父容器有缩放时放在子对象上的选中框不对的问题

修复节点树上拖动对象到子对象上时导致的异常

修复属性面板颜色选择器初始颜色不对的问题

修复拖拽时图标位置不正确的问题

修复选中宽高为0的对象时显示大框的问题

修复在带render的页面中新拖入的组件可能id不对的问题

修复颜色拾取器的赋值与面板上看到的值不一致的问题

修复资源面板有时图标不对的问题

修复资源树右键没有切换选择的问题