# 弱链接 发布仓库

本仓库只存放 **弱链接** 的构建产物与更新清单，不含源码。

源码仓库：[endtower/N_touch](https://github.com/endtower/N_touch)

## 用户怎么装

下载本仓库最新 Release 里的 `AbyssLauncher.exe`，双击运行即可。
首次运行会释放到 `%LOCALAPPDATA%\Abyss\app`，之后按界面提示逐个安装组件。

## 更新源

程序里的「更新中心」读取本仓库最新 Release 的清单：

- `core-latest.json` → Core 组件
- `manager-latest.json` → 管理服务
- `launcher-latest.json` → 启动器自身

## 维护者

发布由源码仓库的 GitHub Actions 自动完成，推 `v*` 标签触发。
需要配置 `RELEASE_TOKEN` 秘钥（对本仓库有 contents:write 权限）。
