# OpenReview-Score-Watcher
实时监控 ICLR / NeurIPS / OpenReview 论文评分变化的 Chrome 扩展

本插件可自动监控 OpenReview 上任意论文的评审分数变化，并以全局浮窗持续展示。
不用刷新页面就能实时查看 reviewer 是否修改了评分。

非常适合在审稿季盯分数的你 :)

📦 安装方式（开发者模式）

下载插件源码文件夹，必须包含：

manifest.json
background.js
content_script.js
icons/
  ├─ icon16.png
  ├─ icon64.png
  └─ icon128.png


打开 Chrome 扩展管理页面：

chrome://extensions


右上角启用 开发者模式（Developer mode）

点击左上角 “加载已解压的扩展程序（Load unpacked）”

选择插件所在文件夹

加载完成后，浏览器右上角会出现插件图标。

🚀 使用方法
① 打开任意 OpenReview 论文页

示例：

https://openreview.net/forum?id=FmV289gGHp


插件会自动：

识别该论文 ID

将该论文加入监控列表

在后台调用 OpenReview API

抽取所有评审评分

更新并展示浮窗内容

② 浮窗显示评分信息

浮窗会展示如：

论文标题

论文 ID

评分：[6, 6, 4, 4]

平均分

最后更新时间

当你正在浏览该论文时，会自动高亮。

🎛️ 浮窗操作说明
拖拽移动

用鼠标按住浮窗的标题栏即可拖动

面板位置会自动保存，下次也保持一致

收起 / 展开

点击右上角 “收起 / 展开”

状态会自动记忆

删除单篇论文

在每个论文项右上角点击 ✕ 可删除该论文的监控记录

清空所有监控

在浮窗底部点击 “清空全部监控” 即可
