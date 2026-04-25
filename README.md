# ghostty-config

![类型](https://img.shields.io/badge/%E7%B1%BB%E5%9E%8B-%E9%85%8D%E7%BD%AE%E4%BB%93%E5%BA%93-2563eb)
![技术栈](https://img.shields.io/badge/%E6%8A%80%E6%9C%AF%E6%A0%88-Ghostty%20Config-0f766e)
![状态](https://img.shields.io/badge/%E7%8A%B6%E6%80%81-%E4%B8%AA%E4%BA%BA%E9%85%8D%E7%BD%AE-f59e0b)
![README](https://img.shields.io/badge/README-%E4%B8%AD%E6%96%87-111827)

个人 Ghostty 终端配置仓库，当前提供一个基于 Gruvbox Dark Hard 的深色主题配置。

## 仓库定位

| 项目 | 说明 |
| --- | --- |
| 分类 | 配置仓库 / 终端主题 / Ghostty profile |
| 面向对象 | 想复用或参考 Ghostty 深色主题、字体、窗口和光标设置的个人环境 |
| 当前配置 | `configs/gruvbox-dark-hard/config` |
| 边界 | 仓库只保存配置文件，不包含安装器、自动同步脚本或跨平台适配逻辑 |

## 可用配置

| 配置 | 说明 |
| --- | --- |
| `gruvbox-dark-hard` | 基于 `Gruvbox Dark Hard`，使用 `MonoLisa Variable` 字体、轻微透明、背景模糊、窗口 padding 和选中即复制 |

## 使用方式

复制指定 profile 到 Ghostty 配置路径：

```bash
mkdir -p ~/.config/ghostty
cp configs/gruvbox-dark-hard/config ~/.config/ghostty/config
```

复制后重启 Ghostty，或按你的本地方式重新加载配置。

## 配置摘要

| 设置 | 当前值 |
| --- | --- |
| `theme` | `Gruvbox Dark Hard` |
| `font-family` | `MonoLisa Variable` |
| `font-size` | `12` |
| `window-width` / `window-height` | `110` / `30` |
| `background-opacity` | `0.95` |
| `background-blur-radius` | `20` |
| `cursor-style` | `block` |
| `cursor-style-blink` | `true` |
| `cursor-opacity` | `.8` |
| `macos-titlebar-style` | `tabs` |
| `window-padding-x` / `window-padding-y` | `15` / `10` |
| `copy-on-select` | `clipboard` |

## 项目结构

```text
.
├── README.md
└── configs/
    └── gruvbox-dark-hard/
        ├── README.md
        └── config
```

## 调整建议

- 如果本机没有安装 `MonoLisa Variable`，请把 `font-family` 和 `window-title-font-family` 改成本机可用字体。
- 如果不想启用背景透明或模糊，可以调整 `background-opacity` 和 `background-blur-radius`。
- 如果不希望选中文本时自动复制，可以移除或修改 `copy-on-select = clipboard`。

## 备注

- 当前只有一个 profile，新增主题时建议放在 `configs/<profile-name>/` 下，并补充 profile 级 README。
- `font-feature` 当前关闭了常见连字特性，适合偏传统的代码显示习惯。
