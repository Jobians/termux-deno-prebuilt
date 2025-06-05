# termux-deno-prebuilt

**Prebuilt Deno packages for Termux (Android)**

This repository hosts prebuilt `.deb` packages of [Deno](https://deno.land/) for Termux on Android devices.
Use these packages to easily install or upgrade Deno without building from source.

> 🛠 These packages are built from the [`enable-deno` branch](https://github.com/0komo/termux-packages/tree/refs/heads/enable-deno) of [`0komo/termux-packages`](https://github.com/0komo/termux-packages), which adds support for Deno in Termux.

---

## 📦 Available Packages

* `deno_2.1.2_aarch64.deb` — Deno 2.1.2 for ARM 64-bit (aarch64) Termux
  *(More architectures may be added in the future)*

---

## 🚀 Installation

### 1. Download the latest `.deb` package:

```bash
wget https://github.com/jobians/termux-deno-prebuilt/releases/download/v2.1.2/deno_2.1.2_aarch64.deb
```

> 💡 You can find the latest version on the [Releases page](https://github.com/jobians/termux-deno-prebuilt/releases).

---

### 2. Install the package:

```bash
pkg install libffi
dpkg -i deno_2.1.2_aarch64.deb
```

---

### 3. Fix any missing dependencies:

```bash
pkg install -f
```

---

### 4. Verify the installation:

```bash
deno --version
```

---

## ⚠️ Notes

* These packages are specifically built for Termux on Android devices and tested on aarch64 architecture.
* If you encounter issues or want to request support for other architectures, please open an issue or submit a pull request.

---

## 🙏 Thanks

Thanks to the Termux community, the Deno project, and the [0komo/termux-packages](https://github.com/0komo/termux-packages) fork for making this possible!
