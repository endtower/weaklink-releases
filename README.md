# 弱链接 发布仓库

**用户下载入口。** 只存放构建产物与更新清单，不含源码。

## 下载

在 [Releases](../../releases/latest) 里下载 `AbyssLauncher.exe`，双击运行即可。

首次运行会释放到 `%LOCALAPPDATA%\Abyss\app`，之后按界面提示逐个安装组件。
Windows 若提示「已保护你的电脑」，点「更多信息」→「仍要运行」。

## 源码

源码在 **[endtower/N_touch](https://github.com/endtower/N_touch)**（目录 `dev/`）。

## 更新源

程序里的「更新中心」读取本仓库最新 Release 的清单：

| 文件 | 对应组件 |
|---|---|
| `core-latest.json` | Core（大脑、记忆、QQ 接入） |
| `manager-latest.json` | 管理服务 |
| `launcher-latest.json` | 启动器自身 |

各组件有独立版本号，可以分别更新，互不牵动。

## 维护者

发布由源码仓库的 GitHub Actions 自动完成，推 `v*` 标签触发。
需要 `RELEASE_TOKEN` 秘钥（对本仓库有 contents:write 权限）。