# ConceptLine · AI Timeline

静态单页知识时间轴原型，当前版本：v1.2.0。

## v1.2 更新

- 增加“卡片时间轴 / 刻度时间轴”双模式。
- 刻度时间轴按真实年份定位节点，日期、标题、描述分层显示。
- 增加时间轴缩放滑杆，可放大查看密集年份。
- 搜索框支持快速定位，输入关键词后自动选中并滚动到第一个匹配节点。
- 增加 AI 产品 / AI 软件图标：优先使用产品官网 favicon，无法加载时自动回退为首字母圆标。
- 扩充国内外 AI 产品时间线，包括 DeepSeek、豆包、通义千问、Kimi、腾讯元宝、文心一言、讯飞星火、智谱清言、可灵、海螺、即梦、Vidu、Trae、OpenCode、Open Design 等。
- 知识点详情增加官网 / 产品页、Google 搜索、维基百科搜索、Google Scholar 等外部资料入口。

## v1.1 更新

- 增加主题模式：默认跟随系统，可切换浅色 / 深色 / 系统。
- 修复底部时间轴 hover 卡片被滚动容器遮挡的问题，改为全局浮层提示。
- 改为 100dvh 应用式布局：整体页面不产生浏览器级滚动条，内容区内部滚动。
- 弹窗和当前知识卡片增加外部资料入口。
- 点击网站 Logo 返回首页状态。
- 扩充 AI 专业热词与节点。

## 运行

```bash
cd concept-line
python -m http.server 8080
```

访问：

```txt
http://localhost:8080
```

也可以直接双击 `index.html` 打开。Lucide 图标使用 CDN；产品图标使用 favicon 外链。如果离线打开，页面内容和交互仍可使用，外部图标可能显示为首字母回退样式。

## 数据

时间轴数据位于：

```txt
data/ai-timeline.json
```

单文件版本也把同一份 JSON 内嵌在 `index.html` 的 `#timeline-data` 中。

## 数据规模

- 时间轴节点：84 个
- AI 产品 / 软件节点：45 个
- 热词词条：46 个
- 国产 AI 产品节点：17 个

## 主要文件

```txt
concept-line/
├─ index.html
├─ README.md
└─ data/
   └─ ai-timeline.json
```
