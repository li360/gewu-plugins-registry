# GeWu 社区插件注册表

本仓库为 [GeWu（格物）](https://github.com/li360/gewu-project) 桌面应用提供社区插件注册表 `registry.json`。

GeWu 客户端在「插件管理 → 社区」中读取本仓库 main 分支根目录的 `registry.json`（直连失败时自动尝试镜像）。

## registry.json 格式

JSON 数组，每项一个插件：

| 字段 | 类型 | 必填 | 说明 |
|------|------|------|------|
| `id` | string | 是 | 插件 ID，须与插件包 `manifest.json` 的 id 一致（`plugin-` 前缀） |
| `name` | string | 是 | 显示名称 |
| `version` | string | 是 | 当前发布的语义化版本号 |
| `downloadUrl` | string | 是 | `gewu-plugin.zip` 下载地址（推荐 GitHub Release latest 直链） |
| `description` | string | 否 | 插件描述 |
| `author` | string | 否 | 作者 |
| `repository` | string | 否 | 源码仓库地址 |
| `homepage` | string | 否 | 首页/文档地址 |
| `icon` | string | 否 | emoji 图标 |
| `checksum` | string | 否 | SHA256（`sha256:` 前缀或纯 hex） |

## 收录新插件

向本仓库提交 PR，在 `registry.json` 数组中追加一项即可。插件自身仍需托管在可公开下载的位置（推荐按 GitHub Release 约定发布 `gewu-plugin.zip` 与 `update.json`）。
