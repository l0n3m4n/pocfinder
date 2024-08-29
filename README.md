<h2 align="center">
  PoC Finder 
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExb3lybGJrZnI4aXJuYjBmOHVxZTR5azcyanlrNGtzbTY3b2xkODc5ZiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT9IgFLfWUZigjoem4/giphy.gif" width="28">
</h2>

<p align="center">
<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=28E914&random=false&width=435&lines=PoC+Finder+is+a+specialized+tool++;design+for+discovering+(PoC)+;and+providing+detailed+information;about++common++vulnerabilities+;exposure+(CVE)+" alt="Typing SVG" /></a>
</p>


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


[![asciicast](https://asciinema.org/a/666760.svg)](https://asciinema.org/a/666760)
## 📚 Table of Contents
- 📜 [Description](#-description)
- 🛠️ [Installation](#-installation)
- 💡 [Features](#-features)
- ⚙️ [Usage](#-usage)
- 💁 [References](#-references)
- 👨🏾‍⚖️ [License](#-license)

 
## 📜 Description
Poc Finder and CVE Details tool is a powerful yet a simple utility designed for pentesters and cybersecurity researchers to streamline the process of discovering proof of concept (PoC) and accessing essential details about Common Vulnerabilities and Exposures (CVEs). This tool integrates advanced search functionalities with comprehensive CVE database access.

## 💡 Features

- **Search and Discovery**: Quickly find `POCs` for known vulnerabilities by searching through `databases` and `repositories`.
- **CVE Information**: Retrieve `comprehensive details` about CVEs, including descriptions, `severity levels`, `affected software versions`, `mitigation` and `references`.
- **Automatic Updates**: `Regularly updates` its database to ensure access to the latest CVE information and POCs.
- **Export Capabilities**: `Export` CVE details and POCs in various formats (`HTML`, `JSON`, `CSV`, `TXT`, `docx`) for further analysis or reporting.
- **User-Friendly Interface**: `Intuitive interface` for ease of use, making it accessible to both security professionals and enthusiasts.

## 🛠️ Installation

### Installing pocfinder 
```bash
# creating virtual environment
$ sudo apt install python3.11-venv
$ python3 -m pip install virtualenv 
$ python3 -m venv venv 

# cloning repo
$ git clone https://github.com/l0n3m4n/pocfinder.git
$ cd pocfinder && source venv/bin/activate
$ pip install -r requirement.txt
$ chmod +x pocfinder.py && python3 pocfinder.py -h
```
## ⚙️ Usage
![logo](/assets/pocfinder.png)

## 📝 Todo
- [x] **~~Adding total entries~~**
- [x] **~~Adding default html report templates~~**
- [x] **~~Adding html,csv,json,docx report output~~**
- [ ] **Adding Dockerfile for easy deployment**
- [ ] **Extending features and custom templates**

 

## 👨🏾‍⚖️ License
This project is under terms of the [MIT License](LICENSE). For fixing Bugs, create [issue](https://github.com/l0n3m4n/pocfinder/issues/new)
