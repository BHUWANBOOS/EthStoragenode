# **EthStorage Trusted Setup Ceremony - VPS / Local Guide**

### **📌 Requirements**

* Ubuntu 22.04 (Local PC या VPS)
* 2 vCPU, 4 GB RAM, 30+ GB SSD
* GitHub account:

  * उम्र ≥ 1 महीना
  * ≥ 1 Public Repo
  * ≥ 5 Followers
  * ≥ 1 Following
  * **Gists Enabled**

---

## **1️⃣ सिस्टम अपडेट करें**

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install -y curl git build-essential screen
```

---

## **2️⃣ Node.js v18 और npm v9.2 इंस्टॉल करें**

```bash
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install -y nodejs
sudo npm install -g npm@9.2
```

---

## **3️⃣ वर्शन चेक करें**

```bash
node -v
npm -v
```

---

## **4️⃣ Temporary वर्कस्पेस बनाएं**

```bash
mkdir ~/trusted-setup-tmp && cd ~/trusted-setup-tmp
```

---

## **5️⃣ Phase2 CLI इंस्टॉल करें**

```bash
npm install -g @p0tion/phase2cli
```

---

## **6️⃣ CLI वर्शन चेक करें**

```bash
phase2cli --version
```

---

## **7️⃣ GitHub Authentication**

```bash
phase2cli auth
```

> GitHub login करें और **p0tion** को Gists read/write access allow करें

---

## **8️⃣ Ceremony में योगदान दें**

**VPS Users के लिए Screen का Use:**

```bash
screen -S ceremony
phase2cli contribute -c ethstorage-v1-trusted-setup-ceremony
```

**Screen Commands:**

```bash
# सेशन से बाहर निकलने के लिए
Ctrl + A, फिर D

# सेशन में वापस आने के लिए
screen -r ceremony

# सभी सेशन देखने के लिए
screen -ls

# किसी स्पेसिफिक सेशन को Resume करने के लिए
screen -r <ID>
```

---

## **9️⃣ Cleanup (Optional)**

```bash
phase2cli clean
phase2cli logout
rm -rf ~/trusted-setup-tmp
```

---

✅ अब आप Ceremony में सफलतापूर्वक शामिल हो चुके हैं! 🎉
