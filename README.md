# 启元 Linux · aarch64 包仓库

启元 Linux（Quor-a/qiyuan-linux）的 **aarch64（ARM64）交叉编译二进制包**发布仓库。
配方与源码在主仓库：https://github.com/Quor-a/qiyuan-linux

## 下载

所有包以 GitHub Release 附件发布（tag=latest 滚动更新），单个包永久直链：

```sh
BASE=https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download
curl -LO $BASE/busybox-1.36.1-1.aarch64.qyp
```

## 安装到安卓 / aarch64 设备

qyp 包用 qypkg（启元包管理器）安装。设备上没有 qypkg 时，先建本地仓库目录再装：

```sh
mkdir -p ~/qyrepo/aarch64 && cd ~/qyrepo/aarch64
curl -LO https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/index.json
# 下载需要的 .qyp 到同一目录，然后：
qypkg --root ~/qyroot --repo ~/qyrepo --allow-unsigned install busybox
```

## 校验

index.json 里每个包都有 sha256：

```sh
sha256sum busybox-1.36.1-1.aarch64.qyp   # 与 index.json 对照
```

## 包清单

见 PACKAGES.txt（文件名 / 版本 / 大小 / 描述 / 依赖），与 Release 附件同步。

## 全部包（31）

| 包名 | 版本 | 说明 | 下载 |
|---|---|---|---|
| `bash` | 5.3-1 | GNU Bourne-Again Shell（系统默认 shell） | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/bash-5.3-1.aarch64.qyp) |
| `busybox` | 1.36.1-1 | 静态多合一 Unix 工具箱 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/busybox-1.36.1-1.aarch64.qyp) |
| `ca-certificates` | 20250415-1 | 系统可信 CA 证书集 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/ca-certificates-20250415-1.aarch64.qyp) |
| `diffutils` | 3.11-1 | 文件比较工具（diff cmp） | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/diffutils-3.11-1.aarch64.qyp) |
| `expat` | 2.7.0-1 | 流式 XML 解析库 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/expat-2.7.0-1.aarch64.qyp) |
| `file` | 5.46-1 | 按内容识别文件类型 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/file-5.46-1.aarch64.qyp) |
| `findutils` | 4.10.0-1 | 文件搜索工具（find xargs locate） | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/findutils-4.10.0-1.aarch64.qyp) |
| `gawk` | 5.3.1-1 | GNU awk 文本处理语言 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/gawk-5.3.1-1.aarch64.qyp) |
| `gmp` | 6.3.0-1 | 任意精度算术库 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/gmp-6.3.0-1.aarch64.qyp) |
| `grep` | 3.11-1 | 模式匹配与文本搜索 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/grep-3.11-1.aarch64.qyp) |
| `gzip` | 1.13-1 | GNU 压缩工具 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/gzip-1.13-1.aarch64.qyp) |
| `less` | 668-1 | 文本文件分页查看器 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/less-668-1.aarch64.qyp) |
| `libffi` | 3.4.7-1 | 外部函数接口库（解释器与 JIT 依赖） | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/libffi-3.4.7-1.aarch64.qyp) |
| `libqydemo` | 0.2.0-1 | 启元构建系统演示共享库 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/libqydemo-0.2.0-1.aarch64.qyp) |
| `linux-headers` | 6.16.1-1 | Linux 内核用户空间头文件 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/linux-headers-6.16.1-1.aarch64.qyp) |
| `make` | 4.4.1-1 | GNU make 构建工具 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/make-4.4.1-1.aarch64.qyp) |
| `mpfr` | 4.2.2-1 | 多精度浮点运算库（gcc/gawk 依赖） | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/mpfr-4.2.2-1.aarch64.qyp) |
| `ncurses` | 6.5-1 | 终端处理库（供 bash、less、vi 等使用） | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/ncurses-6.5-1.aarch64.qyp) |
| `patch` | 2.8-1 | 应用 diff 补丁 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/patch-2.8-1.aarch64.qyp) |
| `pcre2` | 10.45-1 | Perl 兼容正则表达式库 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/pcre2-10.45-1.aarch64.qyp) |
| `pkgconf` | 2.4.0-1 | 编译期依赖查询工具（pkg-config 的替代实现） | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/pkgconf-2.4.0-1.aarch64.qyp) |
| `procps-ng` | 4.0.5-1 | 进程与系统状态工具（ps top kill） | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/procps-ng-4.0.5-1.aarch64.qyp) |
| `readline` | 8.3-1 | 命令行行编辑与历史库 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/readline-8.3-1.aarch64.qyp) |
| `sed` | 4.9-1 | 非交互式流编辑器 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/sed-4.9-1.aarch64.qyp) |
| `sqlite` | 3.49.2-1 | 嵌入式关系型数据库引擎 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/sqlite-3.49.2-1.aarch64.qyp) |
| `tar` | 1.35-1 | 归档工具 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/tar-1.35-1.aarch64.qyp) |
| `util-linux` | 2.41-1 | 系统杂项工具（mount lsblk fdisk 等） | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/util-linux-2.41-1.aarch64.qyp) |
| `which` | 2.23-1 | 定位可执行文件位置 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/which-2.23-1.aarch64.qyp) |
| `xz` | 5.8.1-1 | XZ / LZMA 压缩工具与库 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/xz-5.8.1-1.aarch64.qyp) |
| `zlib` | 1.3.1-1 | 通用无损数据压缩库 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/zlib-1.3.1-1.aarch64.qyp) |
| `zstd` | 1.5.7-1 | Zstandard 实时压缩算法与库 | [下载](https://github.com/Quor-a/qiyuan-linux-aarch64/releases/latest/download/zstd-1.5.7-1.aarch64.qyp) |
