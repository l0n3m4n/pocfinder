<div align="right">
  <a href="https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fl0n3m4n%2Fpocfinder">
    <img src="https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fl0n3m4n%2Fpocfinder&label=Visitors&countColor=%2337d67a" />
  </a>
</div>


# PoC Finder 
📚 Table of Contents
- 📜 [Description](#-description)
- 🛠️ [Installation](#-installation)
- ⚙️ [Usage](#-usage)
- 💁 [References](#-references)
- 📌 [Author](#-author)
- 👨🏾‍⚖️ [License](#-license)

 
## 📜 Description
The Poc Finder and CVE Details tool is a powerful yet simple utility designed for cybersecurity professionals and researchers to streamline the process of discovering (PoC) and accessing essential details about Common Vulnerabilities and Exposures (CVEs). This tool integrates advanced search functionalities with comprehensive CVE database access.

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
### Sample usage
```py
$ python3 pocfinder.py CVE-2024-4577 --export txt --save CVE-2024-4577.html 

██████╗  ██████╗  ██████╗███████╗██╗███╗   ██╗██████╗ ███████╗██████╗ 
██╔══██╗██╔═══██╗██╔════╝██╔════╝██║████╗  ██║██╔══██╗██╔════╝██╔══██╗
██████╔╝██║   ██║██║     █████╗  ██║██╔██╗ ██║██║  ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║     ██╔══╝  ██║██║╚██╗██║██║  ██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚██████╗██║     ██║██║ ╚████║██████╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚═════╝╚═╝     ╚═╝╚═╝  ╚═══╝╚═════╝ ╚══════╝╚═╝  ╚═╝
    Author: l0n3m4n | CVE Details and PoC Finder | Version: v1.2     

Fetching CVE information for CVE ID: CVE-2024-4577...

Fetching Data |████████████████████████████████████████| 1/1 [100%] in 3.2s (0.31/s) 

+-------------+--------------------------------------------------------------+
| File Type   | URLs                                                         |
+=============+==============================================================+
| c           | https://github.com/php/php-src                               |
+-------------+--------------------------------------------------------------+
| c++         | https://github.com/vwilzz/php-rce-4577                       |
+-------------+--------------------------------------------------------------+
| go          | https://github.com/tam-k592/cve-2024-4577                    |
+-------------+--------------------------------------------------------------+
| go          | https://github.com/zan8in/afrog                              |
+-------------+--------------------------------------------------------------+
| go          | https://github.com/zephrfish/cve-2024-4577-php-rce           |
+-------------+--------------------------------------------------------------+
| go          | https://github.com/zomasec/cve-2024-4577                     |
+-------------+--------------------------------------------------------------+
| html        | https://github.com/advisories/GHSA-vxpp-6299-mxw3            |
+-------------+--------------------------------------------------------------+
| html        | https://github.com/mr-xn/penetration_testing_poc             |
+-------------+--------------------------------------------------------------+
| javascript  | https://github.com/projectdiscovery/nuclei-templates         |
+-------------+--------------------------------------------------------------+
| markdown    | https://github.com/0x20c/cve-2024-4577-nuclei                |
+-------------+--------------------------------------------------------------+
| markdown    | https://github.com/0xmarcio/cve                              |
+-------------+--------------------------------------------------------------+
| markdown    | https://github.com/abosteam/popc                             |
+-------------+--------------------------------------------------------------+
| markdown    | https://github.com/alpereny-cs/cve-2024-4577                 |
+-------------+--------------------------------------------------------------+

Data saved to CVE-2024-4577.html
Total Entries: 108 out of 20 entries display on terminal


Data saved to CVE-2024-4577.html
```
## Html PoC report example
![report sample](/assets/report.png)

## TXT file exmaple
```bash
Description: Exploit Observer has 108 entries in 14 file formats related to CVE-2024-4577. In PHP versions 8.1.* before 8.1.29, 8.2.* before 8.2.20, 8.3.* before 8.3.8, when using Apache and PHP-CGI on Windows, if the system is set up to use certain code pages, Windows may use "Best-Fit" behavior to replace characters in command line given to Win32 API functions. PHP CGI module may misinterpret those characters as PHP options, which may allow a malicious user to pass options to PHP binary being run, and thus reveal the source code of scripts, run arbitrary PHP code on the server, etc.
Entries:
- archives:
  - http://www.openwall.com/lists/oss-security/2024/06/07/1
  - https://lists.fedoraproject.org/archives/list/package-announce@lists.fedoraproject.org/message/PKGTQUOA2NTZ3RXN22CSAUJPIRUYRB4B

- c:
  - https://github.com/php/php-src
- c++:
  - https://github.com/vwilzz/php-rce-4577
- go:
  - https://github.com/tam-k592/cve-2024-4577
  - https://github.com/zan8in/afrog
 
- html:
  - https://bdu.fstec.ru/vul/2024-04432
  - https://github.com/advisories/GHSA-vxpp-6299-mxw3
 

- javascript:
  - https://github.com/wy876/poc
  - https://github.com/wy876/wiki
 
 
- media:
  - https://www.youtube.com/watch?v=-59bKxwir5Q
  - https://www.youtube.com/watch?v=0KLRXDhdhMg
 
- ruby:
  - https://github.com/rapid7/metasploit-framework
  - https://raw.githubusercontent.com/rapid7/metasploit-framework/master/modules/exploits/windows/http/php_cgi_arg_injection_rce_cve_2024_4577.rb
- shell:
  - https://github.com/11whoami99/cve-2024-4577
  - https://github.com/bl4cksku11/cve-2024-4577
 
- unknown:
  - https://advisories.checkpoint.com/advisories
  - https://arstechnica.com/security/2024/06/php-vulnerability-allows-attackers-to-run-malicious-code-on-windows-servers
 
```
## Json file example
```bash
{
    "description": "Exploit Observer has 108 entries in 14 file formats related to CVE-2024-4577. In PHP versions\u00a08.1.* before 8.1.29, 8.2.* before 8.2.20, 8.3.* before 8.3.8, when using Apache and PHP-CGI on Windows, if the system is set up to use certain code pages, Windows may use \"Best-Fit\" behavior to replace characters in command line given to\u00a0Win32 API functions. PHP CGI module may misinterpret those characters as PHP options, which may allow a malicious user to pass options to PHP binary being run, and thus reveal the source code of scripts, run arbitrary PHP code on the server, etc.",
    "clusters": [
        "http://api.exploit.observer/?keyword=VEDAS:VIRIDIANVERVE"
    ],
    "entries": {
        "archives": [
            "http://www.openwall.com/lists/oss-security/2024/06/07/1",
            "https://lists.fedoraproject.org/archives/list/package-announce@lists.fedoraproject.org
        "c": [
            "https://github.com/php/php-src"
        ],
        "c++": [
            "https://github.com/vwilzz/php-rce-4577"
        ],
        "go": [
            "https://github.com/tam-k592/cve-2024-4577",
            "https://github.com/zan8in/afrog",
          
        ],
        "html": [
            "https://bdu.fstec.ru/vul/2024-04432",
            "https://github.com/advisories/GHSA-vxpp-6299-mxw3",
       
        ],
        "javascript": [
            "https://github.com/projectdiscovery/nuclei-templates"
        ],
        "markdown": [
            "https://github.com/0x20c/cve-2024-4577-nuclei",
            "https://github.com/0xmarcio/cve",
        ],
        "media": [
            "https://www.youtube.com/watch?v=-59bKxwir5Q",
            "https://www.youtube.com/watch?v=0KLRXDhdhMg",
        ],
        "python": [
             "https://www.exploit-db.com/raw/52047",
            "https://github.com/aaddmin1122345/cve-2024-4577-poc",
           
        ],
        "ruby": [
            "https://github.com/rapid7/metasploit-framework",
            "https://raw.githubusercontent.com/rapid7/metasploit-framework/master/modules/exploits/windows/http/php_cgi_arg_injection_rce_cve_2024_4577.rb"
        ],
        "shell": [
            "https://github.com/11whoami99/cve-2024-4577",
            "https://github.com/bl4cksku11/cve-2024-4577",
        ],
        "text": [
            "https://cxsecurity.com/ascii/WLB-2024060031"
        ],
        "yaml": [
            "https://raw.githubusercontent.com/projectdiscovery/nuclei-templates/main/http/cves/2024/CVE-2024-4577.yaml"
        ],
        "unknown": [
            "https://advisories.checkpoint.com/advisories",
            "https://arstechnica.com/security/2024/06/php-vulnerability-allows-attackers-to-run-malicious-code-on-windows-servers",
            
        ]
    },
    "priority": 0.5342357
}                                 
```
## 💁 References
- [**Exploit Observer**](https://api.exploit.observer)
## 📝 Todo
- [x] **~~Adding total entries~~**
- [x] **~~Adding default html report templates~~**
- [x] **~~Adding html,csv,json,docx report output~~**
- [ ] **Extending features and custom templates**


## 📌 Author
- [Facebook](https://facebook.com/l0n3m4n)
- [Twitter (X)](https://twitter.com/l0n3m4n)
- [Medium](https://medium.com/l0n3m4n)
- [Website](https://l0n3m4n.github.io)

## 👨🏾‍⚖️ License
This project is under terms of the [MIT License](LICENSE). For fixing Bugs, create [issue](https://github.com/l0n3m4n/pocfinder/issues/new)
