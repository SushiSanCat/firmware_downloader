<h1 align="center">⚡ Realme Firmware Downloader</h1>

<p align="center">
  <i>A blazing fast, no-setup firmware and OTA downloader for Realme devices</i><br>
  <b>Built with 💻 Batch Script + ⚙️ Native Binary (.exe)</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-windows-blue?style=flat-square" />
  <img src="https://img.shields.io/github/license/YOUR_USERNAME/realme-firmware-downloader?style=flat-square" />
  <img src="https://img.shields.io/badge/script-.bat-yellow?style=flat-square" />
  <img src="https://img.shields.io/badge/binary-.exe-lightgrey?style=flat-square" />
</p>

---

## 🧩 What is This?

**Realme Firmware Downloader** is a lightweight Windows tool that allows you to download official Realme OTA and firmware files using just your device model and firmware version string.

No Python. No dependencies. Just double-click and download.

---

## ⚙️ How It Works

> 🛠 Powered by:
> - `downloader.bat`: A smart script wrapper
> - `bin.exe`: A helper binary that builds and fetches the direct OTA link

The batch script parses your input and passes it to the `.exe`, which constructs the official download URL — fast, clean, and offline-friendly.

---

## 🚀 Usage

### ▶️ Method 1: Drag & Drop
1. Extract `FirmwareDownloader_English_by_NeFeroN.zip` onto your desktop.
2. Double-click the `Downloader.bat`.
3. Enter the link of the ota, like:
```
https://gauss-componentotacostmanual-sg.allawnofs.com/remove-27e6bc730df1dccb48d6485b235beeb7/component-ota/25/02/27/96f1df8b8e344eb897fc0884899bec6f.zip
```
(you can get the link of your device's latest ota by installing the android app `oplus_ota_finder.apk` here: https://github.com/SushiSanCat/oplus_ota_finder)
but if you try to access this link directly then it will give you access denied.

4. The tool will fetch the OTA link and begin download automatically.

---

### ▶️ Method 2: Command Prompt

```cmd
Downloader.bat RMX3472_14.0.0.800(EX01)
```

You’ll see something like:

```
[✔] Fetching OTA link...
[🔗] https://gauss-componentotacostmanual-eu.allawnofs.com/remove-<HASH>/component-ota/24/08/27/<HASH>.zip
[⬇️] Downloading... please wait
```

The ZIP will be saved in the current folder.

---

## 📦 Output

- 🔗 Official OTA or full firmware URL
- 💾 Saves `.zip` to the folder where the script is run
- 📁 Future versions may log metadata to a file

---

## 🛠 Requirements

- 🖥 Windows 7/10/11
- Internet access
- Realme firmware version code (e.g., `RMX3472_14.0.0.800(EX01)`)

---

## ✅ Tested On

- ✔ Realme 9 Pro (RMX3472)
- ✔ Other RMX-series devices (manual entry required)

---

## 🧠 Power Modder Tips

- Combine with `payload_dumper` to extract `boot.img`, `vbmeta.img`, etc.
- Flash extracted images using `fastboot`
- Use with Magisk for root
- Safe for backups or offline flashing

---

## ⚠️ Disclaimer

> This project is not affiliated with Realme or any of its partners. Use at your own risk. Downloading and flashing the wrong firmware may brick your device. Always double-check model and version before proceeding.

---

## 🙏 Credits

- Inspired by the Realme & Android modding community
- Thanks to OTA reverse engineers
- Special thanks to YOU for trying this tool 🙌

---

## 📜 License

MIT License. See [LICENSE](LICENSE) file for details.
