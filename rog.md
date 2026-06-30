# 本机配置文档

> 主机名：**GUO**  
> 文档生成日期：2026-06-30  
> GitHub 账号：jerusalem1187

---

## 1. 硬件概览

| 项目 | 配置 |
|------|------|
| 品牌型号 | ASUS ROG STRIX G15CF_G15CF |
| 主板 | ASUSTeK G15CF v1.0 |
| CPU | 12th Gen Intel Core i7-12700（12 核 / 20 线程，基准 2.1 GHz） |
| 内存 | 16 GB（2 × 8 GB SK Hynix DDR4-3200，HMA81GU6DJR8N-XN） |
| 独立显卡 | NVIDIA GeForce RTX 3060 Ti（4 GB 显存，驱动 32.0.15.8195） |
| 虚拟显示 | GameViewer Virtual Display Adapter |
| 系统盘 | Micron 3400 MTFDKBA1T0TFH 1 TB NVMe（C:） |
| 数据盘 | TOSHIBA DT01ACA100 1 TB HDD（D:） |
| 其他分区 | Z: Trading（387 GB） |
| 显示器 | Generic PnP Monitor，2560 × 1440 |
| BIOS | American Megatrends Inc. G15CF.301（2022-01-24） |

---

## 2. 操作系统

| 项目 | 值 |
|------|-----|
| 系统 | Microsoft Windows 11 家庭中文版 |
| 版本 | 10.0.26200（Build 26200，25H2） |
| 架构 | 64-bit (x64) |
| 时区 | (UTC+08:00) 北京，重庆，香港，乌鲁木齐 |
| 系统安装日期 | 2025-06-11 |
| 最近启动 | 2026-06-24 09:59:40 |
| 虚拟化 | Hyper-V 已检测到；基于虚拟化的安全功能已启用 |
| 页面文件 | D:\pagefile.sys |

### 磁盘分区

| 盘符 | 卷标 | 总容量 | 可用空间 | 文件系统 |
|------|------|--------|----------|----------|
| C: | OS | 542.37 GB | 209.02 GB | NTFS |
| D: | DATA | 931.51 GB | 310.65 GB | NTFS |
| Z: | Trading | 387.30 GB | 58.65 GB | NTFS |

---

## 3. 网络

| 适配器 | 状态 | 说明 |
|--------|------|------|
| MediaTek Wi-Fi 6 MT7921 | 已连接 | WLAN，DHCP 192.168.1.1，IP 192.168.1.170 |
| Realtek Gaming 2.5GbE | 已断开 | 有线网卡 |
| Wintun Userspace Tunnel (Meta) | 活动 | 198.18.0.1 |
| TAP-Windows Adapter V9 (LetsTAP) | 已断开 | VPN 适配器 |
| Bluetooth PAN | 已断开 | 蓝牙网络 |

---

## 4. 开发工具链

### 版本信息

| 工具 | 版本 |
|------|------|
| Git | 2.49.0.windows.1 |
| GitHub CLI (gh) | 2.93.0 |
| Node.js | v22.17.1 |
| npm | 10.9.2 |
| Python | 3.13.5 |
| pip | 25.1.1 |
| Conda | 24.9.1 |
| Docker Desktop | 28.1.1 |
| WSL | 2.7.3.0（内核 6.6.114.1-1） |
| VS Code | 1.67.2 |
| Cursor | 3.9.16 |
| PowerShell | 5.1.26100.8655 (Desktop) |

### WSL 发行版

| 名称 | 状态 | WSL 版本 |
|------|------|----------|
| docker-desktop | Stopped | 2 |
| Ubuntu | Stopped | 2 |

### 未安装 / 未配置

- Java、Go、Rust 未在 PATH 中检测到
- .NET SDK 未安装（运行时目录存在但无 SDK）

---

## 5. Git 全局配置

```ini
user.name=jerusalem1187
user.email=georgeguo96@gmail.com
core.editor="C:\Users\86139\AppData\Local\Programs\Microsoft VS Code\bin\code" --wait
filter.lfs.required=true
```

- 远程协议：HTTPS
- GitHub 账号：jerusalem1187（已登录 gh CLI）

---

## 6. Cursor / VS Code 编辑器配置

配置文件路径：`%APPDATA%\Cursor\User\settings.json`

```json
{
    "python.defaultInterpreterPath": "d:\\ProgramData\\Anaconda3\\python.exe",
    "diffEditor.maxComputationTime": 0,
    "window.customTitleBarVisibility": "windowed",
    "zenMode.fullScreen": false,
    "claudeCode.preferredLocation": "sidebar",
    "cursor.composer.usageSummaryDisplay": "always",
    "python.createEnvironment.trigger": "off",
    "window.restoreWindows": "preserve",
    "window.autoDetectColorScheme": false,
    "editor.accessibilitySupport": "off"
}
```

---

## 7. 环境变量（PATH 摘要）

### 系统级 PATH 主要条目

- Python 3.13（`C:\Python313\`）
- Git（`z:\Program Files\Git\cmd`）
- VeighNa Studio 4（量化框架）
- Docker Desktop
- Node.js
- Chocolatey
- GitHub CLI
- WireGuard
- 东方财富 Choice Excel 插件

### 用户级 PATH 主要条目

- Hermes Agent / Hermes CLI
- VS Code / Cursor
- Anaconda3 Scripts
- Wind 金融终端（WindNET）
- GitHub Desktop
- npm 全局包
- MiKTeX（LaTeX）
- cursor-agent

---

## 8. 主要软件 / 工具生态

| 类别 | 软件 |
|------|------|
| IDE / 编辑器 | Cursor、VS Code |
| 量化 / 金融 | VeighNa Studio 4、Wind 金融终端、东方财富 Choice |
| 容器 / 虚拟化 | Docker Desktop、WSL2、Hyper-V |
| 网络 | WireGuard、Meta VPN (Wintun) |
| 文档 / 排版 | MiKTeX |
| AI / Agent | Hermes Agent、cursor-agent |
| 版本管理 | Git、GitHub Desktop、Git LFS |

---

## 9. Python 环境（pip 部分包）

本地 Python 3.13 已安装常用数据与量化相关包，例如：

- akshare（金融数据）
- aiohttp / aiohappyeyeballs
- alpha101（本地可编辑项目：`Trading2025\Factor\Alpha101`）
- alembic

> 完整包列表可通过 `pip list` 查看。

---

## 10. 目录结构习惯

| 路径 | 用途 |
|------|------|
| `C:\Users\86139\Desktop` | 桌面 / 工作区 |
| `C:\Users\86139\OneDrive` | OneDrive 同步 |
| `D:\` | 数据盘、页面文件 |
| `Z:\` | Trading 专用分区 |
| `d:\ProgramData\Anaconda3\` | Conda / Python 主环境 |
| `C:\veighna_studio4\` | VeighNa 量化环境 |

---

## 11. 备注

- 本仓库用于记录个人开发机配置，便于换机或环境重建时参考。
- 请勿在此仓库中提交密钥、Token、密码等敏感信息。
- 配置变更后建议更新本文档并 push。
