# desk-pet

Codex 自定义桌宠仓库。目前收录的是新版 **白泽阿衡**：一只雪白、蓬松、带月白玉角和琥珀金眼的幼年白泽。

![白泽阿衡触碰回应](docs/images/baize-aheng-hover-response.gif)

## 白泽阿衡

- 宠物 ID：`baize-aheng`
- 图集规格：Codex v2，`1536×2288`，`8×11`，RGBA WebP
- 视觉特征：绒毛层次、珍珠釉面淡金纹、额心神目、墨绿色玉牌和祥云尾
- 鼠标回应：先停顿并竖耳，再抬爪招呼，最后稳定回到坐姿
- 跑动与触碰动作均已检查头身比例和尺寸连续性

[查看完整动作图集](docs/images/baize-aheng-contact-sheet.png) · [查看验证摘要](qa/validation.json)

## 安装

在仓库根目录执行：

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/pets/baize-aheng"
cp pets/baize-aheng/pet.json "${CODEX_HOME:-$HOME/.codex}/pets/baize-aheng/pet.json"
cp pets/baize-aheng/spritesheet.webp "${CODEX_HOME:-$HOME/.codex}/pets/baize-aheng/spritesheet.webp"
```

随后在 Codex 的“设置 → 宠物”页面点击刷新，并选择“白泽阿衡”。

## 仓库口径

本仓库只保留当前最新版和必要的预览、验证摘要。旧版备份、生成缓存、临时图集及本机绝对路径均不纳入版本控制。
