# 魔法变身

Magic Transformation.

这是一套放在本项目里的网页技能。用来新建、改版或重做一页：先定一种气质，再按段拼版式，最后只加少数表面和动作。也可以用来查页面为什么慢。

技能怎么执行，以 [SKILL.md](.cursor/skills/magic-transformation/SKILL.md) 为准。本文件只描述这套方案里有什么，方便人查阅。做页面时不要通读四份目录，只打开选中的条目。

## 四条轴

风格决定整页像什么，一页只留一个主风格。布局决定每一段怎么分栏，一页可以有多段，相邻段不重复。特效决定表面，最多 3 个，其中高成本最多 1 个。动画决定怎么动，最多 4 个。关掉脚本和动效之后，标题、说明和主按钮仍然在。

没有真实客户、员工、价格、日期、人数或合作标识时，不编造，也不留空位假装有。某一段需要配图而手里没有文件时，去网上找符合这一段题材的图，放进站点图库并署名。图放进固定比例的画框里裁切，焦点留住主体。背景再上网找纸纹、颗粒或表面素材，存进站点并署名，文字放在实色块或遮罩上。首页从上到下分层，第 1 层是导航，最后一层是页脚，整页不少于 9 层。规范里的句子不够时，按文档已经点名的题材上网补材料并写来源。写代码前先有一份设计稿：色值、最多两套字体、第一层怎么构图。左右对开要底边对齐，不留空底。每一页要有导航、一个标题、首屏主动作、分节、字号和间距阶梯、结尾和页脚。下拉、单选、多选和弹层不用系统默认样式，按当前风格自己写。

## 文件

| 文件 | 作用 |
|------|------|
| [SKILL.md](.cursor/skills/magic-transformation/SKILL.md) | 何时使用、先做什么、默认配方、随机算法、互斥、页面标准、设计完成度、首页篇幅、补材料、配图、背景、裁切、交稿前检查 |
| [references/styles.md](.cursor/skills/magic-transformation/references/styles.md) | 风格，80 条 |
| [references/layouts.md](.cursor/skills/magic-transformation/references/layouts.md) | 样式布局，84 条 |
| [references/effects.md](.cursor/skills/magic-transformation/references/effects.md) | 特效，49 条 |
| [references/motion.md](.cursor/skills/magic-transformation/references/motion.md) | 动画，59 条 |
| [references/implement.md](.cursor/skills/magic-transformation/references/implement.md) | 选定之后怎么接、怎么停、失败时回到哪一帧 |
| [references/templates.md](.cursor/skills/magic-transformation/references/templates.md) | 风格对照的网页模板，每条附有参考链接 |

每条目录都按同一顺序写：何时使用、怎么做、不要做什么、必须遵守的尺寸和缺内容时的做法。

## 怎么选

可以说具体 id，也可以把某一条轴或全部轴设为「随机」。随机按 `SKILL.md` 里的种子公式抽。主风格只要没被点名，就每次从全部风格里重抽，不用默认表里的风格，也不重复上一轮。布局、特效、动画没指定、也没说随机、也没有成文规范时，用 `SKILL.md` 里那张按用途准备的默认表。

选定之后先写出配方。没有页面清单时做完整的一页。已经有页面清单或规范时，先读规范。主风格每次随机抽一个没用过的，把要做的页一次做完。首页按「首页篇幅」做满不少于 9 层，句子不够就按规范里的题材上网补。之后可以说换风格，就重抽并把已做的页改成新风格。布局只负责这些块怎么分栏，不把目录里的示例题材贴到别的页上。导航、结尾动作和页脚都要在。

## 风格

| id | 名称 | 是什么 |
|----|------|--------|
| `style.editorial` | 编辑杂志 | 像一本可以翻的专题，而不是一张海报 |
| `style.swiss` | 瑞士网格 | 信息按格子对齐，靠留白和字号分层次 |
| `style.minimal` | 极简留白 | 把内容减到还能说明白为止 |
| `style.brutalist` | 粗野 | 结构外露，像没装修完的页面仍然能用 |
| `style.neo-brutal` | 新粗野 | 粗野的规矩版：粗边框、硬投影、色块，但网格是齐的 |
| `style.poster` | 海报 | 每一屏是一张海报 |
| `style.product` | 产品发布 | 把一个产品讲清楚：它是什么、看一眼、为什么现在用 |
| `style.cinematic` | 电影 | 像预告片的节奏，但网页仍然能读、能点 |
| `style.immersive` | 沉浸实验 | 页面本身是一件交互作品 |
| `style.luxury` | 奢侈时装 | 慢、稀、准 |
| `style.photo` | 影像册 | 照片是正文 |
| `style.archive` | 建筑档案 | 像档案柜：项目可检索、元数据清楚 |
| `style.commerce` | 电商橱窗 | 先帮人看清商品，再帮人买 |
| `style.nostalgia` | 复古数字 | 借用早期屏幕、印刷广告或低清晰度影像的味道，但文字和按钮按现在的可用性做 |
| `style.organic` | 有机流体 | 曲线、连续的形状和柔软的节奏 |
| `style.terminal` | 终端技术 | 像一台能读的机器界面 |
| `style.playful` | 玩具 | 鼓励拨弄，但每个拨弄都有反馈 |
| `style.longform` | 长文 | 阅读优先的文章或报告 |
| `style.index` | 目录索引 | 很多入口，平等陈列 |
| `style.hospitality` | 餐饮空间 | 把地点、时间和食物或房间讲具体 |
| `style.dashboard` | 说明板 | 把一组指标或步骤摊开给决策的人看 |
| `style.soft` | 柔软圆角 | 界面像摸得到的圆角物件，但结构仍然整齐 |
| `style.flat` | 扁平色块 | 靠纯色块和字号区分，不用阴影和材质 |
| `style.maximal` | 繁密 | 信息多、颜色多、层次多，但有一条主线能读完 |
| `style.memphis` | 孟菲斯 | 几何色块、短曲线和撞色，像一张平面海报铺到页面上 |
| `style.vapor` | 蒸汽波 | 晚霞色、窗格和早期数字界面的气氛 |
| `style.y2k` | 千禧 | 铬面、气泡和塑料高光，表达千禧年前后的乐观界面 |
| `style.cyber` | 赛博 | 暗底、少量霓虹和明确的信息层级 |
| `style.collage` | 拼贴 | 多张图和字条像贴在同一张板上 |
| `style.zine` | 小志 | 像一本自制小册子：便宜的印刷、直接的语气、不一致也被控制在一册之内 |
| `style.street` | 街头 | 大字、贴纸、高对比，像墙面和衣服上的图形 |
| `style.gallery` | 白盒子 | 像展厅：白、静、作品之间有距离 |
| `style.blueprint` | 蓝图 | 细线、标注和单色，像图纸 |
| `style.ink` | 水墨 | 留白像纸，墨色像笔触 |
| `style.riso` | 孔版 | 双色错位印刷的味道 |
| `style.comic` | 分格 | 用格子讲一件事 |
| `style.type` | 实验字体 | 字就是图像 |
| `style.event` | 活动页 | 把时间、地点和为什么来写清楚 |
| `style.course` | 课程 | 说明学什么、给谁、怎样上课 |
| `style.news` | 报头 | 很多条消息按时间和重要性排列 |
| `style.launch` | 预告 | 一件东西还没公开完全，页面负责收集兴趣或告知日期 |
| `style.lookbook` | 造型册 | 按造型或系列往下看，节奏慢，一件看完再下一件 |
| `style.agency` | 案例代理 | 用案例证明能做什么，而不是用形容词 |
| `style.saas` | 软件服务 | 把正在提供的软件讲清楚：解决什么、界面长什么样、怎么收费、怎么开始 |
| `style.local` | 上门服务 | 让人打得通、约得到、知道你在哪干活 |
| `style.clinic` | 诊疗 | 安静、好找、能预约 |
| `style.realty` | 房源 | 帮人看清单、筛条件、问一套具体的房 |
| `style.legal` | 执业咨询 | 说明你处理什么、费用怎么谈、怎样开始一次咨询 |
| `style.fitness` | 锻炼课表 | 让人看懂今天有什么课、多少钱、怎样开始 |
| `style.wedding` | 婚礼信息 | 把日期、地点、安排和是否出席说清 |
| `style.travel` | 行程 | 按天说明去哪、住哪、注意什么 |
| `style.consulting` | 顾问 | 卖的是判断和一次谈话，不是功能列表 |
| `style.resume` | 履历 | 一个人的工作记录 |
| `style.docs` | 文档 | 让人查到步骤并照着做 |
| `style.nonprofit` | 公益 | 说明在帮谁、钱或时间怎么用、人怎样参与 |
| `style.stay` | 住宿 | 帮人看清房间、日期相关的信息和怎样预订 |
| `style.music` | 曲目 | 先听到或看到作品，再给演出和购买 |
| `style.app` | 应用落地 | 说明这是什么应用、在什么设备上用、怎样安装 |
| `style.finance` | 财务说明 | 讲清你做什么、怎样收费、一次谈话如何开始 |
| `style.beauty` | 护理预约 | 把项目、时长、价格和预约说清楚 |
| `style.construction` | 工程 | 说明做什么工程、在哪些区域、怎样报价 |
| `style.personal` | 个人名片 | 一个名字下的整页：你是谁、做什么、怎样联系 |
| `style.blog` | 专栏 | 一篇篇可以订阅或回看的文章，首页是目录不是单篇 |
| `style.glass-dark` | 深色玻璃 | 深色底上只有少量半透明面板，字仍然是实的 |
| `style.bauhaus` | 包豪斯 | 圆、方、三角和原色承担结构，不是贴上去的装饰 |
| `style.deco` | 装饰几何 | 对称、阶梯线和细金属线 |
| `style.grunge` | 做旧 | 磨损、复印边和略微歪斜的标题 |
| `style.japandi` | 静木 | 暖纸色、浅木色和很少的物件 |
| `style.clay` | 软泥 | 控件和插图块像有厚度的软物件，放在平的桌面上 |
| `style.neumorphic` | 浮雕 | 同一底色上，用亮暗两层阴影做出凸起和按下 |
| `style.glass-light` | 浅色玻璃 | 浅底上一条或一块磨砂，字是深色实字 |
| `style.noir` | 暗调 | 近黑的底、暖白的字、一种琥珀或红只做一点 |
| `style.academic` | 书斋 | 章节号、边注和出处是版式的一部分 |
| `style.biophilic` | 草木 | 用真实的日光、植物或土壤的颜色组织页面 |
| `style.retro-70s` | 暖调七十 | 棕、橙、芥末和胖一点的字 |
| `style.pixel` | 像素 | 有限的几种颜色和整数倍的块 |
| `style.case` | 案例叙述 | 把一件已经做过的工作讲完：当时的情况、限制、做了什么、结果 |
| `style.podcast` | 节目 | 一档节目的首页或单集页，能看出节目名、这一集讲什么、以及能不能听 |
| `style.museum` | 展陈 | 一场展览的参观信息：展名、日期、地点、展厅顺序 |
| `style.directory` | 名录 | 许多同类条目，字段一致，可以筛选 |

## 样式布局

| id | 名称 | 是什么 |
|----|------|--------|
| `layout.single` | 单栏 | 整页一条栏，读起来像文档 |
| `layout.split` | 左右对开 | 屏幕分成两块，一块看，一块读 |
| `layout.feature-rows` | 图文交替行 | 每一节换一边放图，用来讲三到五个步骤或功能 |
| `layout.magazine` | 杂志多栏 | 一条宽栏配一条窄栏，窄栏放章节名、注释或小图 |
| `layout.sticky-side` | 粘性侧栏 | 一侧是目录或筛选，另一侧是长内容 |
| `layout.cards` | 等大卡片格 | 同样大小的格子重复出现，用来比较多件并列的东西 |
| `layout.bento` | 便当格 | 几块大小不同的矩形拼在同一组里，突出一块，其余作补充 |
| `layout.masonry` | 瀑布流 | 卡片高度随内容变化，上下错落 |
| `layout.mosaic` | 不规则马赛克 | 少数几张图拼成一张墙，有的大、有的小，用来做作品封面墙 |
| `layout.gallery` | 画廊墙 | 等宽的图按行排列，行高可以不同，但同一行内对齐 |
| `layout.full-bleed` | 满幅章节 | 某一节的图或色块贴到屏幕左右边缘，用来换气 |
| `layout.frame` | 留框 | 内容四周始终留着一圈边，像画被装在框里 |
| `layout.chapters` | 整屏章节 | 每一章大约一屏，滚完一章就是下一章 |
| `layout.center-stage` | 居中舞台 | 一个主体坐在视口正中，周围留白 |
| `layout.header-stack` | 标题叠图 | 标题压在主图上，图是第一屏的底 |
| `layout.overlap` | 重叠层 | 一组元素故意叠在一起，形成前后 |
| `layout.broken` | 破格 | 大多数元素在网格上，少数标题或图片故意出格 |
| `layout.diagonal` | 斜切分区 | 两个区域用一条斜线分开 |
| `layout.band` | 色带分区 | 用整宽的色带把页面分成几段 |
| `layout.timeline` | 时间线 | 沿着一条竖线排列事件 |
| `layout.steps` | 步骤条 | 把过程收成连续的几步，用来说明如何开始 |
| `layout.comparison` | 对比双栏 | 左右各一个方案，用来比较 |
| `layout.pricing` | 价格列 | 专门放真实价格的一排 |
| `layout.index-rows` | 索引行 | 每一条是一行，字段对齐，用来扫很多名称 |
| `layout.cover-index` | 封面加目录 | 第一屏是封面，接着是可以扫的目录 |
| `layout.pinned-media` | 媒体钉住 | 一边的图或产品停在屏幕里，另一边的文字往下走，文字走到头，图再一起离开 |
| `layout.carousel-row` | 横滑一排 | 一排卡片超出屏幕，可以横滑 |
| `layout.stack` | 层叠卡片区 | 几张卡片在同一节里叠成一摞，用来收纳步骤或引言 |
| `layout.tabs` | 标签面板 | 同一位置切换几组内容 |
| `layout.faq` | 问答折叠 | 一组问题，答案默认收起 |
| `layout.form-split` | 表单对开 | 一边解释为什么要填，一边是表单 |
| `layout.quote-break` | 引文打断 | 正文中间插入一条短引文，把长文切开 |
| `layout.stats-row` | 指标行 | 一排真实数字，用来支持一个已经说出的结论 |
| `layout.footer-heavy` | 重页脚 | 页脚本身是一个收束的大区域，放联系、地址或一句收尾，而不是四列小字 |
| `layout.manifesto` | 宣言大字 | 用极少的几句大字构成一节，适合开场或换章 |
| `layout.listing-map` | 列表加地图 | 一边是可筛选的结果，一边是地图或区域说明 |
| `layout.product-detail` | 产品详情 | 一件商品或一个套餐的购买区 |
| `layout.docs` | 文档三栏 | 目录、文章、页内目录 |
| `layout.resume` | 履历两栏 | 一侧是身份和联系，一侧是经历 |
| `layout.booking` | 预约时刻 | 选日期或场次，再留下联系方式 |
| `layout.matrix` | 功能对照表 | 用表比较方案或包含项 |
| `layout.hours` | 时间与地点 | 营业、上课或开放时间，加上地址 |
| `layout.menu-board` | 价目板 | 一份可以扫读的价目 |
| `layout.itinerary` | 行程日 | 按顺序的一天或一程 |
| `layout.property` | 房源参数 | 一套房或一间客房的头图加参数 |
| `layout.app-frame` | 设备框 | 一个真实界面放在简单的设备轮廓里，旁边是说明 |
| `layout.reel` | 主片加片单 | 一件主作品加可点的列表 |
| `layout.cta` | 结尾行动 | 一节只做一件事：重复页面的主动作 |
| `layout.newsletter` | 订阅 | 留下邮箱或电话以便以后联系 |
| `layout.search` | 搜索结果 | 一个搜索框加结果列表 |
| `layout.practice` | 业务领域 | 一组并列的服务范围，每项有边界 |
| `layout.announce` | 公告条 | 页面顶部一条可关闭的短消息 |
| `layout.footer-columns` | 多列页脚 | 页脚放栏目、联系和法务，分成清楚的几列 |
| `layout.image-grid` | 图片优先格 | 图是这一段的正文，说明永远可见 |
| `layout.case-study` | 案例长页 | 一件工作从上写到下 |
| `layout.changelog` | 版本记录 | 按版本把改动列出来，新的在上 |
| `layout.roadmap` | 三列路线 | 现在、接下来、以后，三列 |
| `layout.schedule` | 日程表 | 一天或一场的时间顺序 |
| `layout.roster` | 名册 | 一组真实的人，每人名字和角色 |
| `layout.mark-row` | 标识一排 | 用户已经提供的机构或工具标识，安静地排成一行 |
| `layout.hotspot` | 图上编号 | 一张图上的编号，对应旁边的一份列表 |
| `layout.spec-table` | 参数表 | 名称和值成对排列 |
| `layout.filter-grid` | 筛选加格子 | 上面或左侧是筛选，其余是结果格子 |
| `layout.article` | 正文边注 | 长文一栏，外侧放图注、定义或出处 |
| `layout.video-hero` | 影像首屏 | 首屏是一段用户提供的影像，字放在实色块上 |
| `layout.hero-form` | 标题加短表单 | 左边或上面是一句主张，旁边是一个短表单 |
| `layout.numbered` | 大号序号 | 01、02、03 配一句说明 |
| `layout.gallery-thumbs` | 主图加小图 | 一张主图，下面一排小图 |
| `layout.job-list` | 职位列表 | 开放的职位 |
| `layout.episode` | 单集 | 节目的一集：标题、播放、笔记、其他集 |
| `layout.recipe` | 配料与步骤 | 配料在前，步骤在后 |
| `layout.year-index` | 按年归档 | 条目按年份分组，新年份在上 |
| `layout.curriculum` | 课纲 | 课程分成模块，模块里是课 |
| `layout.status-board` | 状态板 | 若干组成部分和用户提供的状态 |
| `layout.not-found` | 找不到 | 访问的地址没有这一页 |
| `layout.waitlist` | 等候登记 | 一件还不能用的事，只收集联系方式 |
| `layout.legal` | 长法务 | 隐私、条款或版权说明，给读完用的 |
| `layout.colophon` | 版本说明 | 页尾或单独一页，写这页用的字、纸感以外的制作事实 |
| `layout.contact-sheet` | 接触印样 | 很多小图同一尺寸，像一张接触印样 |
| `layout.specimen` | 字体样本 | 展示这一页真正使用的字：大标题、一段正文、一组字符 |
| `layout.phases` | 阶段 | 一件工程或计划的前后阶段 |
| `layout.lineup` | 场次 | 演出、放映或比赛的场次列表 |
| `layout.sticky-buy` | 追随购买 | 详情往下走时，名称、价格和主按钮留在一栏里 |
| `layout.empty` | 空状态 | 这一段本来会有内容，但现在没有 |

## 特效

高成本，并且彼此只留一个：`fx.liquid`、`fx.glass`、`fx.goo`、`fx.displace`。

| id | 名称 | 是什么 |
|----|------|--------|
| `fx.grain` | 胶片颗粒 | 一层很细的噪点，让大色块不发闷 |
| `fx.paper` | 纸感 | 背景像纸，而不是塑料 |
| `fx.halftone` | 半调网点 | 印刷网点，用于海报和图，不用于正文 |
| `fx.hard-shadow` | 硬投影 | 没有模糊的偏移色块，用来把层分开 |
| `fx.sticker` | 描边贴纸 | 元素像剪下来贴上 |
| `fx.clip` | 几何裁切 | 用直线或一个弧把图裁出形状 |
| `fx.glow` | 局部辉光 | 一块柔光，用来把产品从底上托出来 |
| `fx.scan` | 扫描线 | 细横线暗示屏幕 |
| `fx.compress` | 压缩伪影 | 故意的低码率色带或块状，用在图上表达年代 |
| `fx.chroma` | 色差 | 高光边缘分开成两条色边 |
| `fx.pixel` | 像素位移 | 图按小格错位，像信号不稳，但停在一个可读的状态 |
| `fx.dof` | 景深模糊 | 前景清楚，远处或近处糊一点，把视线送到主体 |
| `fx.reflect` | 倒影 | 主体下面有一条变淡的倒影，像放在桌上 |
| `fx.cursor-shape` | 自定义光标外形 | 系统光标换成一个小圆或十字，用来强调这是一个可探索的页面 |
| `fx.liquid` | 液体置换 | 图像或标题边缘像液体一样被指针或滚动轻轻推开 |
| `fx.glass` | 单处折射 | 透过一块玻璃看见图被轻微扭曲 |
| `fx.goo` | 粘连 | 几个色块在靠近时融成一块，离开时再分开 |
| `fx.duotone` | 双色调 | 一张图只保留两种颜色，用来把照片收进版面 |
| `fx.dither` | 抖动 | 用有限的颜色和抖动点模拟层次 |
| `fx.spotlight` | 聚光 | 一块区域亮，周围暗，把视线送到主体 |
| `fx.vignette` | 暗角 | 画面四角略暗，像镜头边缘 |
| `fx.chrome` | 铬面 | 一个物件有金属高光，像抛过光 |
| `fx.iridescent` | 虹彩 | 表面随着角度轻轻变色，像薄膜 |
| `fx.light-leak` | 漏光 | 一条暖色或冷色的光渗进画面边缘 |
| `fx.double-exposure` | 双重曝光 | 两张图叠成一张，共享同一轮廓 |
| `fx.grid-overlay` | 坐标网格 | 一层细线网格，暗示图纸或早期屏幕 |
| `fx.dot-grid` | 点阵 | 规则的点，用来做安静的底或海报的一角 |
| `fx.wireframe` | 线框 | 物体或界面只用线表达 |
| `fx.hologram` | 全息 | 细的水平亮纹和轻微的透明感，像一块投影 |
| `fx.frost` | 磨砂 | 一块区域像磨砂玻璃，后面的颜色透出来，但形状看不清 |
| `fx.ink-bleed` | 洇墨 | 墨在纸上略微晕开 |
| `fx.stamp` | 印章 | 一个红或深色的印，用来标记日期、状态或刊号 |
| `fx.torn` | 撕边 | 纸的一边是撕开的 |
| `fx.noise-field` | 噪声场 | 比胶片颗粒更大块的明暗起伏，用来让一块平涂不那么死 |
| `fx.mesh` | 网格渐变 | 一块由两三个色标形成的柔和彩色底，用来代替纯色大底 |
| `fx.edge-blur` | 边缘渐变模糊 | 视口顶边或底边一条逐渐变实的模糊，用来托住固定导航 |
| `fx.metal-edge` | 金属边 | 一个物件或主按钮的一圈缓慢变化的亮边 |
| `fx.text-fill` | 字面填图 | 大标题的笔画里填进一张图或一条渐变 |
| `fx.polaroid` | 拍立得框 | 一组照片各有白边，略微转一点 |
| `fx.neon` | 灯管 | 一句标题或一块招牌像灯管，只亮这一处 |
| `fx.displace` | 局部置换 | 指针经过时，一张图的局部被轻轻推歪 |
| `fx.hatch` | 排线 | 细密的平行或交叉线，像刻出来的阴影 |
| `fx.topo` | 等高线 | 一圈圈等高线做块面的纹理 |
| `fx.foil` | 箔压 | 一个词或一个标记上有一小块金属反光 |
| `fx.paper-cut` | 层纸 | 两三层纸错开一点，形成简单的深度 |
| `fx.film-gate` | 片门 | 一张影像或照片套在片孔框里 |
| `fx.split-tone` | 分色 | 照片的暗部偏一种色，亮部偏另一种色 |
| `fx.outline-type` | 空心字 | 标题只有轮廓，没有填充 |
| `fx.ascii` | 字符密度 | 一张图用字符的疏密再呈现一次，作为装饰层 |

## 动画

滚动类里只留一个：`motion.pin-story`、`motion.horizontal`、`motion.image-sequence`、`motion.smooth-scroll`、`motion.infinite-columns`、`motion.video-scrub`。封面流转不再和轮播、横向画廊各做一套横移。

| id | 名称 | 是什么 |
|----|------|--------|
| `motion.fade-rise` | 淡入上移 | 内容进入视口时从下方 16px 到 24px 淡入 |
| `motion.mask-reveal` | 遮罩揭开 | 图或标题像从一条边被揭开 |
| `motion.word-stagger` | 逐词出现 | 标题按词依次出现，形成阅读节奏 |
| `motion.blur-in` | 由糊到清 | 元素从轻微模糊变为清晰，像对上焦 |
| `motion.scale-in` | 缩放落入 | 卡片或图从 0.96 放到 1，同时淡入 |
| `motion.parallax` | 视差 | 两层以不同速度移动，产生浅深度 |
| `motion.pin-story` | 钉住叙事 | 一节被固定在屏幕里，滚动改为推进这节内部的步骤 |
| `motion.horizontal` | 横向画廊 | 纵向滚动被这一节换成横向移动的一排作品 |
| `motion.velocity-skew` | 速度拉伸 | 快速滚动时，图片沿滚动方向轻微拉伸，停下后在 300ms 内回到正常 |
| `motion.card-stack` | 粘性卡片 | 卡片依次盖住上一张，用来比较三到五个步骤 |
| `motion.color-shift` | 滚动换色 | 滚动到新章节时，页面底色和字色一起换，用来分章 |
| `motion.image-sequence` | 图片序列 | 滚动进度对应一串帧，像产品旋转 |
| `motion.smooth-scroll` | 平滑滚动 | 滚轮和触控的滚动带一点惯性，让锚定动画更稳 |
| `motion.snap` | 章节吸附 | 滚动在章节之间靠齐，适合 `style.poster`、`style.cinematic` 这种一屏一章的页面 |
| `motion.magnetic` | 磁吸 | 指针靠近按钮时，按钮向指针移动几像素，离开后回到原位 |
| `motion.image-trail` | 图片轨迹 | 指针移动时在身后短暂留下小图，用来浏览一组作品 |
| `motion.tilt` | 悬停倾斜 | 卡片随指针轻微倾斜 |
| `motion.hover-swap` | 悬停换图 | 指针停在作品或商品上时，换成第二张真实图片 |
| `motion.curtain` | 帘幕转场 | 离开一页时一块实色盖住屏幕，新页面准备好后再揭开 |
| `motion.shared-element` | 共享元素 | 列表里的一张图过渡成详情里的同一张图 |
| `motion.marquee` | 跑马灯 | 一句口号或一串名称循环横移 |
| `motion.underline-draw` | 线条绘制 | 链接或章节标记的下划线从一侧画到另一侧 |
| `motion.count-up` | 数字计数 | 真实数字在进入视口时从 0 增到目标值 |
| `motion.kinetic-type` | 字距展开 | 大标题的字距从紧到正常，用来开场 |
| `motion.scramble` | 字符落定 | 标题先显示成无关字符，再从左到右落成真实句子 |
| `motion.typewriter` | 打字 | 文字像被逐字打出来 |
| `motion.text-swap` | 词语轮换 | 一个句子里的某个词轮流换成几个真实的词 |
| `motion.highlight-sweep` | 记号扫过 | 一条马克笔或下划线扫过句中的一个词 |
| `motion.shimmer` | 微光扫过 | 一条淡的高光从按钮或骨架上扫过，表示正在等待或此处可点 |
| `motion.accordion` | 折叠展开 | 问答或小节打开时高度展开，箭头或「打开」状态同时改变 |
| `motion.menu-overlay` | 全屏菜单 | 点开导航后，一块面板盖住内容，里面是完整的栏目 |
| `motion.scroll-progress` | 阅读进度 | 一条细进度表示文章读了多少 |
| `motion.nav-shrink` | 导航收缩 | 向下滚动后，导航变矮或收起说明，只留名称和主动作 |
| `motion.ken-burns` | 缓慢推近 | 一张静帧照片在原地极慢地放大或平移 |
| `motion.float` | 缓慢漂浮 | 一个装饰物件上下移动几个像素 |
| `motion.path-draw` | 路径绘制 | 一条真实的线被画出来，例如图纸引线或签名下划线 |
| `motion.preloader` | 开场加载 | 页面准备时有一个短的开场，然后进入内容 |
| `motion.carousel` | 轮播 | 一组同等重要的幻灯按顺序切换 |
| `motion.before-after` | 对比滑杆 | 一张图上用滑杆比较两个状态，例如改版前后 |
| `motion.filter-layout` | 筛选重排 | 筛选或排序后，条目移动到新位置 |
| `motion.text-focus` | 滚动点亮 | 长文里当前这一句变实，上下句变淡 |
| `motion.ripple` | 点击涟漪 | 按下按钮时从接触点扩出一圈 |
| `motion.cursor-spotlight` | 指针聚光 | 精细指针移动时，一块光跟着走，照亮下面的图 |
| `motion.infinite-columns` | 分栏对走 | 两列或三列图片以不同方向缓慢移动，用来浏览一组作品 |
| `motion.nav-hide` | 向下隐藏导航 | 页面向下走时导航收起，向上走一点就回来 |
| `motion.pointer-trail` | 光标拖尾 | 精细指针移动时，身后留下一小串很快消失的点或短线 |
| `motion.line-stagger` | 逐行出现 | 一段话按行出现，而不是按词 |
| `motion.shape-morph` | 形状渐变 | 一张图的裁切从一种简单形状过渡到另一种，进度跟这一段的滚动走 |
| `motion.circle-reveal` | 圆形揭开 | 一张图从中心的小圆张到完整，只播放一次 |
| `motion.coverflow` | 封面流转 | 几张封面呈浅浅的立体排列，中间一张是当前 |
| `motion.footer-reveal` | 页脚揭开 | 主内容像一张纸，卷走后露出底下的页脚 |
| `motion.page-wipe` | 页面擦除 | 在同一页里切换一整块视图时，用一块实色擦过，时长约 500ms |
| `motion.video-scrub` | 影像随滚动 | 一段很短的、用户提供的影像，播放进度等于这一段的滚动进度 |
| `motion.video-inview` | 进入后播放 | 影像有一半以上进入视口才播放，离开就暂停 |
| `motion.hover-lift` | 悬停抬起 | 卡片或按钮在悬停和键盘焦点时上移 4px |
| `motion.toc-spy` | 目录跟随 | 长文旁边的目录标出当前章节 |
| `motion.text-distort` | 标题扭曲 | 指针经过一句大标题时，笔画轻微扭曲，离开后回到原样 |
| `motion.frame-echo` | 叠影 | 一张图沿短距离重复 4 到 6 个淡下去的影子，像运动残留 |
| `motion.hotspot-pulse` | 编号轻跳 | `layout.hotspot` 上的编号点轻轻放大一次再回到原尺寸，用来表明它可以点 |
