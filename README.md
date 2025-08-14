````markdown
<h1 align="center">🚀 EthStorage V1 Trusted Setup Ceremony</h1>
<p align="center">
  <b>Local System / VPS Guide</b> <br>
  <i>Contribute • Earn • Be a part of the Trusted Setup</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Ubuntu-22.04-orange?logo=ubuntu&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-18.x-green?logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/NPM-9.2-red?logo=npm&logoColor=white" />
  <img src="https://img.shields.io/badge/Status-Active-brightgreen" />
</p>

---

## 📌 Prerequisites

| Requirement        | Minimum |
|--------------------|---------|
| **OS**             | Ubuntu 22.04 (Local या VPS) |
| **CPU**            | 2 vCPU  |
| **RAM**            | 4 GB    |
| **Storage**        | 30 GB+ SSD |
| **GitHub Account** | ≥ 1 महीना पुराना, ≥ 1 Public repo, ≥ 5 Followers, ≥ 1 Following, Gists enabled |

---

## 🛠 Installation & Setup

### **1️⃣ सिस्टम अपडेट करें**
```bash
sudo apt update && sudo apt upgrade -y
sudo apt install -y curl git build-essential
````

### **2️⃣ Node.js v18 और npm v9.2 इंस्टॉल करें**

```bash
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install -y nodejs
sudo npm install -g npm@9.2
```

### **3️⃣ वर्शन चेक करें**

```bash
node -v
npm -v
```

### **4️⃣ Temporary वर्कस्पेस बनाएं**

```bash
mkdir ~/trusted-setup-tmp && cd ~/trusted-setup-tmp
```

### **5️⃣ Phase2 CLI इंस्टॉल करें**

```bash
sudo npm install -g @p0tion/phase2cli
```

### **6️⃣ CLI वर्शन चेक करें**

```bash
phase2cli --version
```

### **7️⃣ GitHub Authentication**

```bash
phase2cli auth
```

* ब्राउज़र में GitHub login करें
* **p0tion** को Gists read/write access allow करें

### **8️⃣ Ceremony में योगदान दें**

```bash
screen -S ceremony
phase2cli contribute -c ethstorage-v1-trusted-setup-ceremony
```

* `screen` से बाहर: **Ctrl+A, D**
* वापस आने के लिए: `screen -r ceremony`

### **9️⃣ Cleanup**

```bash
phase2cli clean
phase2cli logout
rm -rf ~/trusted-setup-tmp
```

---

## ✅ GitHub Checklist

* [x] अकाउंट ≥ 1 महीना पुराना
* [x] ≥ 1 Public Repository
* [x] ≥ 5 Followers
* [x] ≥ 1 Following
* [x] GitHub Gists enabled

---

## 🎯 Tips

* `screen` या `tmux` का इस्तेमाल करें ताकि डिस्कनेक्ट होने पर भी प्रोसेस चलता रहे।
* Contribution पूरा होने के बाद VPS terminate कर दें या लोकल temp files delete कर दें।

---

<p align="center">🎉 <b>Done! आप Ceremony में सफलतापूर्वक जुड़ गए हैं।</b> 🎉</p>
```
