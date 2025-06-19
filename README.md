
# 🐧 proot-aarch

> Chạy Ubuntu Bionic (18.04) user-space trên ARM64 hoặc x86_64 với PRoot, không cần root.

---

## 📦 Features

- Không cần root (dùng được Termux, WSL, VPS...)
- Ubuntu base nhẹ, chuẩn Bionic
- Hỗ trợ ARM64 và x86_64
- PRoot v5.3.0 static sẵn
- Dễ cài, dễ dùng

---

## 🚀 Quick Setup Guide

### 1. Setup cho ARM64 (`aarch64`)
```bash
git clone https://github.com/huongcl81/proot-aarch.git
cd proot-aarch

chmod +x proot-v5.3.0-aarch64-static
mkdir -p ubuntu-rootfs
tar -xzf bionic-base-arm64.tar.gz -C ubuntu-rootfs

# Vào Ubuntu
./proot-v5.3.0-aarch64-static -S ubuntu-rootfs /bin/bash

### 2. Setup cho x86_64
```bash
git clone https://github.com/huongcl81/proot-aarch.git
cd proot-aarch

chmod +x proot-v5.3.0-x86_64-static
mkdir -p ubuntu-rootfs
wget https://cdimage.ubuntu.com/ubuntu-base/bionic/daily/20250618/bionic-base-amd64.tar.gz
tar -xzf bionic-base-amd64.tar.gz -C ubuntu-rootfs

# Vào Ubuntu
./proot-v5.3.0-x86_64-static -S ubuntu-rootfs /bin/bash
