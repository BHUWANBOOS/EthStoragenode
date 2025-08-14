hi

---

````markdown
# 🚀 EthStorage V1 Trusted Setup Ceremony (Local/VPS Guide)

## 📌 Requirements
- Ubuntu 22.04 (Local PC या VPS)
- 2 vCPU, 4 GB RAM, 30+ GB SSD
- GitHub account (≥ 1 महीना पुराना, ≥ 1 Public repo, ≥ 5 followers, ≥ 1 following, Gists enabled)

---

## 🛠 Installation Steps

### 1. सिस्टम अपडेट करें
```bash
sudo apt update && sudo apt upgrade -y
sudo apt install -y curl git build-essential
````

### 2. Node.js v18 और npm v9.2 इंस्टॉल करें

```bash
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install -y nodejs
sudo npm install -g npm@9.2
```

### 3. वर्शन चेक करें

```bash
node -v
npm -v
```

### 4. Temporary वर्कस्पेस बनाएं

```bash
mkdir ~/trusted-setup-tmp && cd ~/trusted-setup-tmp
```

### 5. Phase2 CLI इंस्टॉल करें

```bash
sudo npm install -g @p0tion/phase2cli
```

### 6. CLI वर्शन चेक करें

```bash
phase2cli --version
```

### 7. GitHub Authentication

```bash
phase2cli auth
```

* GitHub login करें
* **p0tion** को Gists read/write access allow करें

### 8. Ceremony में योगदान दें

```bash
phase2cli contribute -c ethstorage-v1-trusted-setup-ceremony
```

* `screen` से बाहर: **Ctrl+A, D**
* वापस आने के लिए:

```

### 9. Cleanup (optional)

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

🎉 **Done!** अब आप Ceremony में सफलतापूर्वक शामिल हो गए हैं।

```

---

ये version 100% plain text है — कोई hidden character या fancy quotes नहीं,  
GitHub में डालोगे तो commands एकदम clean copy होंगी और terminal में error नहीं आएगा।  

तुम चाहो तो मैं अभी इसे तुम्हारे `BHUWANBOOS/EthStoragenode` repo के README में डालने के लिए final version बना सकता हूँ।
```
