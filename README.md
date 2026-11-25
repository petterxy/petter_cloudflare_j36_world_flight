# 歼-36 · 环球飞行（J-36 World Flight）

一个循环播放的电影级飞行视频页面：歼-36 隐身战斗机载着两位特别机组人员，
在六条中国龙的环绕伴飞下，飞越珠穆朗玛峰、吉萨金字塔、万里长城，
最终冲出大气层环绕地球飞行。

## 制作管线

- 关键帧：阿里云百炼 `qwen-image-3.0-pro`（以真实照片为参考，保持人物面部一致）
- 视频：阿里云百炼 `wan3.0-video` 图生视频（720P）
- 剪辑：ffmpeg 拼接 + 交叉淡化
- 页面：纯静态单文件 `index.html` + `flight.mp4`，零外部依赖
- 部署：GitHub → Cloudflare Workers Builds（push 自动重建）

## 免责声明

本视频为 AI 生成的幻想作品：歼-36 为概念机型，龙为神话生物，
飞行轨迹与画面均为艺术创作，不代表真实飞行性能或真实事件。

## 姊妹项目

- [黎曼猜想 · 无限延续](https://petter-cloudflare-riemann-hypothesis.petter-xy.workers.dev)
- [考拉兹猜想 · 无限飞行](https://petter-cloudflare-collatz-conjecture.petter-xy.workers.dev)