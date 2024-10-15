<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=EB+Garamond&weight=800&size=28&duration=4000&pause=1000&random=false&width=435&lines=+VIPPER_BUG;WHATSAPP+CRASH+x+BUG+BOT;DEVELOPED+BY+𝐂𝐀𝐒𝐄𝐘𝐑𝐇𝐎𝐃𝐄𝐒 🌟" alt="Typing SVG" />
  </a>
</p>

![VIPPER_BUG](https://i.imgur.com/wOfxm0e.jpeg)
<p align="center">
<a href="https://www.youtube.com/@Caseyrhodes01"><img src="https://img.shields.io/badge/YouTube-ff0000?style=for-the-badge&logo=youtube&logoColor=ff000000&link=https://youtube.com/@caseyrhodes02" /><br>
<a href="https://whatsapp.com/channel/0029VakUEfb4o7qVdkwPk83E"><img src="https://img.shields.io/badge/WhatsApp Channel-25D366?style=for-the-badge&logo=whatsapp&logoColor=white&link=https://whatsapp.com/channel/0029VakUEfb4o7qVdkwPk83E" /><br>

---

## DEVELOPED BY 𝐂𝐀𝐒𝐄𝐘𝐑𝐇𝐎𝐃𝐄𝐒 🌟

---

## CREATE YOUR FORK
<a href="https://github.com/caseyweb/VIPPER_BUG/fork">
  <img title="VIPPER_BUG" src="https://img.shields.io/badge/FORK-VIPPER_BUG-red?color=red&style=for-the-badge&logo=stackshare">
</a>

---

### 🔐 Generate Pair Code For Session

#### PAIRING SERVER 
<a href="https://drk-tech-1.onrender.com/" target="_blank">
  <img alt="Pairing Code Server " src="https://img.shields.io/badge/PAIRING CODE-green?style=for-the-badge&logo=opencv&logoColor=white"/>
</a>

---

###  🐛DEPLOYMENTS👌

<div align="center">
  <!-- Badges for deployment -->
  <a href="https://youtu.be/AZg7UMMy6q8?si=_YyYGgUS1AL9oR-B" target="_blank">
    <img src="https://img.shields.io/badge/Deployment-GitHub-blue?style=for-the-badge&logo=github" alt="GitHub Deployment" />
  </a>
  <a href="https://youtu.be/4b1HNuaQx54?si=CSRoq27E8nS0AeNA" target="_blank">
    <img src="https://img.shields.io/badge/Deployment-Codespace-blue?style=for-the-badge&logo=github" alt="Codespace Deployment" />
  </a>
  <a href="https://youtu.be/yH2KCK0AD4I?si=F5tjgBpK4ZQO0F-x" target="_blank">
    <img src="https://img.shields.io/badge/Deployment-Replit-blue?style=for-the-badge&logo=replit" alt="Replit Deployment" />
  </a>
  
---

## ⚠️ WARNING ⚠️

I am not responsible for any damage caused by this bot. Use this bot at your own risk. It is developed for educational purposes only. Any malicious use is strictly discouraged.

---

<details>
  <summary><strong>Show more</strong></summary>


---

## Developer 💀

<a href="https://github.com/VIPPER_BUG">
  <img src="https://github.com/VIPPER_BUG.png" width="200" height="200" alt="VIPPER_BUG"/>
</a>
<p align="center"><strong>VIPPER_BUG</strong></p>

---

## Contributors 🤝

<a href="https://github.com/caseyweb">
  <img src="https://github.com/caseyweb.png" width="200" height="200" alt="caseyrhodes"/>
</a>
<p align="center"><strong>CASEYRHODES</strong

---

## GitHub Deployment

```yaml
name: Node.js CI

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main
  schedule:
    - cron: '0 */6 * * *'  

jobs:
  build:

    runs-on: ubuntu-latest

    strategy:
      matrix:
        node-version: [20.x]

    steps:
    - name: Checkout repository
      uses: actions/checkout@v3

    - name: Set up Node.js
      uses: actions/setup-node@v3
      with:
        node-version: ${{ matrix.node-version }}

    - name: Install dependencies
      run: npm install

    - name: Install FFmpeg
      run: sudo apt-get install -y ffmpeg

    - name: Start application with timeout
      run: |
        timeout 21590s npm start  # Limits run to 5h 59m 50s

    - name: Save state (Optional)
      run: |
        ./save_state.sh
