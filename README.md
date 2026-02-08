# 💊 UrlCapsule

**UrlCapsule** is a private, serverless file‑sharing tool that encapsulates files directly into a URL hash. It requires **no database, no cloud storage, and no backend** — just pure browser‑side logic.

🔗 **Live Tool:** [https://giriaryan694-a11y.github.io/UrlCapsule/](https://giriaryan694-a11y.github.io/UrlCapsule/)

---

## 🚀 Features

* **100% Private**
  Your files never touch a server. They exist only inside the link you generate.

* **No Expiry**
  Since there is no database or storage layer, the link works as long as the URL remains intact.

* **High Capacity (for URLs)**
  Uses the **URL Fragment Identifier (`#`)** to support files up to ~2MB (browser‑dependent).

* **Zero Infrastructure**
  A single HTML file — host it on GitHub Pages, Vercel, or run it locally.

* **Minimal & Fast**
  Built for speed, simplicity, and portability.

---

## 🛠️ How It Works

### 1️⃣ Encoding

* The browser reads the selected file using the **FileReader API**.
* The file is converted into a **Base64 string**.

### 2️⃣ Encapsulation

* File data, name, and MIME type are wrapped into a JSON object.
* The JSON payload is compressed and stored inside the URL hash (`#`).

### 3️⃣ Decoding

* When the link is opened, the browser detects the hash data.
* The file is reconstructed entirely on the client side.
* A download button is generated automatically.

---

## 📋 Technical Specifications

| Feature       | Limit / Detail           |
| ------------- | ------------------------ |
| Max File Size | ~2MB (browser dependent) |
| Technology    | HTML5, JavaScript        |
| APIs Used     | FileReader API           |
| Storage       | None (Client‑side only)  |
| Encoding      | Base64                   |

---

## 💻 Installation & Usage

1. Download the `index.html` file.
2. Open it in any modern web browser.
3. Select a file (under 2MB).
4. Copy the generated **Massive Link**.
5. Send the link to the recipient via email or direct message.

*No build step. No dependencies. No setup.*

---

## ⚠️ Limitations

* **Very Long URLs**
  Since file data is embedded in the link, URLs can become extremely long. Some platforms (e.g., WhatsApp, Discord) may truncate them.

  **Best Practice:**
  Paste the link directly into the browser address bar or send via email.

* **P2P Only**
  There is no file management or recovery. If you lose the link, the file is permanently lost.

---

## 🔐 Security Model

* No servers
* No uploads
* No logs
* No tracking

All operations happen **entirely in your browser**.

---

## 👤 Credits

Developed by **Aryan Giri**

---

## 📜 License

Licensed under the **Apache License 2.0**.
---

> ⚡ UrlCapsule is ideal for quick, private, infrastructure‑free file sharing where privacy matters more than permanence.
