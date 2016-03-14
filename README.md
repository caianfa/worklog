# Worklogs

# **2016**

### *Date: 3 - 14 (一)*

#### Plan:

- H5 红包区域投放功能接口调试

- 配合测试人员修复抽奖功能 `bug`

### *Date: 3 - 11 (五)*

#### Plan:

- H5 红包区域选择前端实现

  1. 已经实现区域选择和移除
  2. 移除后返回到可选区域原本的排序位置

#### Mark:

- [跨站攻击 - CRSF] [16-3-11-1]

  [16-3-11-1]: https://github.com/Monine/study/issues/5
  '跨站攻击 - CRSF'

### *Date: 3 - 10 (四)*

#### Plan:

- 抽奖功能缓存机制完善

  1. 加入缓存机制后，抽奖功能无法在后端抽奖结果数据返回之前执行预抽奖操作~
  2. 目前只是简单粗暴的使用 `alert` 提示用户已经抽过奖和没有抽奖机会了

- 开始 H5 红包功能区域投放前端实现

  1. 计划与红包广告功能区域投放使用相同实现机制

#### Mark:

- 加班 18:30 ~ 22:00 (3.5h)

- 把 `stady` 仓库 `Issues` 内的部分与工作相关的内容移动到这个仓库的 `Issues` 内

- > 红包广告功能在开发\测试环境切换的时候需要手动更改接口的域名值，需要一个实现自动修改可行方案~ (3 - 8)

  1. 今天想到一个方案就是在打开预览页面调用 `GetDomain` 接口时后端返回红包和抽奖功能在对应环境下的接口域名地址，目前 `GetDomain`           接口只返回了二维码相关的一些配置数据，所以可以充分利用~

### *Date: 3 - 9 (三)*

#### Plan:

- 抽奖功能 debug

  1. 奖品数量负值检测修改
  2. 加入缓存机制

- 电商平台页面框架搭建
  
  1. [网站项目目录结构规范] [16-3-9-1]

  [16-3-9-1]: https://github.com/appbone/mobile-spa-boilerplate/blob/master/directory.md
  '网站项目目录结构规范'

  2. 商品管理页面搭建完成

#### Mark:

- 晚上在 [慕课网] [16-3-9-2] 把 `Bootstrap` 教程复习了一遍

  [16-3-9-2]: http://www.imooc.com/
  '慕课网'

### *Date: 3 - 8 (二)*

#### Plan:

- 抽奖功能 `debug`

- H5 红包添加匿名抽奖功能

  1. 用户打开场景的时候弹出微信授权确认页面，获取用户的头像、昵称、性别、头像、地址、 `OpenID` 、 `UnionID` 等信息~

- 添加摇一摇抽奖功能

  1. 15 号 `v5.5.0` 版本发布之后再正式开始实现融入目前的大转盘和九宫格抽奖

#### Mark:

- 红包广告功能在开发\测试环境切换的时候需要手动更改接口的域名值，需要一个实现自动修改可行方案~

- 摇一摇抽奖功能并没有想到合适的方案

  下午工作状态非常差 #_#

- [2016十家公司前端面试小记] [16-3-8-1]

  [16-3-8-1]: http://www.cnblogs.com/xxcanghai/p/5205998.html
  '2016十家公司前端面试小记'

  1. 晚上看到的文章，感受就是面试题的内容都明白一二，但要我回答可能就表述不清，无法深入。一定找个时间把里面题目全部详细解答一遍！！！

### *Date: 3 - 7 (一)*

#### Plan:

- 抽奖功能 `debug`

#### Mark:

- update 环境红包广告曝光接口修改

- 抽奖功能领奖表单提交数据进行编码

  呃，这里我忘了 `jQuery` 的 `ajax` 方法会自动给参数进行编码，导致给后台传的参数实际进行了 2 次编码~

### *Date: 3 - 4 (五)*

#### Plan:

- 抽奖功能今天开始细节调优、 `debug`

#### Mark:

- > 编辑页面抽奖功能奖品设置的奖品名称字符长度限制需要一个可行方案 (3 - 1)

  1. 目前的解决方案是在当前奖品名称输入框失去焦点 `blur()` 的时候再去判断字符的长度，如果超出长度则触发错误处理机制~

- 好想吐槽咱后端目前的混乱状态，尼玛获取代码后编译各种报错~

  无法调取接口获得数据，尼玛只能各种造假数据来调试代码，盲写代码有木有！

- [UTF-8 编码标准下获取字符串中字符的字节长度] [16-3-4-1]

  [16-3-4-1]: https://github.com/Monine/Worklogs/issues/1
  'UTF-8 编码标准下获取字符串中字符的字节长度'

  晚上还特意看了一篇关于 [字符、字节和编码] [16-3-4-2] 的文章

  [16-3-4-2]: http://www.regexlab.com/zh/encoding.htm
  '字符、字节和编码'

- [常用的正则表达式] [16-3-4-3]

  [16-3-4-3]: https://github.com/Monine/study/issues/2
  '常用的正则表达式'

### *Date: 3 - 3 (四)*

#### Plan:

- 今天务必走完抽奖功能流程！

  1. 没做完就加班！ T-T

#### Mark:

- 抽奖功能流程终于走完了 T_T

- 晚上看了 `张鑫旭` 大神一篇关于 SVG 动画的文章 [超级强大的SVG SMIL animation动画详解] [16-3-3-1]

  [16-3-3-1]: http://www.zhangxinxu.com/wordpress/2014/08/so-powerful-svg-smil-animation
  '超级强大的SVG SMIL animation动画详解'

- 俺军哥写了一篇关于前端职业发展规划的文章 [前端工程师的职业发展规划] [16-3-3-2]

  [16-3-3-2]: https://github.com/f2e-journey/f2e-journey/blob/master/career-planning.md
  '前端工程师的职业发展规划'

### *Date: 3 - 2 (三)*

#### Plan:

- 调试预览页面抽奖功能接口

#### Mark:

- 早晨阅读时间读到 `AlloyTeam` 的一篇文章 [谈前端工程师的职业规划] [16-3-2-1]

  [16-3-2-1]: http://www.alloyteam.com/2015/04/talk-about-the-front-end-engineering-career-planning
  '谈前端工程师的职业规划'

  > “一专多长” 才是前端工程师的终极目标

  不仅是前端，大部分领域都应该是这样

  > “一专” 是指你不可替代 “多长” 表示你可以替代别人

  一专已是难得，多长更是宝贵！

- 上午开了一上午的需求评审会议，其他正常需求都 OK，然而我们准备启动的新项目 (商城) 最终讨论未果，还需细细琢磨~

- 下午用 `css` 实现圆形的时候遇到一个小难关 o_o

  1. 因为要做手机适配，在百分比值宽高不相等的容器内，如何实现一个相对父容器大小比例固定的圆形？

  2. 一个基础却又容易混淆的css知识点 [巧用margin/padding的百分比值实现高度自适应（多用于占位，避免闪烁）] [16-3-2-2]

  [16-3-2-2]: https://segmentfault.com/a/1190000004231995
  '巧用margin/padding的百分比值实现高度自适应'

### *Date: 3 - 1 (二)*

#### Plan:

- 继续完善抽奖功能

  1. 看后端今天能否解决报错问题进行调试

- 查看易企秀的长页面功能实现原理

  1. 呃~事实上是并没有腾出时间看
  2. 好吧~确实是我给忘了

#### Mark:

- 编辑页面抽奖功能奖品设置的奖品名称字符长度限制需要一个可行方案

  1. 目前是用 `AngularJS` 的 `$watch` 函数监听奖品列表输入变化，但是我们在使用输入法输入汉字的时候，`input` 标签内会先出现拼音，等确定选择哪个字或是词语之后按下空格或者对应的数字键，汉字才会出现在 `input` 标签内，可就在汉字准备出现在 `input` 标签内的时候，`AngularJS` 的机制就判定了监听变化，并且把拼音也算进这变化之中，这就使判定出错~
  
- 下午有重新整理编辑页面抽奖功能的代码，做了一系列优化与封装等，由草版变为正式版~

- 军哥中午跟我说咱 70c 的 H5 制作平台就交给我来负责了，然后有新人来也交给我带，嗯... OK，没问题~

### *Date: 2 - 29 (一)*

#### Plan:

- 完善大转盘编辑、预览页面

  1. 主要调试细节问题和与后端调试接口数据
  
#### Mark:

- 上午调试大转盘抽奖发现百分比控制的元素大小或距离会有小数上的偏差，类似于 `rem` 产生的 [小像素问题] [16-2-29-1]

  [16-2-29-1]: http://taobaofed.org/blog/2015/11/04/mobile-rem-problem
  'rem 产生的小数像素问题'

- 下午调试大转盘指针在指向抽奖结果那格区域的随机摆动角度，并没有与后端调试接口数据，后端还是一片混乱，各种报错，无法调试状态~

- [大转盘抽奖 Demo] [16-2-29-2]

  [16-2-29-2]: http://monine.github.io/study/public/lottery_dzp.html
  '大转盘抽奖 Demo'

### *Date: 2 - 26 (五)*

#### Plan:

- 预览页面大转盘抽奖功能

  1. 实现用户点击抽奖按钮之后调用接口，在接口获得抽奖结果数据之前大转盘保持转动，直到接口返回抽奖结果数据之后再停止转动，并且保证大转盘转动流畅自然~

#### Mark:

- 上午调休两个小时

### *Date: 2 - 25 (四)*

#### Plan:

- 抽奖功能完善 

  1. 根据后端接口数据调整 JS 代码
  
- 5.4.0 版本发布

#### Mark:

- 因为版本发布加班到凌晨 12 点

- 军哥介绍了一个替代 [f5] [16-2-25-1] 的前端开发工具  [Puer] [16-2-25-2]

  [16-2-25-1]: http://getf5.com
  'f5'

  [16-2-25-2]: http://leeluolee.github.io/2014/10/24/use-puer-helpus-developer-frontend
  'Puer'

  > Puer 是一个可以实时编辑刷新的前端服务器

- 阅读了一些关于 [js 内存泄漏] [16-2-25-3] 的相关知识

  [16-2-25-3]: http://www.ibm.com/developerworks/cn/web/wa-jsmemory
  'js 内存泄漏'
