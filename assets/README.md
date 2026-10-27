| 属性 | 值 |
|---|---|
| 文档名称 | assets 目录说明 |
| 版本 | v1.0 |
| 日期 | 2026-11-10 |
| 作者 | 项目负责人 |
| 状态 | 已定稿 |

# assets 目录说明

本项目级静态资源目录，存放**不随小程序包发布**的视觉与演示素材。

## 目录结构

| 子目录 | 内容 | 使用者 |
|---|---|---|
| `logo/` | 项目 Logo，各尺寸、各背景色版本 | README / 答辩 PPT / 软著 |
| `illustrations/` | 空状态插画、引导页插画、情感化配图 | 设计稿 / 小程序（导出后复制到 miniprogram/assets） |
| `diagrams/` | 架构图、流程图、ER 图（含 draw.io 源文件） | 技术文档 / 答辩 |
| `screenshots/` | 各版本演示截图，按版本分子目录 | 结题报告 / 用户手册 / 演示 |
| `docs-assets/` | 知识库文档内嵌配图 | 飞书文档 |

## 命名规范


[模块]-[描述]-[版本].[格式]

示例：
```plaintext
  step-empty-v1.png          # 步数模块空状态插画 v1
  architecture-v2.png       # 架构图 v2
  db-er-v1.drawio           # ER 图源文件
  ui-home-v0.5.png          # 首页设计稿 v0.5
```


## 规则

1. 原始源文件（.drawio / .fig / .sketch）与导出图（.png / .pdf）同目录存放
2. 单张图片不超过 2MB，超大会压缩或降分辨率
3. 图片内文字不小于 12px
4. 所有图片在文档中引用时必须加说明文字
5. 不得将他人版权素材放入本目录（插画需标注来源或确认为可商用）
6. `diagrams/` 改动后，同步更新对应技术文档中的配图

## 与 miniprogram/assets 的区别

- 本目录 `assets/`：给人看的素材，不进小程序包
- `miniprogram/assets/`：给用户看的素材，随包发布，引用路径 `/assets/xxx.png`
