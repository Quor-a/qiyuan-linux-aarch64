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
