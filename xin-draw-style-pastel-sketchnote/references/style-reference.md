# 视觉参考（不含布局）

`assets/samples/` 内 PNG 仅用于对齐**画风**，不要照搬其构图、分栏或步骤结构。排版由用户内容与任务自行决定。

## 从参考图提取什么

打开任意一张或多张样例，只校准下列视觉要素：

| 要素 | 观察要点 |
|------|----------|
| 线条 | 墨线略抖、约 2px、非 CAD 直线 |
| 底色 | 奶油白 `#FFF9F0`，无渐变 |
| 填色 | 低饱和柔彩块，同图种类少 |
| 容器 | 大圆角；实线外框 + 虚线子框可并存 |
| 间距 | 相邻元素疏朗（≥24px），框内 ≥12px；勿拥挤 |
| 字体 | 手写/圆体标题 + 清晰正文；**浅底墨字 / 深底白字**，禁止低对比 |
| 图标 | 简约线稿，少量平涂 |
| 装饰 | 星标/放射线稀疏；便签/胶带可选 |
| 连线 | 留空、够长；正交 L/之 形，勿迂回 U 折、勿穿框内字；见 SKILL.md |
| 气质 | 友好教程笔记，非冷色工程图 |

## Badcase（勿模仿）

| 文件 | 问题 | 正确做法 |
|------|------|----------|
| `badcase-arrow-line-too-short.png` | 连线/箭杆过短，与结构线堆积 | 元素间距 ≥16px，线段 ≥24px，与结构线间距 ≥8px |
| `badcase-text-low-contrast.png` | 深灰字在近黑底上无法阅读 | 浅底 `#1E293B`，深底 `#FFFFFF` |
| `badcase-connector-circuitous.png` | 连线迂回 U 折、穿过框内文字 | 最短正交路径，从对侧出入，走元素间隙 |

## 参考图列表（`assets/samples/`）

- `img_v3_02127_812b0b70-0810-4fe3-9ad7-def570fdf65g.png`
- `img_v3_02127_45b99c26-9096-47ea-9572-f21b8a4259bg.png`
- `img_v3_02127_0fd188d2-ab73-4d6b-ad55-321e4a82badg.png`
- `img_v3_02127_0ccd0961-6076-48f5-8bd8-9789341ad64g.png`
- `img_v3_02127_3729665a-2b8d-42d8-a3c6-5eea2e073e2g.png`
- `img_v3_02127_3d0bcdfe-3706-4a49-8100-b3409832fa6g.png`
- `img_v3_02127_9f9ac027-0001-44da-a184-4ba62e1020cg.png`
- `badcase-arrow-line-too-short.png`
- `badcase-text-low-contrast.png`
- `badcase-connector-circuitous.png`

## 维护

源文件可能在仓库根 `local/`。更新后同步：

```bash
cp local/*.png draw-style-pastel-sketchnote/assets/samples/
```
