# <img src="https://falconpdf.com/images/logo.png" alt="Falcon PDF Logo" width="40"/> Falcon PDF App


## 🚀 About Falcon PDF

Falcon PDF is a powerful **cross-platform PDF viewer, editor, and collaboration tool**.  
Available on **Android, iOS, Web, Windows, macOS, Linux, Chromebooks, and TVs**.  

🚫 **No Ads** — Even in the free version, and we promise to never add them.  
⭐ **Favorites Sync** — Mark PDFs as favorite and sync securely to **Google Drive**. Access them anywhere, even on TVs.  
📚 **One App, All-in-One Solution** — Includes **30+ robust PDF tools** (organizing, AI summarization, editing, encryption, signing, etc.), **document scanning** (mobile apps only for now), and a **powerful collaborative PDF viewer** (comments, form filling, editing).  

## ⬇️ Download

Falcon PDF is available on all major platforms. The Direct download links always point to the **[latest release](https://github.com/avrapps/falcon-pdf-app/releases/latest)** on GitHub.

| Platform | App Store | Direct download |
| --- | --- | --- |
| **Android** (Mobiles, Tablets, Chromebooks & TVs) | [![Google Play](https://img.shields.io/badge/Google_Play-414141?logo=google-play&logoColor=white)](https://play.google.com/store/apps/details?id=com.avrapps.pdfviewer) | [![.apk](https://img.shields.io/badge/.apk-3DDC84?logo=android&logoColor=white)](https://github.com/avrapps/falcon-pdf-app/releases/latest) |
| **iOS** (iPhone & iPad) | [![App Store](https://img.shields.io/badge/App_Store-0D96F6?logo=apple&logoColor=white)](https://apps.apple.com/app/falcon-pdf-editor-tools/id6760542830) | — |
| **Windows** | [![Microsoft Store](https://img.shields.io/badge/Microsoft_Store-0078D4?logo=microsoft&logoColor=white)](https://apps.microsoft.com/detail/9p18j5g85clt) | [![.msi](https://img.shields.io/badge/.msi-0078D4?logo=windows&logoColor=white)](https://github.com/avrapps/falcon-pdf-app/releases/latest) [![.exe](https://img.shields.io/badge/.exe_portable-0078D4?logo=windows&logoColor=white)](https://github.com/avrapps/falcon-pdf-app/releases/latest) |
| **macOS** | [![Mac App Store](https://img.shields.io/badge/Mac_App_Store-000000?logo=apple&logoColor=white)](https://apps.apple.com/app/falcon-pdf-editor-tools/id6760542830) | [![.dmg](https://img.shields.io/badge/.dmg-000000?logo=apple&logoColor=white)](https://github.com/avrapps/falcon-pdf-app/releases/latest) |
| **Linux** | [![Snap Store](https://img.shields.io/badge/Snap_Store-82BEA0?logo=snapcraft&logoColor=white)](https://snapcraft.io/falcon-pdf) [![FlatPark](https://img.shields.io/badge/Flatpak-FlatPark-4A90D9?logo=flatpak&logoColor=white)](https://flatpark.org/apps/com.falconpdf.app) | [![.deb](https://img.shields.io/badge/.deb-A81D33?logo=debian&logoColor=white)](https://github.com/avrapps/falcon-pdf-app/releases/latest) [![.rpm](https://img.shields.io/badge/.rpm-EE0000?logo=redhat&logoColor=white)](https://github.com/avrapps/falcon-pdf-app/releases/latest) [![AppImage](https://img.shields.io/badge/AppImage-FCC624?logo=linux&logoColor=black)](https://github.com/avrapps/falcon-pdf-app/releases/latest) [![Pacman](https://img.shields.io/badge/Pacman-1793D1?logo=archlinux&logoColor=white)](https://github.com/avrapps/falcon-pdf-app/releases/latest) |
| **Web** (any browser) | [![Web App](https://img.shields.io/badge/Web_App-Open_in_browser-4285F4?logo=googlechrome&logoColor=white)](https://app.falconpdf.com/) | — |

### 💻 Command-line installation

Prefer the terminal? On **Windows** use `winget` and on **macOS** use Homebrew — both always pull the latest published version. On **Linux**, the commands below download the installer straight from the latest [GitHub release](https://github.com/avrapps/falcon-pdf-app/releases/latest) using the GitHub API to resolve the newest asset automatically (requires `curl` and `jq`).

**Linux — Snap (all distros)**
```bash
sudo snap install falcon-pdf
```

**Linux — Flatpak via [FlatPark](https://flatpark.org/apps/com.falconpdf.app) (all distros)**
```bash
flatpak remote-add --if-not-exists flatpark https://dl.flatpark.org/flatpark.flatpakrepo
flatpak install flatpark com.falconpdf.app
```

**Linux — Debian / Ubuntu (.deb)**
```bash
curl -sL "$(curl -sL https://api.github.com/repos/avrapps/falcon-pdf-app/releases/latest \
  | jq -r '.assets[] | select(.name | endswith(".deb")) | .browser_download_url')" -o falconpdf.deb \
  && sudo apt-get install -y ./falconpdf.deb
```

**Linux — Fedora / RHEL (.rpm)**
```bash
curl -sL "$(curl -sL https://api.github.com/repos/avrapps/falcon-pdf-app/releases/latest \
  | jq -r '.assets[] | select(.name | endswith(".rpm")) | .browser_download_url')" -o falconpdf.rpm \
  && sudo dnf install -y ./falconpdf.rpm
```

**Linux — AppImage (portable, any distro)**
```bash
curl -sL "$(curl -sL https://api.github.com/repos/avrapps/falcon-pdf-app/releases/latest \
  | jq -r '.assets[] | select(.name | endswith(".AppImage")) | .browser_download_url')" -o FalconPDF.AppImage \
  && chmod +x FalconPDF.AppImage && ./FalconPDF.AppImage
```

**Linux — Arch (.pacman)**
```bash
curl -sL "$(curl -sL https://api.github.com/repos/avrapps/falcon-pdf-app/releases/latest \
  | jq -r '.assets[] | select(.name | endswith(".pacman")) | .browser_download_url')" -o falconpdf.pacman \
  && sudo pacman -U falconpdf.pacman
```

**Windows — winget**
```powershell
winget install --id 9P18J5G85CLT --source msstore
```

**macOS — Homebrew (cask)**
```bash
brew tap avrapps/tap && brew install --cask falcon-pdf
```

> Tip: You can also install from the app stores or package managers — see the [Download](#️-download) table above for Google Play, App Store, Microsoft Store, Snap Store, and FlatPark (Flatpak) links.



## ✨ Features

### 📖 Viewer
- Recent files & favorites (sync across devices with Drive)  
- Multi-device support (Mobiles, Web, Desktop, Chromebooks, TVs)  
- Multiple themes & adaptive theme  
- **Dark Mode** (Pro)  
- **Readout PDFs aloud** (Premium)  
- Support for **10+ document formats**: FB2/3, DOC/DOCX, TXT, CHM/HTML, RTF, EPUB, TIFF  

### 📝 Editor
- Create / update / delete annotations  
- Edit text inside PDFs  
- Fill forms  
- Run embedded JavaScript  
- Create PDFs  
- PDF manipulation tools (Encrypt, Decrypt, Digital Signature, Rearrange, etc.)  

### 🤝 Collaboration
- Replies on annotations & in-PDF chat  
- Share PDFs easily  
- Sync files across devices  

### 🛠 Tools
- Security features  
- Convert from PDF to other formats  

### 📷 Scanner
- Scan documents from camera  
- Cloud backup & sync  
- Organize scanned documents  
- OCR (Text recognition & reading)  
- Create PDFs from scans  

### 🏢 Enterprise
- Dedicated technical assistance & support channels  
- Configurable private cloud setup (AWS, company-owned infra)  


## 🌍 Community & Support

- 🌐 Website: [https://falconpdf.com](https://falconpdf.com)
- ✖️ X (Twitter): [https://x.com/falcon_pdf](https://x.com/falcon_pdf)
- 📘 Facebook: [https://www.facebook.com/profile.php?id=61584270131681](https://www.facebook.com/profile.php?id=61584270131681)
- 💬 WhatsApp Channel: [https://whatsapp.com/channel/0029Va4rWa2JENy9pTvxGL24](https://whatsapp.com/channel/0029Va4rWa2JENy9pTvxGL24)
- 🎮 Discord: [https://discord.gg/YMedDK2c3](https://discord.gg/YMedDK2c3)
- ✈️ Telegram: [https://t.me/falconpdf](https://t.me/falconpdf)
- 💼 LinkedIn: [https://www.linkedin.com/company/falcon-pdf/](https://www.linkedin.com/company/falcon-pdf/)
- ▶️ YouTube: [https://www.youtube.com/@FalconPDF](https://www.youtube.com/@FalconPDF)
- 🧵 Threads: [https://www.threads.com/@falcon_pdf](https://www.threads.com/@falcon_pdf)
- 📸 Instagram: [https://www.instagram.com/falcon_pdf/](https://www.instagram.com/falcon_pdf/)  


## 📜 License

© 2025 Falcon PDF. All rights reserved by ANRMS Private Limited.
