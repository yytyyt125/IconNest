# IconNest

绿色免安装的 Windows 桌面图标整理工具。将桌面图标按分类拖入独立的悬浮窗口，保持桌面清爽；退出时可选择是否把图标移回桌面并还原布局。

## 下载

前往 [Releases](https://github.com/yytyyt125/IconNest/releases) 下载最新版 `IconNest.exe`（单文件，无需安装，直接运行）。

当前版本：**v0.2.12**

## 使用

1. 双击 `IconNest.exe` 直接运行，无需安装。
2. 在托盘图标上右键，可新建分类窗口、打开设置。
3. 将桌面图标拖入分类窗口进行分类收纳。

## 分类文件存储位置

- **默认位置**：桌面所在盘根目录下的 `IconNest 分类文件`（例如桌面在 `C:\Users\...\Desktop`，则默认目录为 `C:\IconNest 分类文件`）。该目录按当前用户自动计算，不会落到他人机器上。
- **更改位置**：托盘右键 → 设置 → 「分类文件存储位置」→ 更改… ，选择新文件夹后，程序会自动把现有分类文件夹整体迁移过去（跨盘为复制+删除，失败自动回滚），并立即生效。
- **手动指定**：编辑 `IconNest.exe` 同级目录下的 `config\config.json`，将 `settings.storageRoot` 设为目标绝对路径，重启生效。

## 绿色性说明

- 配置保存在 `IconNest.exe` 同级的 `config\` 目录，不写入注册表或 `%APPDATA%`。
- 建议将 `IconNest.exe` 放在有写入权限的普通目录（如 `D:\Tools\`）；若放入 `C:\Program Files` 等受保护目录，配置写入可能失败。
