# OpenReview-Score-Watcher
OpenReview Score Watcher

实时监控 ICLR / NeurIPS / OpenReview 论文评分变化的 Chrome 扩展

本插件自动追踪 OpenReview 上任意论文的分数变化，并以全局浮窗实时展示评分、均分与更新时刻。

✨ 功能特性
自动监控论文评分

自动解析 Reviews / Meta-Reviews

自动识别所有评分（如：[6, 6, 4, 4]）

自动计算平均分

无需刷新即可实时更新

全局浮窗显示

在任何网页都能看到监控列表

最近更新的 5 篇论文最先展示

当前浏览论文会自动高亮

支持多论文监控

打开任意论文页面会自动加入监控

最多保存 30 篇（自动清理最旧的）

可拖拽 + 收起展开 + 自动记忆状态

浮窗标题栏可拖拽到任意位置

支持收起 / 展开

自动记忆位置和折叠状态（浏览器重启也不丢）

支持删除论文监控

单篇论文支持一键删除

支持清空所有监控项

📦 安装方法（开发者模式）

下载插件源码（包含以下文件）：

manifest.json
background.js
content_script.js
icons/
  ├─ icon16.png
  ├─ icon64.png
  └─ icon128.png


打开 Chrome 并访问：

chrome://extensions


开启右上角 开发者模式（Developer mode）

点击左上角 “加载已解压的扩展程序（Load unpacked）”

选择插件文件夹

安装完成后，右上角会出现插件图标。

🚀 使用方法
① 打开 OpenReview 上的任意论文

例如：

https://openreview.net/forum?id=FmV289gGHp


插件会自动：

识别论文 forumId

将论文加入监控列表

在后台请求 OpenReview API

提取所有评分与 meta 信息

更新浮窗显示

② 浮窗展示内容

浮窗会即时显示：

论文标题（自动截断）

论文 ID

所有当前评分（如 [6, 6, 4, 4]）

平均分

最后更新时间

当前所在论文会绿色高亮。

🎛️ 浮窗操作说明
拖拽移动

按住标题栏拖动即可

自动记住位置，下次保持一致

收起 / 展开

点击右上角按钮

收起状态会自动记住

删除某论文

每个论文右上角会显示一个 ✕ 按钮

点击即可从监控列表中移除

清空全部监控

浮窗底部提供「清空全部」功能
