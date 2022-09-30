# os-assignment1 readme file



# Getting the latest version of Linux Kernel source code from kernel.org.

$ wget https://cdn.kernel.org/pub/linux/kernel/v5.x/linux-5.19.7.tar.xz


# Extracting the tar file that we downloaded.

$ tar -xf linux-5.19.7.tar.xz


# Switching to linux (that we installed) directory.

$ cd linux-5.19.7


# Configuring the features  of linux kernel.

$ cp /boot/config-$(uname -r) .config


# Installing the required dependencies.

$ sudo apt-get install build-essential libncurses-dev bison flex libssl-dev libelf-dev


# Configuring the kernel.

$ make menuconfig


# Compiling the kernel.

$ make -j 4


# Installing the kernel modules

$ sudo make modules_install


# Installing the compiled kernel

$ sudo make install


# Showing the latest kernel that we installed.

$ uname -r

