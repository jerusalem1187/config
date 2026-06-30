# 本机配置文档

> 主机名：**GUOXIONG**  
> 文档生成日期：2026-06-30  
> GitHub 账号：jerusalem1187

---

## 1. 硬件概览

| 项目 | 配置 |
|------|------|
| 品牌型号 | ASUS Adol 14 M5451GADOL |
| 主板 | ASUSTeK M5451GA v1.0 |
| CPU | AMD Ryzen AI 9 H 465 w/ Radeon 880M（10 核 / 20 线程，基准 2.0 GHz，L2 10 MB / L3 24 MB） |
| 内存 | 32 GB（4 × 8 GB Samsung DDR5-8533，K3KL9L90DM-MGCU） |
| 核显 | AMD Radeon 880M Graphics（512 MB 共享显存，驱动 32.0.22042.17002） |
| 虚拟显示 | GameViewer Virtual Display Adapter |
| 系统盘 | Kioxia KBG60ZNV1T02 1 TB NVMe |
| 显示器 | MyASUS Splendid，2880 × 1800 @ 120 Hz |
| 电池 | ASUS Battery（当前约 95%） |
| BIOS | American Megatrends M5451GA.311（2026-04-17） |

---

## 2. 操作系统

| 项目 | 值 |
|------|-----|
| 系统 | Microsoft Windows 11 家庭中文版 |
| 版本 | 10.0.26200（Build 26200，25H2） |
| 架构 | 64-bit (x64) |
| 时区 | (UTC+08:00) 北京，重庆，香港，乌鲁木齐 |
| 系统安装日期 | 2026-03-31 |
| 最近启动 | 2026-06-10 13:03:48 |
| 虚拟化 | Hyper-V 已检测到；基于虚拟化的安全功能已启用 |
| 页面文件 | C:\pagefile.sys |

### 磁盘分区

| 盘符 | 卷标 | 总容量 | 可用空间 | 文件系统 |
|------|------|--------|----------|----------|
| C: | OS | 383.55 GB | 269.80 GB | NTFS |
| D: | 新加卷 | 283.20 GB | 121.80 GB | NTFS |
| E: | 新加卷 | 285.28 GB | 160.17 GB | NTFS |
| — | MYASUS | 256 MB | — | FAT32（华硕恢复分区） |
| — | RECOVERY | ~1.1 GB | — | NTFS |

---

## 3. 网络

| 适配器 | 状态 | 说明 |
|--------|------|------|
| Realtek RTL8852BE WiFi 6 802.11ax | 已连接 | WLAN，DHCP 192.168.21.1，IP 192.168.21.8 |
| Bluetooth PAN | 已断开 | 蓝牙网络 |

---

## 4. 开发工具链

### 版本信息

| 工具 | 版本 |
|------|------|
| Git | 2.54.0.windows.1 |
| GitHub CLI (gh) | 2.95.0 |
| Python | 3.13.8（VeighNa Studio 内置） |
| pip | 26.1.2 |
| Cursor | 3.9.16 |
| PowerShell | 5.1（Desktop） |

### 未安装 / 未配置

- Node.js、npm 未安装
- Docker Desktop 未安装
- WSL 未安装
- VS Code 未安装
- Java、Go、Rust、.NET SDK 未在 PATH 中检测到
- Conda 未安装

---

## 5. Git 全局配置

```ini
credential.https://github.com.helper=!gh auth git-credential
credential.https://gist.github.com.helper=!gh auth git-credential
```

- 远程协议：HTTPS
- GitHub 账号：jerusalem1187（已登录 gh CLI）
- 注：本机未设置 `user.name` / `user.email`，提交前需按需配置

---

## 6. Cursor 编辑器配置

配置文件路径：`%APPDATA%\Cursor\User\settings.json`

```json
{
    "window.autoDetectColorScheme": false
}
```

---

## 7. 环境变量（PATH 摘要）

### 系统级 PATH 主要条目

- VeighNa Studio（`C:\veighna_studio\`、`C:\veighna_studio\Scripts`）
- Git（`C:\Program Files\Git\cmd`）
- GitHub CLI（`C:\Program Files\GitHub CLI\`）

### 用户级 PATH 主要条目

- Cursor（`%LOCALAPPDATA%\Programs\cursor\resources\app\bin`）
- cursor-agent（`%LOCALAPPDATA%\cursor-agent`）
- Windows Apps

---

## 8. 主要软件 / 工具生态

| 类别 | 软件 |
|------|------|
| IDE / 编辑器 | Cursor |
| 量化 / 金融 | VeighNa Studio（Python 3.13 环境） |
| AI / Agent | cursor-agent |
| 版本管理 | Git、GitHub CLI |

---

## 9. Python 环境（pip 部分包）

本地 Python 3.13（VeighNa Studio）已安装常用数据与量化相关包，例如：

- aiohttp / aiohappyeyeballs
- alphalens-reloaded
- anthropic
- auto-researcher（本地可编辑项目：`Desktop\机器学习\auto_researcher`）
- beautifulsoup4

> 完整包列表可通过 `pip list` 查看。

---

## 10. 目录结构习惯

| 路径 | 用途 |
|------|------|
| `C:\Users\GuoX\Desktop` | 桌面 / 工作区 |
| `C:\veighna_studio\` | VeighNa 量化 Python 环境 |
| `D:\`、`E:\` | 数据盘 |

---

## 11. 备注

- 本仓库用于记录个人开发机配置，便于换机或环境重建时参考。
- 同仓库另有 `rog.md`，记录另一台 ASUS ROG 台式机配置。
- 请勿在此仓库中提交密钥、Token、密码等敏感信息。
- 配置变更后建议更新本文档并 push。
