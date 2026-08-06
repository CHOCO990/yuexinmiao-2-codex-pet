# 月薪猫2 Codex 桌宠

[中文 README](README.md) | [English README](README_EN.md)

这是一个可直接安装到 Codex 桌面端的本地宠物包。它保留了 **月薪猫2** 的主体动作，并整理成 Codex 可读取的 9 个标准动画行。

![月薪猫2 动作预览](assets/preview-standard-actions.png)

## 快速安装

1. 下载或克隆这个仓库。
2. 把下面这两个文件复制到本机的 Codex 宠物目录：

```text
pet.json
spritesheet.png
```

3. 目标目录如下：

```text
~/.codex/pets/yuexinmiao-2/
```

4. 重启 Codex，或者重新切换一次宠物。

如果你更习惯命令行，也可以直接运行：

```bash
mkdir -p ~/.codex/pets/yuexinmiao-2
cp pet.json spritesheet.png ~/.codex/pets/yuexinmiao-2/
```

## 文件一览

| 文件 | 作用 |
| --- | --- |
| `pet.json` | Codex 宠物配置，定义名称、描述和图集路径。 |
| `spritesheet.png` | 最终宠物图集，尺寸为 `1536 x 1872`。 |
| `assets/preview-standard-actions.png` | 9 个标准动作的预览图。 |
| `NOTICE.md` | 素材来源与署名说明。 |
| `LICENSE-NOTE.md` | 授权提醒。 |

## 动作列表

这个版本包含 9 个标准动作：

| 行号 | 动作 | 中文说明 | 帧数 |
| --- | --- | --- | ---: |
| 0 | `idle` | 待机 | 6 |
| 1 | `running-right` | 向右移动 | 8 |
| 2 | `running-left` | 向左移动 | 8 |
| 3 | `waving` | 挥手 | 4 |
| 4 | `jumping` | 跳跃 | 5 |
| 5 | `failed` | 失败/出错 | 8 |
| 6 | `waiting` | 等待用户 | 6 |
| 7 | `running` | 正在工作 | 6 |
| 8 | `review` | 审阅/检查 | 6 |

## 说明

- `waiting` 已替换为本地另一只月薪猫的等待动作。
- 最终图集使用 PNG，避免透明区域在 WebP 保存后留下残留颜色。
- 当前图集已经按 `1536 x 1872`、8 列 x 9 行的格式整理好。

## 排查

如果 Codex 里没有看到新宠物，可以检查：

1. `pet.json` 和 `spritesheet.png` 是否都在 `~/.codex/pets/yuexinmiao-2/` 目录下。
2. `pet.json` 里的 `spritesheetPath` 是否是 `spritesheet.png`。
3. 是否已经重启 Codex，或重新切换宠物。

## 适合谁

这个包适合想把月薪猫2 作为 Codex 本地宠物分享给朋友的人。

## 说明与来源

素材来源与署名请查看 `NOTICE.md`。在公开传播、二次创作或商用前，请先确认上游素材的授权范围。
