# os-assignment1 readme file



# Getting the latest version of Linux Kernel source code.

$ wget https://cdn.kernel.org/pub/linux/kernel/v5.x/linux-5.19.7.tar.xz


# Extract the tar.xz file that we downloaded.

$ tar -xf linux-5.19.7.tar.xz


# Switch to linux directory.

$ cd linux-5.19.7


# Configuring the features and modules of linux kernel.

$ cp /boot/config-$(uname -r) .config


# Install the required compilers and tools.

$ sudo apt-get install build-essential libncurses-dev bison flex libssl-dev libelf-dev


# Configuring the kernel.

$ make menuconfig


# Compiling the kernel.

$ make -j 4


# Installing kernel modules

$ sudo make modules_install


# Install the compiled kernel

$ sudo make install


# Showing the latest kernel installed.

$ uname -r

