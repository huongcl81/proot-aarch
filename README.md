# proot-aarch

For arm
```bash
git clone https://github.com/huongcl81/proot-aarch.git
cd proot-aarch
chmod +x proot-v5.3.0-aarch64-static
mkdir -p ubuntu-rootfs
tar -xzf bionic-base-arm64.tar.gz -C ubuntu-rootfs
./proot-v5.3.0-aarch64-static -S ubuntu-rootfs /bin/bash

for x86_x64
```bash
git clone https://github.com/huongcl81/proot-aarch.git
cd proot-aarch
chmod +x proot-v5.3.0-x86_64-static
mkdir -p ubuntu-rootfs
wget https://cdimage.ubuntu.com/ubuntu-base/bionic/daily/20250618/bionic-base-amd64.tar.gz
tar -xzf bionic-base-amd64.tar.gz -C ubuntu-rootfs
./proot-v5.3.0-x86_64-static -S ubuntu-rootfs /bin/bash
