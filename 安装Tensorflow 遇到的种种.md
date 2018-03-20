# 安装Tensorflow 遇到的种种

标签（空格分隔）： 未分类

---

遇见的问题1：
Installing the NVIDIA display driver...
The driver installation is unable to locate the kernel source. Please make sure that the kernel source packages are installed and set up correctly.
If you know that the kernel source packages are installed and set up correctly, you may pass the location of the kernel source with the '--kernel-source-path' flag.

对应的解决方法1：

$uname -r
4.4.0-109-generic

sudo apt-get purge linux-image-4.4.0-109-generic
sudo apt-get purge linux-headers-4.4.0-109-generic
sudo update-initramfs -u

参考链接为:https://devtalk.nvidia.com/default/topic/1028566/cuda-setup-and-installation/cuda-9-1-install-fail-with-ubuntu-16-04-kernel-version-4-13-0-26/


