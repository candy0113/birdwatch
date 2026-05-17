# BirdWatch 观鸟信息流体验

BirdWatch 是一个纯前端观鸟卡片 Web 应用，面向 AI 体验赛道演示。它模拟短视频信息流的竖屏浏览方式，并把识鸟、打卡、鸟点、鸟友动态和图鉴功能组织成可左右滑动的功能卡组。

在线体验：

https://candy0113.github.io/birdwatch/

## 核心体验

- 上下滑动浏览鸟类短视频，保持类似抖音信息流的沉浸感。
- 刷到功能卡组后，左右滑动切换不同观鸟工具。
- “识鸟”是第一张功能卡，突出听鸟叫识别鸟，并提供拍照识别、特征检索入口。
- “每日打卡”使用 `localStorage` 保存当天抽到的鸟卡，再次进入会提示“你又遇到了它”。
- “鸟点地图”展示附近和热门观鸟地点。
- “鸟友动态”展示附近实时鸟况，和鸟点地图明确分区。
- “鸟类图鉴”展示已收集的鸟卡。

## 技术约束

本项目不依赖后端服务，不调用外部付费 API。所有交互、状态和演示数据都在浏览器本地完成。

主要实现：

- 单文件 HTML/CSS/JavaScript 应用
- 本地视频素材
- DOM 虚拟化的竖向信息流
- 横向 `scroll-snap` 功能卡组
- `localStorage` 本地状态
- Web Audio 模拟鸟鸣识别反馈

## 项目结构

```text
.
├── index.html
├── birdwatch-optimized.html
├── assets/
│   └── videos/
│       ├── bird-eagle.mp4
│       ├── bird-humming.mp4
│       ├── bird-pelican.mp4
│       └── douyin-bird.mp4
└── README.md
```

## 本地预览

直接打开 `index.html` 即可预览。也可以使用任意静态服务器预览仓库根目录。

## GitHub Pages

仓库推送后，将 GitHub Pages 的发布源设置为：

- Branch: `main`
- Folder: `/ (root)`

设置完成后，访问：

https://candy0113.github.io/birdwatch/
