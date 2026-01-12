# Linux 基础入门 - 第一天（2026-01-13）

> 📌 学习目标：搭建 Ubuntu 虚拟机环境，掌握常用 Linux 命令，理解文件系统与权限机制。

## ✅ 今日完成

- 在 VMware Workstation 中安装 **Ubuntu 22.04 LTS**
- 熟悉终端基本操作
- 练习核心命令：`ls`, `cd`, `pwd`, `mkdir`, `touch`, `cp`, `mv`, `rm`
- 初步了解用户权限与 `sudo` 机制

---

## 💻 实操记录

### 1. 虚拟机配置
| 项目 | 配置 |
|------|------|
| 虚拟化软件 | VMware Workstation 17 |
| 操作系统 | Ubuntu 22.04.3 LTS (Desktop) |
| 内存 | 2 GB |
| 硬盘 | 20 GB（单文件）|
| 网络模式 | 桥接（Bridge）——可访问外网 |

> 安装过程顺利，设置用户名为 `xiongye`，主机名 `ops-vm`。

---

### 2. 常用命令练习

```bash
# 查看当前路径
pwd

# 列出目录内容（详细格式）
ls -l

# 进入家目录
cd ～

# 创建项目文件夹
mkdir -p ～/projects/linux-practice

# 创建测试文件
touch ～/projects/linux-practice/hello.txt

# 复制文件
cp hello.txt backup.txt

# 重命名文件
mv backup.txt old-hello.txt

# 删除文件
rm old-hello.txt

# 查看文件内容（空文件）
cat hello.txt