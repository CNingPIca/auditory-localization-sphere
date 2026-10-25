# 听觉方位球 · Auditory Localization Sphere

以人头为中心的 3D 交互可视化：对比人耳天然的定位能力，和单声道、立体声、5.1、7.1、5.1.2、7.1.4、9.1.6、回音壁、各类空间音频耳机等重放系统在每个方向上的还原精度。

同一个可视化的两个版本并列保存，可以任选一个来展示。

## 版本

| 版本 | 目录 | 空间分辨能力的画法 | 日期 |
|---|---|---|---|
| v1.0.0 | [`v1-heatmap/`](v1-heatmap/index.html) | 球面热力图 + 精度椭圆 + 听感分区色块 | 2026-10-19 |
| v2.0.0 | [`v2-pointcloud/`](v2-pointcloud/index.html) | 三维点云（疏密 + 颜色）+ 低多边形写实头像 | 2026-10-25 |

在线演示：[版本选择首页](https://cningpica.github.io/auditory-localization-sphere/) · [v1 热力图版](https://cningpica.github.io/auditory-localization-sphere/v1-heatmap/) · [v2 点云版](https://cningpica.github.io/auditory-localization-sphere/v2-pointcloud/)

## 怎么打开

- **在线**：打开上面的演示链接，首页可以选版本。
- **本地**：每个版本都是单个 HTML 文件，下载后直接双击 `index.html`。联网时会加载网页字体，离线也能运行（自动换成系统字体）。

## 分支与版本管理

| 名称 | 类型 | 内容 |
|---|---|---|
| `main` | 分支 | 最新状态，两个版本并列放在各自目录里，GitHub Pages 从这里发布 |
| `release/v1` | 分支 | v1 这条线的维护分支，以后 v1 的小修改在这里做 |
| `release/v2` | 分支 | v2 这条线的维护分支 |
| `v1.0.0`、`v2.0.0` | 标签 | 每个版本发布时的快照，永远不变 |

以后的约定：

- 出一个**新的大版本**：新建目录 `vN-名称/`，在 `main` 上提交，打标签 `vN.0.0`，并从这个提交建 `release/vN` 分支。
- 对某个版本**小修**：在对应的 `release/vN` 分支上改，打标签 `vN.1.0`、`vN.1.1`……，再合并回 `main`。
- 每次的变化写进 [CHANGELOG.md](CHANGELOG.md)。

## 说明

各数值是为了比较不同布局的趋势，不是实测结果；模型细节写在页面底部。
