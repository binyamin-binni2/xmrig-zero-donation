# 🌌✨ XMRig Zero Donation Binaries ✨🌌

<p align="center">
  <img src="https://img.shields.io/github/release/binyamin-binni2/xmrig-zero-donation.svg?style=for-the-badge&color=brightgreen&label=Latest%20Build" />
  <img src="https://img.shields.io/badge/Donations-0%25-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/OS-Linux%20%7C%20Windows%20%7C%20Android-informational?style=for-the-badge&logo=linux" />
</p>

---

## 💎 About

This repository provides manually compiled and optimized binaries of [XMRig](https://github.com/xmrig/xmrig) for:

- ✅ Linux (x86_64)
- ✅ Windows (x86_64)
- ✅ Android (aarch64 - Termux)

All binaries are built with:

- 🧠 **Zero Dev Fee** (`--donate-level=0`)
- ⚡ Optimized performance flags
- 🔐 TLS support included
- 🧱 Static or dynamic linking as per platform

---

## 📦 Available Downloads

| Platform | File | HWLOC | TLS | Notes |
|----------|------|--------|-----|-------|
| 🐧 Linux | `xmrig-linux.tar.gz` | ✅ Yes | ✅ | Built with system `hwloc` and `libuv` |
| 🪟 Windows | `xmrig-windows.zip` | ❌ No | ✅ | Static libuv included |
| 🤖 Android (Termux) | `xmrig-android.tar.gz` | ❌ No | ✅ | libuv prebuilt from Termux repo |

Visit the **[Releases](https://github.com/binyamin-binni2/xmrig-zero-donation/releases)** tab to download the latest binaries.

---

## 🧪 How to Use

### Linux

```bash
tar -xzf xmrig-linux.tar.gz
cd xmrig
./xmrig -a rx -o pool.supportxmr.com:443 -u YOUR_WALLET_ADDRESS -k --tls
```

### Windows

```powershell
xmrig.exe -a rx -o pool.supportxmr.com:443 -u YOUR_WALLET_ADDRESS -k --tls
```

### Android (Termux)

```bash
pkg update && pkg install tar
tar -xzf xmrig-android.tar.gz
cd xmrig
./xmrig -a rx -o pool.supportxmr.com:443 -u YOUR_WALLET_ADDRESS -k --tls
```

---

## 🧱 Build Notes

These binaries were built **manually**, not using the official repo fork. That means:

- You get updated versions directly by modifying the `git clone` step before build.
- No accidental donation patch leaks.
- Source code edits stay private (not in a public fork).
- Android `libuv` was downloaded from:
  [libuv_1.51.0_aarch64.deb](https://packages.termux.dev/apt/termux-main/pool/main/libu/libuv/libuv_1.51.0_aarch64.deb)

---

## 🌟 Credits

- 🔧 [XMRig](https://github.com/xmrig/xmrig)
- 🧩 [libuv](https://github.com/libuv/libuv)
- 📦 [Termux Packages](https://github.com/termux/termux-packages)
- ❤️ Maintained by [@binyamin-binni2](https://github.com/binyamin-binni2)

---

## 💬 License

XMRig is open-source software under the [GPLv3 License](https://github.com/xmrig/xmrig/blob/master/LICENSE).  
This repository provides **binaries only** — no modifications to original logic.

> ✅ Built with ❤️. Enjoy mining 100% for yourself.
