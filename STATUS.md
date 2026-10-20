# STATUS — gewu-plugins-registry（社区插件注册表）

> 更新：2026-10-18 · 维护人：li360

<!-- resume:start -->
现在: 稳定维护；`registry.json` 通过 PR 更新，客户端读取 main 分支。
下一步:
- 收录新插件（按 README 的校验脚本跑一遍）
- 定期检查失效的 downloadUrl 与过期 version
阻塞: 无
<!-- resume:end -->

## 最近完成

- 2026-10-18 补本地校验脚本、测试清单与发布说明（`5d12b7d`）

## 发布状态

- 无构建产物；`main` 分支即线上数据
- 客户端：直连 `raw.githubusercontent.com/li360/gewu-plugins-registry/main/registry.json`，失败时镜像

## 入口

- 格式与校验：[README.md](README.md)
- 主仓库台账：[../MyProj/docs/status/todo.md](../MyProj/docs/status/todo.md)
