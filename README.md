# Flowchart Preview

一个基于 Mermaid 的在线流程图预览工具，支持实时编辑、交互式操作和图片导出。

## 在线访问

https://guilingwn.github.io/flowchart-preview/flowchart-preview.html

## 功能特性

### 编辑与渲染
- 左侧代码编辑器，支持 Mermaid 语法输入
- 输入后自动渲染（600ms 防抖），也可 `Ctrl+Enter` 立即渲染
- 本地缓存自动保存，刷新页面恢复上次编辑内容

### 画布交互
- 鼠标滚轮缩放（以鼠标位置为锚点）
- 拖拽平移画布，带物理惯性效果（根据图表大小自适应）
- 双击空白区域自适应窗口
- 双击文本可选中复制

### 节点拖拽
- 开启「拖拽节点」模式后，可自由拖动流程图节点
- 连接箭头自动跟随重绘，保留箭头样式
- 边上的标签文本同步移动

### 导出
- 导出为 PNG（2倍分辨率高清）
- 导出为 SVG（矢量格式）

## 快捷键

| 操作 | 快捷键 |
|------|--------|
| 渲染 | `Ctrl+Enter` |
| 放大 | `+` / 滚轮上 |
| 缩小 | `-` / 滚轮下 |
| 适应窗口 | `0` / 双击空白 |
| 平移 | 鼠标拖拽 |

## 技术栈

- [Mermaid.js](https://mermaid.js.org/) v10 - 流程图渲染
- [html-to-image](https://github.com/bubkoo/html-to-image) - PNG 导出
- 原生 JavaScript - 交互逻辑（缩放、拖拽、惯性、节点拖拽）
- localStorage - 编辑内容持久化
