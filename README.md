# proot-aarch

git clone https://github.com/huongcl81/proot-aarch.git
cd proot-aarch
chmod +x proot-v5.3.0-aarch64-static
mkdir -p ubuntu-rootfs
tar -xzf bionic-base-arm64.tar.gz -C ubuntu-rootfs
./proot-v5.3.0-aarch64-static -S ubuntu-rootfs /bin/bash
