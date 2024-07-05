 <p align="center">
    <a href="https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fl0n3m4n%2Fpocfinder">
    <img src="https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fl0n3m4n%2Fpocfinder&label=Visitors&countColor=%2337d67a" />
    </a>
    <a href="https://www.facebook.com/l0n3m4n">
        <img src="https://img.shields.io/badge/Facebook-%231877F2.svg?style=for-the-badge&logo=Facebook&logoColor=white" alt="Facebook">
    </a>
      <a href="https://www.twitter.com/l0n3m4n">
        <img src="https://img.shields.io/badge/Twitter-%23000000.svg?style=for-the-badge&logo=X&logoColor=white" alt="X">
    </a>
    <a href="https://medium.com/@l0n3m4n">
        <img src="https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white" alt="Medium">
    </a>
    <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" alt="Python">
    </a>
    <a href="https://www.kali.org/">
    <img src="https://img.shields.io/badge/Kali-268BEE?style=for-the-badge&logo=kalilinux&logoColor=white" alt="Kali">      
    </a>
</p>



# PoC Finder 
[![asciicast](https://asciinema.org/a/666760.svg)](https://asciinema.org/a/666760)
## 📚 Table of Contents
- 📜 [Description](#-description)
- 🛠️ [Installation](#-installation)
- ⚙️ [Usage](#-usage)
- 💁 [References](#-references)
- 👨🏾‍⚖️ [License](#-license)

 
## 📜 Description
Poc Finder and CVE Details tool is a powerful yet a simple utility designed for pentesters and cybersecurity researchers to streamline the process of discovering proof of concept (PoC) and accessing essential details about Common Vulnerabilities and Exposures (CVEs). This tool integrates advanced search functionalities with comprehensive CVE database access.

## 🛠️ Installation

### Installing pocfinder 
```bash
# creating virtual environment
$ sudo apt install python3.11-venv
$ python3 -m pip install virtualenv 
$ python3 -m venv venv 

# cloning pocfinder
$ git clone https://github.com/l0n3m4n/pocfinder.git
$ cd pocfinder && source venv/bin/activate
$ pip install -r requirement.txt
$ chmod +x pocfinder.py && python3 pocfinder.py -h
```
## ⚙️ Usage
![logo](/assets/pocfinder.png)
## 💁 References
- [**Exploit Observer**](https://api.exploit.observer)

## 📝 Todo
- [x] **~~Adding total entries~~**
- [x] **~~Adding default html report templates~~**
- [x] **~~Adding html,csv,json,docx report output~~**
- [ ] **Extending features and custom templates**

 

## 👨🏾‍⚖️ License
This project is under terms of the [MIT License](LICENSE). For fixing Bugs, create [issue](https://github.com/l0n3m4n/pocfinder/issues/new)
