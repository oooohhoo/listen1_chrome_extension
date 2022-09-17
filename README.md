# Listen 1 (Chrome Extension) V2.26.2

（最后更新于 2022 年 09 月 17 日）

[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE)

[English Version](https://github.com/listen1/listen1_chrome_extension/blob/master/README_EN.md)

## 缘起

当我发现找个想听的歌因为版权听不了，需要打开好几个网站开始搜索，来回切换让我抓狂的时候，我知道是时候该做点什么了。

妈妈再也不用担心我找不到我想听的歌了。

支持音乐平台

- 网易云音乐
- QQ 音乐
- 酷狗音乐
- 酷我音乐
- bilibili
- 咪咕音乐
- 千千音乐

搜歌，听歌，就用 `Listen1`。

[![imgur](https://i.imgur.com/dIVFtor.gif)]()

V2.9.0 新特性：自动切换播放源(Beta)

当一首歌的播放源不可用时，会自动搜索其他平台，获得可用的播放源。避免了用户手动搜索的麻烦。

还有精选歌单哦。

## 官方商店安装（推荐）

按你的浏览器类型点击下面的链接安装

- [Chrome Web Store 安装](https://chrome.google.com/webstore/detail/listen-1/indecfegkejajpaipjipfkkbedgaodbp)
- [FireFox 安装](https://addons.mozilla.org/zh-CN/firefox/addon/listen1/)
- [Microsoft Edge 安装](https://microsoftedge.microsoft.com/addons/detail/hneiglcmpeedblkmbndhfbeahcpjojjg)

感谢 [@TNT-c](https://github.com/TNT-c) 维护 Firefox 的发布渠道

感谢 [@dhxh](https://github.com/dhxh) 维护 Microsoft Edge 的发布渠道

## Chrome 下载安装

1. 下载项目的 zip 文件，在右上方有个 `Download ZIP`, 解压到本地

2. chrome 右上角的设置按钮下找到更多工具，打开`扩展程序`

3. 选择 `加载已解压的扩展程序`(如果没有显示先选中`开发者模式`)，选中解压后的文件夹，完成！

## Firefox 打包安装

1. 将根目录下 manifest_firefox.json 替换 manifest.json

2. `cd listen1_chrome_extension`

3. `zip -r ../listen1.xpi *`, 完成打包 xpi 文件

4. 打开 Firefox，加载 xpi 文件，完成安装

## QQ 音乐举报 Listen1 导致代码库临时关闭事件 （2017 年 11 月）

Listen1 的用户，有个坏消息希望和大家分享。Listen1 最近收到了[QQ 音乐的 DMCA Takedown Notice](https://github.com/github/dmca/blob/master/2017/2017-11-17-Listen1.md), 主要代码库已经因为此原因而临时关闭。悲观一点看，Listen1 项目可能会在今年内彻底消失。

Listen1 诞生的初衷从不是和大公司的争夺版权利益，而是为了给予热爱音乐的人更好的收听体验，所以，Listen1 是开源，免费的，并且不接受任何形式的捐助。正是因为有热爱音乐的 Listen1 的你们，Listen1 才发展到今天这一步。不管结果如何，Listen1 团队感谢所有支持过这个项目的人们。

在这个关系项目生死存亡的时刻，我寻求项目因为 DMCA 被 github 关闭的援助。如果有对这个比较了解如何解决的人，或者你想对这个事情发表看法和建议，可以在[issue](https://github.com/listen1/listen1_chrome_extension/issues/113)留言，或者发送邮件到 githublisten1@gmail.com。我们会尽最大努力，来守护 Listen1，即使可能它即将成为历史。

## 更新日志

`2022-09`

功能改进

- 添加现代白，现代黑两款主题（感谢 @814959822 的提交）
- 优化了新主题性能

`2022-08`

修复：

- 修复开启一段时间后无法播放的问题 #902 （感谢 @reserveword 的提交）
- 修复 QQ 音乐无法搜索的问题 (感谢 lx-music-desktop 提供技术方案)
- 修复 bilibili 搜索没有响应的问题

`2022-07`

功能改进：

- 增加 bilibili 视频音源搜索功能

修复：

- 修复酷狗音乐的播放错误
- 修复酷狗音乐热门歌单加载更多时的错误
- 修复 qq 音乐歌手页的错误
- 修复咪咕音乐排行榜打开时的错误

`2022-06`

功能改进

- 添加双击歌单列表和搜索结果列表播放（感谢 @piz-ewing 的提交）
- 桌面版本地音乐增加 wav 格式支持 (感谢 @mikelxk 的提交)

  修复：

- 修复清空列表当前播放音乐不停止的问题(感谢 @leca 的提交）
- 酷狗音乐列表无法打开的问题
- 修复随机播放模式出现重复音乐的 bug (感谢 @piz-ewing 的提交)

`2022-02 ~ 2022-03`

功能改进：

- 增加韩语支持（感谢 @kkange 的提交）

修复：

- 酷狗音乐无法播放的问题
- 千千音乐列表接口无法访问的问题（感谢 @mikelxk 的提交）

`2021-08 ~ 2022-01`

修复：

- 修复音乐分类按钮显示没有间距的问题 （感谢 @yinzhenyu-su 的提交）
- 修复在 firefox 无法打开 bilibili 音乐的问题 (感谢 @ktmzcpl 的提交)
- 修复在 electron 环境启动时的 UI 崩溃问题

优化：

- 更平滑的当前播放切换效果 (感谢 @mikelxk 的提交)

`2021-07`

修复：

- 禁止图片拖动
- 增加快捷键中放大缩小功能的描述
- 修改 windows 用户的窗口控制按钮位置到右上角 (感谢 @mikelxk 的提交)
- 升级 howler 库 (感谢 @mikelxk 的提交)
- 修复 QQ 音乐无法搜索的问题
- 修复 chrome 浏览器媒体控制中进度条拖动的问题 (感谢 @mikelxk 的提交)
- 增加本地音乐的本地 lrc 歌词文件支持 (感谢 @mikelxk 的提交)

`2021-04`

功能改进：

- 增加 QQ 音乐的登录支持
- 增加拖拽支持，支持歌单内歌曲调整顺序，歌单调整顺序，正在播放歌曲调整顺序，以及拖动歌曲加入歌单的操作
- 支持歌单内搜索
- 桌面版支持代理设置
- 支持配置自动切换源的搜索平台
- 增加显示当前最新版本
- 增加对网易云平台的默认高码率音源支持

重构和优化：

- 将音乐平台接口做 class 改造 #553
- github 模块去除 angular 依赖 #532 (感谢 @Dumeng 的提交)
- lastfm 模块去除 angular 依赖 #532 (感谢 @Dumeng 的提交)
- 优化 UI 细节，提升用户体验 #537

修复：

- 修复需要登录才能获取咪咕播放链接，并增加码率数据 #536 (感谢 @RecluseWind 的提交)
- 修复音乐榜和影视榜在 Firefox 上的不能正确获取的 bug #536 (感谢 @RecluseWind 的提交)
- 修复某些情况下歌曲在播放前总是等待 15 秒的 bug
- 修复 QQ 音乐短链接歌单分享地址不被识别的问题
- 修复开启关闭静音功能失效的问题
- 修复 GitHub 账户无法退出的问题
- 修复 kugou 部分音乐因专辑缺失导致的播放错误
- 修复多首歌曲重复播放的问题

`2021-03`

功能改进：

- 新增千千音乐平台 (感谢 @Dumeng 的提交)
- 支持咪咕音乐的分类歌单和排行榜歌单功能 (感谢 @RecluseWind 的提交)
- 桌面版支持放大功能 (感谢 @mikelxk 的提交)
- 支持网易登录功能，支持打开我的歌单和推荐歌单
- 支持咪咕登录功能
- 支持在正在播放页面显示当前播放歌曲的码率和平台
- 移除虾米平台

重构和优化：

- 替换了对 translate，i18n, hotkeys 的 angular 模块依赖，替换为纯 js 库 (感谢 @Dumeng 的提交)
- 优化载入 feather 图标库的效率 (感谢 @Dumeng 的提交)
- 改善了多个平台默认码率，默认播放高码率音乐文件
- 将 app.js 按多个 controller 模块分为多个文件
- 优化显示了因为版权问题无法播放的通知
- 将大部分链接改成 https 协议

修复：

- 修复新语法导致媒体控制在某些系统中不可用的问题 (感谢 @mikelxk 的提交)
- 修复音量控制快捷键失效的问题 (感谢 @mikelxk 的提交)
- 修复了在 firefox 上的滚动条样式 (感谢 @RecluseWind 的提交)
- 修复酷狗音乐封面的错误
- 修复酷狗某些歌曲不能播放的问题
- 修复通知无法显示的问题
- 修复了删除当前播放列表歌曲后导致的各种异常

`2021-02`

功能改进：

- 支持分类歌单和排行榜（感谢 https://github.com/lyswhut/lx-music-desktop 提供 QQ 音乐排行实现）
- 增加繁体中文翻译 (感谢 @yujiangqaq 提供翻译)
- 增加 chrome 媒体控制上一曲，下一曲和快进快退 （感谢 @mikelxk 的提交）
- 改进桌面版桌面歌词，增加字体大小颜色设置和背景透明度调整

重构：

- 将媒体资源服务重构成 MediaService 模块，除去对 angularjs 的依赖 （特别感谢 @Dumeng 的提交）
- 增加 prettier 配置文件和 commit 前检查 （感谢 @mikelxk 的提交）
- 修正一些过往代码的格式错误 （感谢 @mikelxk 的提交）

修复：

- 修复 Github API （感谢 @NoDocCat 和 @Dumeng 的提交）
- 修复因 svg 动画导致的性能问题 （感谢 @Dumeng 的提交）
- 修复虾米部分失效 API（感谢 @RecluseWind 的提交）
- 修复 Mac 桌面版无法导入本地音乐的问题 （感谢 @virgil1996 的提交）
- 修复酷我搜索出错的问题

`2021-01`

功能改进：

- 支持插件版后台播放功能 (特别感谢 @Dumeng 的提交)
- 优化酷我代码 (感谢 @RecluseWind 的提交)
- 优化咪咕音乐代码 (感谢 @RecluseWind 的提交)
- 本地音乐支持 flac 格式 (感谢 @mikelxk 的提交)
- 在软件中增加反馈链接 (感谢 @mikelxk 的提交)
- 增加虾米歌单搜索，统一端口代码 (感谢 @RecluseWind 的提交)
- 优化了歌单访问，增加本地缓存

重构：

- 更换所有加解密库到 forge (感谢 @Dumeng 的提交)
- 去除对 jquery 库的依赖 (感谢 @Dumeng 的提交)
- 更换音频播放库到 howler.js (感谢 @Dumeng 的提交)
- 更换 http 请求库到 axios (感谢 @Dumeng 的提交)
- 支持 eslint 的 github action 语法检查 (感谢 @Dumeng 的提交)

bug 修复：

- 修复 MediaSession 不支持时的报错问题 (感谢 @Jyuaan 的提交)
- 修复咪咕歌单的 404 错误
- 修复正在播放窗口点击空白处弹回的功能 (感谢 @Demeng 的提交)

`2020-12-28`

- 修复最大，最小，关闭按钮在桌面版失效的问题

`2020-12-27`

- 修复无法显示收藏歌单的 bug
- 支持一次输入搜索所有平台（Beta）
- 修复咪咕音乐歌单只显示前 20 首歌的 bug
- 修复网易和酷狗音乐搜索错误未处理的 bug
- 修复虾米音乐歌词解析错误导致无法显示的 bug
- 根据 chrome web store 上架要求修改部分权限

`2020-12-22`

- 修复酷我音乐无法播放的问题
- 修复我创建的歌单升级后无法播放的问题

`2020-12-20`

- 修复版权问题造成的播放中断和循环弹出提示通知的 bug
- 修改歌曲封面为背景时歌词看不清的问题
- 修复 qq 搜索的一个错误，优化接口返回时处理（感谢@RecluseWind 的提交）

`2020-12-12`

- 支持 QQ 音乐歌单搜索 (感谢@RecluseWind 的提交）
- 修复网易云音乐无法打开手机分享的歌单链接的 bug (感谢@RecluseWind 的提交）
- 修复咪咕音乐无法搜索的 bug

`2020-10-28`

- 增加本地音乐（仅限桌面版）

`2020-10-27`

- 增加歌单搜索功能（暂时只支持网易云）
- 优化歌词显示
- 修复 blili 歌手 API 错误，修复歌词时间轴格式不统一产生的错误 (感谢@RecluseWind 的提交)
- 优化 UI，正在播放页增加翻译按钮

`2020-10-26`

- 增加歌词翻译功能 QQ 音乐和虾米音乐的支持（感谢@RecluseWind 的提交)
- 更新了虾米音乐获取歌曲播放地址，获取歌单，搜索 API 的获取方式，增加可靠性 (感谢@RecluseWind 的提交)
- 修复安装插件后 qq 音乐网页部分歌单无法打开的 bug

`2020-10-18`

- 增加歌词翻译功能，暂时只支持网易云音乐 (感谢@reserveword 的提交)
- 修复 bilibili 音乐无法播放的 bug
- 修复虾米播放页歌曲封面无法显示的 bug
- 修复酷我音乐歌单无法打开的 bug

`2020-09-12`

- 修复网易歌单超过 1000 首时导入失败的 bug (感谢@YueShangGuan 的提交）
- 支持显示歌曲封面作为正在播放背景 (感谢@YueShangGuan 的提交）

`2020-08-24`

- 修复虾米歌单歌曲只显示部分歌曲的 bug (感谢@RecluseWind 的提交)
- 修复歌单图片和标题显示问题 (感谢@RecluseWind 的提交)
- 支持桌面版点击链接打开系统默认浏览器

`2020-08-04`

- 增加正在播放窗口和播放列表弹窗的动画效果
- 修复虾米艺人封面图片无法显示的问题 （感谢@RecluseWind 的提交）
- 优化打开歌单功能，支持网易云排行榜单，艺人页面，专辑页面网址（感谢@whtiehack 的提交）
- 优化专辑图片显示，避免图片被压缩 （感谢@RecluseWind 的提交）

`2020-07-10`

- 修复咪咕音乐无法播放的问题
- 支持顶部搜索栏回车触发 （感谢@kangbb 的提交）
- 支持歌单歌曲数显示，支持播放/暂停全局快捷键（桌面版）（感谢@x2009again 的提交）
- 支持返回时回到滚动条历史位置（感谢@x2009again 参与完成）
- 优化 firefox 滑动条，修改 qq 音乐图标网址，解决 firefox 上架 jquery 代码问题 （感谢@RecluseWind 的提交）

`2020-06-29`

- 支持播放失败时自动切换播放源(Beta)

`2020-06-28`

- 修复网易歌单仅显示 10 首歌曲的问题

`2020-04-30`

- 修复咪咕音质较差的问题

`2020-04-27`

- 增加收藏歌单功能，特别感谢 @zhenyiLiang
- 修复咪咕音乐无法播放的 bug
- 一些细节优化

`2019-11-27`

- 加入法语支持, 特别感谢 @Leoche

`2019-09-07`

- 修复 migu 无法播放的 bug

`2019-08-09`

- 增加深色主题

`2019-07-03`

- 修复咪咕音乐无法播放的 bug

`2019-06-24`

- 增加咪咕音乐
- 修复网易音乐无法播放的 bug
- 修复酷狗音乐无法播放的 bug

`2019-06-23`

- 修复无法连接到 github 的 bug

`2019-05-26`

- 修复酷狗音乐无法播放的 bug

`2019-04-26`

- 修复虾米音乐无法播放的 bug
- 修复播放器未在页面底端显示的 bug

`2019-03-03`

- 修复删除单个歌曲导致歌单所有歌曲消失的 bug
- 修复删除单个歌单导致所有歌单消失的 bug

`2019-02-26`

- 修复 qq 音乐歌单无法显示的 bug

`2018-12-30`

- 修复酷我音乐歌单缺失歌曲的问题
- 自动检测客户端语言

`2018-12-29`

- 修复虾米音乐搜索失败的问题
- 修复部分 QQ 音乐歌曲无法播放的问题
- 修复使用插件时 QQ 官方网站无法使用的问题

`2018-12-24`

- 多语言支持，支持英文
- 新添加到歌单的歌曲将出现在歌单头部
- 修复版权通知占满屏幕的 bug

`2018-12-22`

- 全新版本 2.0 发布，更新界面(特别感谢@iparanoid 提供主题设计)
- 升级 jquery 和 angular 版本

`2018-12-21`

- 修复虾米音乐歌单访问的问题
- 修复网易云音乐歌单只有一首歌的问题
- 修复 bilibili 滚动时加载重复歌单的问题
- 修复酷狗部分音乐无法播放的问题
- 修复 Github Gist 备份无法导入的问题
- 升级 soundmanager2 库到最新版本

`2018-12-05`

- 完全修复虾米音乐歌单访问的问题

`2018-08-25`

- 修复虾米音乐无法播放的 bug

`2018-06-15`

- 增加酷我音乐的支持（特别感谢@WinterXMQ 的提交)

`2018-06-10`

- 修复酷狗音乐收藏歌单后可能显示空歌单的 bug

`2018-06-10`

- 修复虾米音乐无法显示歌词的 bug

`2018-06-05`

- 增加酷狗音乐的支持（感谢@WinterXMQ )

`2018-05-30`

- 修复 QQ 音乐无法播放的问题（感谢@noschoollee 提供修复方案）

`2018-04-23`

- 修复虾米音乐无法播放的问题

`2018-02-18`

- 修复无法创建歌单的 bug
- 修复点击关闭歌单按钮后无法再打开歌单的 bug
- 增加歌曲主页，点击封面可进入（特别感谢@iparanoid 提供歌曲页面 UI 设计）

`2018-02-15`

- 修复随机播放在播放列表播放结束后自动停止的问题，开启无限洗脑循环（感谢@sunjie21 的提交）
- 增加将当前播放列表全部添加到歌单的功能 (感谢@sunjie21 的提交)
- 修复标题播放状态不实时更新的 bug (感谢@sibojia 的提交)

`2018-02-14`

- 修复主页在加载更多数据时出现双重滚动条的 bug，并修改了滚动条样式（感谢@zhuzhuyule 的提交)
- 修复打开歌单时，网易云音乐个人歌单地址无法解析的 bug（感谢@zhuzhuyule 的提交)

`2017-12-26`

- 增加同步歌单到 Github Gist 功能。(特别感谢@ConstLhq 提供创意和部分代码实现）

`2017-12-20`

- 增加搜索翻页功能，你可以看到更多的搜索结果了。(感谢@ConstLhq 的提交）
- 增加合并歌单功能。可以快速的把其它你创建的歌曲合并到当前的歌单中了。(感谢@Dumeng 的提交）

`2017-11-27`

- 修复网易云音乐歌单只显示第一首歌的 Bug（感谢[@Binaryify/NeteaseCloudMusicApi](https://github.com/Binaryify/NeteaseCloudMusicApi)提供接口实现）

`2017-11-18`

- 修复版权原因无法播放歌曲时自动暂停的问题

`2017-11-17`

- 在我的歌单页面增加“打开歌单”功能，可打开支持网页的歌单链接地址。这样就可以导入你喜欢的歌单了。
- HTTP 请求头部的 Origin 字段设置为正常网址

`2017-10-16`

- 修复 QQ 音乐歌单翻页显示重复的问题(感谢@Moobusy 的提交)

`2017-10-03`

- 修复网易云音乐歌单无法显示的问题(感谢@Moobusy 的提交)

`2017-09-14`

- 修复 QQ 音乐无法播放的 bug

`2016-05-27`

- 增加快捷键功能（输入?查看快捷键设置）
- 支持同步播放记录到 last.fm
- 增加搜索 loading 时的图标(感谢@richdho 的提交）
- 页面标题增加显示当前播放信息
- 修复了在收藏对话框点击取消出现新建歌单的 bug
- 重新组织代码文件夹结构

`2016-05-21`

- 增加歌单分页加载功能(感谢@wild-flame 的提交)
- 修复关闭按钮随网页滚动的 bug
- 修复点击暂停按钮会重置进度条和歌词的 bug
- 修复点击歌单名称不跳转的 bug
- 调整歌单水平位置居中

`2016-05-14`

- 增加 firefox 插件支持（感谢 fulesdle 的提交）

`2016-05-13`

- 增加我的歌单功能，可以收藏现有歌单，并创建自己的歌单
- 点击 Listen 1 和图标可以回到首页
- 标记了部分因版权无法播放的歌曲,增加版权提示
- 重构了音乐平台代码，使用统一的接口规范
- 重构了歌单接口，合并歌手，专辑和歌单接口
- 修复了阿里云歌手链接点击错误的 bug

`2016-05-08`

- 增加歌词显示
- 精选歌单：添加歌单到当前播放列表，可点击跳转到原始链接
- 修复了搜索 qq 音乐时的乱码问题
- 修复了循环播放网易歌曲一段时间后暂停的 bug
- 修复了可能导致微信公众号无法登录的 bug
- 优化性能，删除了不必要的事件消息触发

`2016-05-02`

- 增加音量控制

## License

MIT
