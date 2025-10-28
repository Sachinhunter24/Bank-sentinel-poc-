# ek folder banao aur git initialize karo
mkdir bank-sentinel-poc
cd bank-sentinel-poc
git init

# README add karo
echo "# Bank Sentinel — PoC" > README.md
git add README.md
git commit -m "init: add README"

# Baaki files add karo
mkdir legal deploy
echo "NDA content" > legal/nda.md
echo "docker-compose placeholder" > deploy/docker-compose.yml
git add .
git commit -m "add initial files and folders"

# Remote connect karo
git remote add origin https://github.com/Sachin24hunter/bank-sentinel-poc.git
git branch -M main
git push -u origin main
