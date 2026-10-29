# 世界熵 · 卡牌数据库

这是《世界熵》DEMO 的独立卡牌数据库。程序通过稳定的 `id` 与 `effect` 标识引用卡牌，美术则通过 `art` 文件名关联图片资源库。

## 文件

- `cards.json`：当前 DEMO 的 13 张卡牌；O1000 仅作为系统备用主世界生成，不进入固定卡组。
- `schema.json`：卡牌数据结构与四维字段约束。
- `keywords.json`：词条及程序结算口径。
- `CHANGELOG.md`：数值和文字版本记录。

## 四维字段

| 字段 | 中文 |
| --- | --- |
| `chaos` | 混沌 |
| `barren` | 荒芜 |
| `disqualification` | 失格 |
| `calamity` | 厄孳 |

数值为 0～6；特殊值可使用 `-` 或 `?`。新增卡牌时，应同时更新图片仓库中的同名资源，并在主 DEMO 的效果表中实现新的 `effect` 标识。

## 关联仓库

- 主程序：https://github.com/Rosmontic/world-entropy-demo
- 图片资源：https://github.com/Rosmontic/world-entropy-assets

本仓库仅保存数据，不依赖主程序即可校验、 diff 和复用。
