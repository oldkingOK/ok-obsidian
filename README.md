# Ok Obsidian Vault Template

oldkingOK 的Obsidian仓库模板，包含了一些插件和仓库设置，避免每次创建仓库繁琐的重复操作

## 设置

1. Setting - File & Links - Detect all file extensions
2. Community Plugins Enable
3. mkdocs.yml 的 `markdown_extensions` 取消 `attr_list` 的注释——以支持python-markdown语法
4. 设置博客模板——创建文件后点击左侧 `Insert template` 即可插入博客头

## 使用的插件

| 名称                                                                                                        | 用途    | 开源协议     | 备注                              |
| --------------------------------------------------------------------------------------------------------- | ----- | -------- | ------------------------------- |
| [obsidian-omnisearch](https://github.com/scambier/obsidian-omnisearch)                                    | 高级搜索  | GPL-3.0  |                                 |
| [advanced-tables-obsidian](https://github.com/tgrosinger/advanced-tables-obsidian)                        | 编辑表格  | GPL-3.0  |                                 |
| [obsidian-custom-attachment-location](https://github.com/RainCat1998/obsidian-custom-attachment-location) | 管理附件  | 无        |                                 |
| [denolehov/obsidian-git](https://github.com/denolehov/obsidian-git)                                       | 版本管理  | MIT      |                                 |
| [sunxvming/obsidian-vscode-editor](https://github.com/sunxvming/obsidian-vscode-editor)                   | 代码编辑  | MIT      | 设置里添加了yml                       |
| [NomarCub/obsidian-open-vscode](https://github.com/NomarCub/obsidian-open-vscode)                         | 打开vsc | MIT      |                                 |
| [polyipseity/obsidian-terminal](https://github.com/polyipseity/obsidian-terminal)                         | 打开终端  | AGPL-3.0 | 比如mkdocs serve                  |
| [mugiwara85/CodeblockCustomizer](https://github.com/mugiwara85/CodeblockCustomizer)                       | 代码块优化 | MIT      | 设置：代码块->启用渐变折叠；头语言->总是显示代码头（折叠） |

## 部署

### 在 github 上

等待 Github Action 构建成功之后，

Settings - Pages - Build and deployment

- Source - Deploy from a branch
- 选择 `gh-pages` 分支

### 在本地

```shell
python -m venv .venv
.\.venv\Scripts\activate # Windows
source .venv/Scripts/activate # Unix
mkdocs serve
```