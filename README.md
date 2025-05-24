# 潇然系统网络启动

[![GitHub last commit](https://img.shields.io/github/last-commit/xrgzs/xrsys-ipxe?label=%E4%B8%8A%E6%AC%A1%E6%8F%90%E4%BA%A4)](https://github.com/xrgzs/xrsys-ipxe/commits)
[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/xrgzs/xrsys-ipxe/build.yml?label=CI%E6%9E%84%E5%BB%BA)](https://github.com/xrgzs/xrsys-ipxe/actions)

（🛠️WIP）潇然系统网络启动（XRSYS-iPXE，XRPXE）通过网络引导系统，实现在线安装系统🌟🚀

🫡由 [iPXE](https://ipxe.org/) 强力驱动。

## 编译

```shell
sudo apt install gcc binutils make perl mtools mkisofs syslinux liblzma-dev isolinux
git clone https://github.com/xrgzs/xrsys-ipxe.git
cd xrsys-ipxe
make -j 4 -C src everything
```

## 启动

```shell
#!ipxe
dhcp
chain http://url.xrgzs.lmxiao.top/ipxe
```

## 参考

<https://itexp.blog.csdn.net/article/details/131125851>

<https://www.egg0.com/show/19831.html>
