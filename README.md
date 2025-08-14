# EthStorage V1 Trusted Setup Ceremony - VPS/Local Guide

## Requirements
- Ubuntu 22.04 (Local PC या VPS)
- 2 vCPU, 4 GB RAM, 30+ GB SSD
- GitHub account (>= 1 month old, >= 1 public repo, >= 5 followers, >= 1 following, Gists enabled)

----------------------------------------

# 1. सिस्टम अपडेट करें
sudo apt update && sudo apt upgrade -y
sudo apt install -y curl git build-essential screen

# 2. Node.js v18 और npm v9.2 इंस्टॉल करें
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install -y nodejs
sudo npm install -g npm@9.2

# 3. वर्शन चेक करें
node -v
npm -v

# 4. Temporary वर्कस्पेस बनाएं
sudo mkdir ~/trusted-setup-tmp && cd ~/trusted-setup-tmp

# 5. Phase2 CLI इंस्टॉल करें
sudo npm install -g @p0tion/phase2cli

# 6. CLI वर्शन चेक करें
phase2cli --version

# 7. GitHub Authentication
sudo phase2cli auth
# GitHub login करें और p0tion को Gists read/write access allow करें

# 8. Ceremony में योगदान दें (VPS users के लिए Screen का use)
sudo screen -S ceremony

sudo phase2cli contribute -c ethstorage-v1-trusted-setup-ceremony

# Screen commands:
# बाहर जाने के लिए: Ctrl+A, D
# वापस आने के लिए: sudo screen -r ceremony
# सभी sessions देखने के लिए: sudo screen -ls
# किसी session को resume करने के लिए: sudo screen -r <ID>

# 9. Cleanup (optional)
sudo phase2cli clean
sudo phase2cli logout
sudo rm -rf ~/trusted-setup-tmp

----------------------------------------

## GitHub Checklist
- अकाउंट >= 1 महीना पुराना
- >= 1 Public Repository
- >= 5 Followers
- >= 1 Following
- GitHub Gists enabled

# Done! Ceremony में सफलतापूर्वक शामिल हो गए।
