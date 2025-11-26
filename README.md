# OpenReview-Score-Watcher


实时监控 ICLR 2026 论文评分变化的 Chrome 扩展

本插件自动追踪 OpenReview 上任意论文的分数变化，并以全局浮窗实时展示评分、均分与更新时刻。


📦 安装方法（开发者模式）

* 下载插件源码

* 打开 Chrome 并访问：chrome://extensions

* 开启右上角 开发者模式（Developer mode）

* 点击左上角 “加载已解压的扩展程序（Load unpacked）”

* 选择插件文件夹

* 安装完成后，右上角会出现插件图标。

🚀 使用方法
*打开 OpenReview 上的任意论文；例如：https://openreview.net/forum?id=xxxx

* 插件会自动：识别论文 forumId,将论文加入监控列表,在后台请求 OpenReview API

* 提取所有评分与 meta 信息 更新浮窗显示

* 浮窗会即时显示：(1) 论文标题（自动截断）(2) 论文 ID (3)所有当前评分（如 [6, 6, 4, 4]）(4)平均分 (5)最后更新时间
当前所在论文会绿色高亮。

🎛️ Update 1: 更新了拖拽以及移除功能
