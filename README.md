# desk-pet

Codex 自定义桌宠仓库。目前收录两个可独立安装的阿衡形态：

- **九尾狐阿衡**：银白蓬松、深金眼睛、黑金尾尖和额心九边形星核。
- **白泽阿衡**：雪白蓬松、带月白玉角和琥珀金眼的幼年白泽。

## 九尾狐阿衡

![九尾狐阿衡侧身奔跑](docs/images/a-heng-side-run.gif)

![九尾狐阿衡触碰微跳](docs/images/a-heng-hover-microhop.gif)

![九尾狐阿衡等待和工作的动作对照](docs/images/a-heng-wait-work.gif)

- 宠物 ID：`a-heng`
- 当前版本：`v0.1.6`
- 图集规格：Codex v2，`1536×2288`，`8×11`，RGBA WebP
- 视觉特征：正面状态保持九条可数清的银白巨尾、流畅黑金尾尖、墨黑耳尖与小爪、额心黑色九边形星核
- 左右跑动：恢复初版侧身前倾、四肢舒展、尾群向后流动的奔跑姿态；侧视中允许九尾因透视自然遮挡
- 鼠标回应：沿用圆润的五帧微跳，起止帧的落脚高度对齐坐姿
- 等待时低头检查星纹尾尖，轻碰后收爪。原卷尾的位置和尾根连接保留，外缘的小尖角已收圆
- 工作时用双爪按住一张小纸片，低头核对
- 方向响应：完整 16 向追视，右下转向正下时尾扇的跳动更小。四个基准方向通过盲测，部分中间角度的转向较轻

[查看完整动作图集](docs/images/a-heng-contact-sheet.png) · [查看验证摘要](qa/a-heng-validation.json)

![白泽阿衡触碰回应](docs/images/baize-aheng-hover-response.gif)

## 白泽阿衡

- 宠物 ID：`baize-aheng`
- 图集规格：Codex v2，`1536×2288`，`8×11`，RGBA WebP
- 视觉特征：绒毛层次、珍珠釉面淡金纹、额心神目、墨绿色玉牌和祥云尾
- 鼠标回应：先停顿并竖耳，再抬爪招呼，最后稳定回到坐姿
- 跑动与触碰动作均已检查头身比例和尺寸连续性

[查看完整动作图集](docs/images/baize-aheng-contact-sheet.png) · [查看验证摘要](qa/validation.json)

## 安装

在仓库根目录选择喜欢的形态执行。

安装九尾狐阿衡：

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/pets/a-heng"
cp pets/a-heng/pet.json "${CODEX_HOME:-$HOME/.codex}/pets/a-heng/pet.json"
cp pets/a-heng/spritesheet.webp "${CODEX_HOME:-$HOME/.codex}/pets/a-heng/spritesheet.webp"
```

安装白泽阿衡：

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/pets/baize-aheng"
cp pets/baize-aheng/pet.json "${CODEX_HOME:-$HOME/.codex}/pets/baize-aheng/pet.json"
cp pets/baize-aheng/spritesheet.webp "${CODEX_HOME:-$HOME/.codex}/pets/baize-aheng/spritesheet.webp"
```

随后在 Codex 的“设置 → 宠物”页面点击刷新，并选择对应形态。

## 仓库口径

本仓库只保留当前最新版和必要的预览、验证摘要。旧版备份、生成缓存、临时图集及本机绝对路径均不纳入版本控制。
