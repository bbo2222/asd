# Windows11 Penetration Suite Toolkit 

![image](https://img.shields.io/badge/Author-Arch3rPro-blueviolet.svg)  ![image](https://img.shields.io/badge/Release-v2.2-blue.svg)  ![image](https://img.shields.io/badge/Platform-Windows-red.svg) ![image](https://img.shields.io/badge/WSL-Kali-9cf.svg) ![image](https://img.shields.io/badge/Property-%E6%AD%A6%E5%99%A8%E5%BA%93-brightgreen.svg)
=======
**系统简介**

  - 本环境旨在提供一个开箱即用的windows渗透测试环境；
  - 本项目欢迎转载，转载时请注明原作者和原文链接:[https://github.com/arch3rPro/Pentest-Windows](https://github.com/arch3rPro/Pentest-Windows)
  - 建议运行环境：【vmware：17.0 】 /【运行内存：8G】 /【固态硬盘：100G】
  - Windows11 Penetration Suite Toolkit v2.2 (WSL) 【推荐】
    - 下载链接：https://www.123pan.com/s/q59KVv-T4Qpd.html  提取码:wpst
    - 文件大小：8.55GB，解压后：23.2GB
    - SHA256：7305DBFFF38EAAD59373C8232EB417F6E996A5E80F379D22688BAC0E7C8CA6A9

  *  Windows11 Penetration Suite Toolkit v2.2 (NoWSL) 【无WSL】
	 * 下载链接：[https://www.123pan.com/s/q59KVv-tvQpd.html](https://www.123pan.com/s/q59KVv-tvQpd.html)  提取码:wpst
	 * 文件大小：7.13 GB，解压后：17.6GB
	 * SHA256：D05F8366E1054911AAE885A61D2621786B74CC6050F55A66B90CE4EDD38CFD98
  - Windows11_22H2_22621.1776-pure 精简系统【无工具】
	* 下载链接：[https://www.123pan.com/s/q59KVv-LVApd.html](https://www.123pan.com/s/q59KVv-LVApd.html) 提取码:7jdE
	* 文件大小：2.80 GB，解压后：5.11GB
	* SHA256：49a829ed7b7bbf1f7f99d7d7e0e04bfb3c91a0092f479e26e99f91cd2ca8c48c

**版本介绍**

    1. 最新版本：v2.2 
    2. v2.2版本基于Windows11_22H2_22621.1992不忘初心精简版镜像制作；
    3. 精简系统自带软件，美化终端字体及部分图标，适度优化；
    4. 镜像系统硬盘100GB，使用单磁盘文件存储，提升性能；（更新中，尽量精简镜像大小）
    5. 工具图标已重新构建，每个工具都有对应图标；
    6. 2.1加入scoop包管理器对大部分软件和工具进行管理，支持scoop update + 工具名称进行更新；
    7. 2.2已解决scoop对脚本类工具进行管理，支持脚本类的工具使用scoop安装和更新；
    8. Windows Terminal进行优化，采用统一的主题风格和oh-my-posh进行增强；
    9. 增加openvpn、proxychains等工具，工具数量已增加至180+，后续需要新增的工具可在issue中进行提交；
    10. 2.2版本新增内网渗透工具和远程管理工具等
    11. 删除了部分已不再维护或基本不用的工具；
    12. 添加CMD Alias，命令行工具直接在CMD命令行下输入工具名称+参数即可；
    13. 添加Powershell Alias，命令行工具直接在Powershell命令行下输入工具名称+参数即可；
    14. 新增wslpp，自动监听WSL端口并映射到本地，使用empire、cobaltstrike等服务端时，请优先打开wslpp。

**v2.2 版本变化**

```
1. phpEnv改用Laragon
2. FluentSearch改用Utools
3. 新增工具清单：wireshark、mRemoteNG、WinSCP、MobaXterm、OpenSSH、Redis-cli、DBeaver、HeidiSQL、OpenVPN、WebShell、Dirdar、Dirscan、fuzzDicts、Dirxk、HashCalculator、BrowserGhost、MDUT、godoh、SharpStrike、Merlin、AsyncRAT、revshell、C3、MeterPeter、Covenant、shellter、Rustcat、Socat、Websocat、Gost、Wslpp、fscan、kscan、LadonGo、Netspy、ServerScan、Mimikatz、Kerbrute、Lazagne
4. 删除工具清单：sx、GoScan、Wfuzz、Houndsploit、Emp3r0r、Shad0w-gui
```

**版本遗留问题**

```
1. Goby不支持命令行启动，报错提示: 没有找到进程 "goby-cmd.exe"（工具箱内直接启动无影响）
2. Perl改用git自带的，未设置环境变量，使用时请运行 "D:\Base\apps\git\current\usr\bin\perl.exe"
3. 工具箱内Dirbuster目标修改为"D:\Global\apps\dirbuster\current\DirBuster.bat"(命令行内启动无影响)
```

**补充介绍**

- 具体支持的工具列表和工具是否有更新版本，请查看[https://github.com/arch3rPro/scoop-bucket](https://github.com/arch3rPro/scoop-bucket) ；
- 部分机器不支持虚拟化嵌套或者本机安装hype-v会冲突，请使用不装kali-WSL的NoWSL精简版；
- 工具默认处于初始安装状态，部分工具需要进行初始化，少量工具因为要安装插件所以手动配置了。

**系统封面v2.0**

![Desktop-v2](DeskTop-v2.png)  

**制作声明：**

    1. 所有的安装类软件均下载自软件对应的官方网站；
    2. 所有的绿色类软件均下载自果核剥壳。（https://www.ghxi.com/）；
    3. 所有的脚本类工具均下载自github。
    4. 部分授权类工具（破解版）及优秀的渗透工具来自微信公众号分享；
    5. 本项目制作的初衷是帮助渗透新手快速搭建工作环境，工欲善其事，必先利其器；
    6. 本项目由于后期调试原因可能会遗留部分本人的信息，请直接忽视；
    7. 本项目坚决不接受也从未曾接受任何形式的赞助。

**免责声明：**

    1. 本镜像仅面向合法授权的企业安全建设行为，如您需要测试本镜像的可用性，请自行搭建靶机环境；
    2. 在使用本镜像进行检测时，您应确保该行为符合当地的法律法规，并且已经取得了足够的授权；
    3. 如您在使用本镜像的过程中存在任何非法行为，您需自行承担相应后果，作者将不承担任何法律及连带责任。

## 软件及工具介绍：

### 0. 基础介绍

- 🪟：由scoop进行管理和安装，支持一键安装和更新；
- 🐧：由Kali WSL 安装和启动 ，端口监听请开启wslpp；
- 💾：脚本类工具，在Windows中启动，运行时需要的依赖包，由手工完成安装；
- 🌐：在线类安全工具，访问时需要网络，部分需要科学上网；
- 📖：离线知识库，包含密码字典、工具使用、漏洞利用、免杀教程等PDF和Markdown文件。

### 1. 编程环境及集成开发环境：

- Python v3.10.11 (D:/Base/apps/Python310) 🪟
     * 启动命令：`python3 test.py`
     * 已集成本镜像所有python3工具的依赖库
     * 使用`pip3`命令调用python3 pip
- Python v2.7.18 (D:/Base/apps/Python27) 🪟
     * 启动命令：`python2 test.py`
     * 已集成本镜像所有python2工具的依赖库
     * 使用`pip2`命令调用python2 pip
- JRE v1.8.0_381 (D:\Base\apps\liberica17-jre\current\bin)🪟 
- Perl v5.36.1 (D:\Base\apps\git\current\usr\bin\perl.exe) 🪟 
- Ruby v3.2.2  🪟
- TDM-gcc v10.3.0 (D:\Base\apps\tdm-gcc) 🪟 
- Laragon v5.0.0 (D:\Base\apps\laragon) 🪟
     * Nginx v1.14.0 
     * Apache v2.4.43 
     * PHP v5.4.9 
     * MySQL v5.1.72 
- Git v2.41.0 (D:/Base/apps/git) 🪟
- Curl v8.1.1 (D:/Base/apps/Curl/bin)  🪟
- Wget v1.21.4 (D:/Base/apps/Wget) 🪟 
- Scoop：windows包管理器 v0.3.1  (D:/Base/apps/scoop) 🪟
### 2. 常用软件：

**系统增强:**

- 7zip：一款拥有极高压缩比的开源压缩软件 🪟
- utools：多功能文件搜索启动器 🪟
  * 搜素快捷键：双击Ctrl启动
- Windows Terminal：（已替换默认cmd） 
- VMware：VMware Tools 虚拟机客户机操作系统性能并改善虚拟机管理的实用工具 
- Oh-My-Posh：全平台终端提示符个性化工具  🪟 
- Clink：Windows Cmd.exe Bash样式命令行编辑工具  (D:/Base/apps/Clink)  🪟 
- Doskey (D:/Program Files/Tools/Scripts/alias_key.bat) 💾
    * alias_key.bat 文件定义了所有宏
    * 已设置注册表，开机自动设置命令alias

**系统优化:** 

- AAct：Windows激活工具 v4.2.8 Portable 
- Dism++：Windows 系统管理优化工具  🪟 
- WiseCare365：系统优化工具绿色修改版 v6.5.1_Pro（果核剥壳）
- Tools：自定义小工具 
  * 右键管理：一键设置WIN10/WIN11右键模式 💾
  * Autologin：Windows自动登录注册表 💾
  * ClearHistory.ps1: 一清除PowerShell历史记录 💾
  * Scripts：cmd 和 powershell 别名脚本 💾

**文本编辑:** 

- SublimeText：高效文本编辑器-汉化特别版 v4.4150 （果核剥壳） 

**服务连接:** 

- mRemoteNG: 标签式、多协议的远程连接管理器 🪟
- WinSCP: 支持SSH的SCP文件传输软件🪟
- MobaXterm: 工作在Windows桌面环境的多合一远程管理工具，包括几乎所有常用的远程网络工具（SSH、X11、RDP、VNC等）和Unix命令（bash、ls、cat，sed、grep、awk、rsync等 🪟
- Telnet: 实用的远程连接命令，采用的是TCP/IP协议 🪟
- OpenSSH:  包含一系列组件和工具，提供安全且简单的远程系统管理方法【启动命令：ssh】 🪟
- Redis-cli: Redis命令行界面，允许向Redis发送命令、并直接从终端读取服务器发送的回复的简单的程序 【客户端：redis-cli】【服务端：redis-server】🪟
- DBeaver: 一个通用的数据库管理工具和SQL 客户端，几乎支持所有主流的数据库 🪟
- HeidiSQL:  免费开源的轻量级数据库客户端软件，拥有图形化界面支持访问MySQL、MariaDB 和SQL Server 🪟
- OpenVPN: 一款基于SSL的开源VPN软件 🪟
- WindTerm：专业的跨平台SSH/Sftp/Shell/Telnet/Serial终端  🪟 

**浏览器及插件：**

- Chrome：已设置为默认浏览器 v116.0.5845.180
       **主要集成插件:**
  
    - Bishop Vulnerability Scanner:Search websites for git repos, exposed config files, and more as you browse.
    - Country Flags & IP Whois：显示网站服务器位置的国旗、Whois 和地理信息
    -  FOFA Pro View: FOFA Pro view
    -  Funnel Search：Advance search operators for google search
    -  Hack-Tools: The all in one Red team extension for web pentester
    -  HackBar: A browser extension for Penetration Testing
    -  IP, DNS & Security Tools: Quick access to IP, DNS & Network Tools.
    - Proxy SwitchyOmega:轻松快捷地管理和切换多个代理设置。
    - Shodan: The Shodan plugin tells you where the website is hosted (country, city), who owns the IP and what other services/ ports are open.
    - Vulners Web Scanner：Tiny vulnerability scanner based on vulners.com vulnerability database.
    - Wappalyzer: 网页技术分析工具
    - WhatRuns: 网页技术分析工具 
    - ZoomEye Tools: ZoomEye Tools provides a variety of functions to assist the use of Zoomeye
    - Octotree: 增强 GitHub 代码审查和探索的浏览器扩展
    - PostWoman：Http接口调试插件
 - Firefox：v117.0 便携版 
   
    ​	**主要集成插件:**
    
    - Country Flags & IP Whois：显示网站服务器位置的国旗、Whois 和地理信息
    - FOFA Pro View: FOFA Pro view
    - Hack-Tools:The all in one Red team extension for web pentester
    - HackBar：A HackBar for google chrome/firefox browser. Small tool for pentesting websercurity.
    - Octotree: 增强 GitHub 代码审查和探索的浏览器扩展
    - Proxy SwitchyOmega:轻松快捷地管理和切换多个代理设置。
    - Shodan: The Shodan plugin tells you where the website is hosted (country, city), who owns the IP and what other services/ ports are open.
    - Supercopy：超级复制
    - Vulners Web Scanner：Tiny vulnerability scanner based on vulners.com vulnerability database.
    - Wappalyzer: 网页技术分析工具

### 3. Maye启动器

```
- Maye：Windows快速启动工具，多文件拖拽添加启动、快捷键呼出、自动多列显示、lnk文件解析
- icon：应用图标集合，新增作者自制图标
- Kali-png：Kali Linux 2022.4 提取的应用图标库
```

### 4. 渗透测试类 ：

> 180+ 常用的脚本、图形化工具均可在Maye工具箱中点击图标进行访问
> 
>  * 已设置默认使用Windows Terminal启动CMD.exe
>   * 已设置脚本类工具Alias，使用工具名称+参数即可
>   * 已设置脚本启动目录
>   * 已安装相应的依赖
>   * 已设置脚本启动时执行Help命令
>   * 部分工具会使用Kali WSL打开


**`[+] Information Gathering 信息收集:`**

- Whois: 收集网络注册,注册域名,IP地址和系统的信息 🪟
- DnsX：多用途DNS工具包 v1.1.2 🪟
- Cewl:可指定URL地址和爬取深度并生成字典文件 🪟
- Layer：子域名挖掘机 v5.0 🪟
- Oneforall：功能强大的子域收集工具 v0.4.5 🪟
- Subfinder：高并发的DNS暴力枚举工具 v2.5.5 🪟
- ct：简单易用的域名爆破工具 v1.0.9 🪟
- ksubdomain：无状态子域名爆破工具 v1.9.5 🪟
- Amass：信息收集、主动侦察、资产发现工具  v3.19.2🪟
- SearchDiggity：SearchDiggity is the primary attack tool of the Google Hacking Diggity Project v3.1 🪟
- Gobuster：目录/文件, DNS、VHost爆破工具 v3.1.0 🪟
- GHDB：Google Hack 数据库搜索引擎 🌐
- GooFuzz：GooFuzz is a tool to perform fuzzing with an OSINT v1.2.2 🪟
- Pagodo：pagodo (Passive Google Dork) - Automate Google Hacking Database scraping and searching .  v2.4.0 🪟
- Google-Dorks:Web安全和漏洞查找相关的Google Dorks集合📄
- GitHacker：.git文件夹利用工具 v1.1.7 🪟
- gitGraber：监控搜索GitHub敏感数据 🪟
- Gitrob：GitHub organizations 侦察工具 v2.0🪟
- Gitminer：Github敏感数据高级挖掘的工具 v2.0🪟
- SvnExploit：SVN源代码泄露全版本Dump源码🪟

**`[+] PortScaner 端口扫描:`**

- Nmap/Zenmap：端口扫描神器（功能强大，但扫描速度偏慢）  v7.92 🪟
- Masscan：高并发TCP 端口扫描器 v1.3.2 🪟
- Goby:端口扫描、资产收集、漏洞利用综合工具 v2.0.5 Beta 🪟
- NimScan：快速端口扫描器 v1.0.8 🪟
- TXPortMap：端口扫描和Banner识别工具 v1.1.2 🪟
- Scaninfo：开源、轻量、快速、跨平台的红队对外网打点扫描仪 v1.1.0 🪟
- Yujian：御剑端口扫描工具 v2020（Beta）🪟
- Naabu：用Go编写的快速端口扫描器，稳定、简单易用 v2.1.1 🪟

**`[+] Web Applications 代理抓包:`**

- Broxy：用Go编写的HTTP/HTTPS开源拦截代理 v1.0.0-alpha 🪟
- Burpsuite：Web应用程序测试的最佳工具之一🪟
- Hetty：用于安全研究的HTTP工具包。 v0.7.0 🪟
- Mitmproxy：一款支持 SSL的HTTP代理 v9.0.1 🪟
- Yakit：一个高度集成化的 Yak 语言安全能力的安全测试平台🪟
- Wireshark: 非常流行的网络封包分析软件，可以截取各种网络数据包，并显示数据包详细信息🪟

**`[+] Vulnerability Scaner 漏洞扫描:`**

- wpscan：Wordpress漏洞扫描器  v3.8.33 🐧
- Nuclei：一款注重于可配置性、可扩展性和易用性的基于模板的快速漏洞扫描器 v2.8.9 🪟
- Nikto:基于perl语言开发的web页面扫描器 v2.1.6 🪟
- Xray：一款强大的web漏洞扫描工具 v1.9.3 🪟
- Xray-GUI:Super-xray图形化漏洞扫描工具，xray的UI v1.5 🪟
- Vscan：开源- 快速、跨平台的网站漏洞扫描工具 v2.0.7
- SiteScan:一站化解决渗透测试信息收集任务 v1.4 🪟
- Scaninfo：开源、轻量、快速、跨平台的红队对外网打点扫描仪 v1.1.0 🪟
- Wapiti3:Web应用程序漏洞检查工具 v3.1.6 🪟
- OSV-Scanner：谷歌开源漏洞扫描器 v1.1.0 【启动命令：osvscanner】🪟
- Afrog：一款快速稳定 PoC可定制化的漏洞扫描器 v2.2.1🪟
- Netsparker：综合型的web应用安全漏洞扫描工具 v22.12 🪟

**`[+] CMS & Framwork Identification 指纹识别:`**

- WhatWeb：下一代Web应用扫描器 v0.5.5 🪟
- WhatCMS：在线识别目标站点CMS类别和版本 🌐
- CMSeek：CMS检测和利用工具,支持WordPress、Joomla、Drupal等180个CMS v1.1.3 🪟
- Ehole：红队重点攻击系统指纹探测工具 v3.0 🪟
- ObserverWard：跨平台社区网页指纹识别工具 v2023.2.24🪟
- 云悉：在线指纹识别网站 🌐
- TideFinger：指纹识别工具，汲取整合了多个网页指标库 v1.1.0 🪟
- 360Finger-P：360在线指纹识别网站 🌐

**`[+] Webshell管理工具：`**

- Antsword：蚁剑 v2.1.15 🪟
- Behinder：冰蝎 v4.0.6（shell密码统一为rebeyond）🪟
- Bantam:PHP shell管理工具🪟
- Skyscorpion：天蝎 v1.0 （shell默认密码统一为sky）🪟
- Godzilla：哥斯拉 v4.0.1（密码为默认pass + key）🪟
- Weevely3：webshell管理工具 v4.0.1 (已安装pyreadline3取代readline依赖)🪟
- PyShell：Python版Shell管理工具 (已安装pyreadline3取代readline依赖) 🪟
- Awesome-shells：webshell收集项目，自行甄别后门 🪟
- WebShell: github上的webshell收集项目，自行甄别后门 🪟

**`[+] Web Crawlers & Directory Brute Force 目录爆破:`**

- ffuf：快速Web Fuzzing工具  v1.5.0 🪟
- Dirbuster：多线程图形化WEB目录爆破工具 v1.0-RC 🪟
- Dirsearch：Web路径扫描工具 v0.4.2 🪟
- Gobuster：目录/文件, DNS、VHost爆破工具 v3.1.0 🪟
- WebPathBrute：Web路径暴力探测工具 v1.62 🪟
- Dirb：dirb是一个基于字典的web目录扫描工具 v2.22 🐧
- Dirmap：一个高级web目录、文件扫描工具，功能将会强于DirBuster、Dirsearch、cansina、御剑 v1.0 🪟
- httpx：HTTPX是Python3的功能齐全的HTTP客户端🪟
- Dirdar：搜索（403-Forbidden）目录以破坏它并获取其上的目录列表的工具 🪟
- Dirscan：一款多线程高并发目录扫描工具 🪟
- fuzzDicts: Web渗透测试Fuzz字典 🪟
- Dirxk: 一款集成了多种老牌工具字典的轻量级目录扫描器 🪟

**`[+] Password Attack 密码破解:`**

- Hydra：一款非常强大的暴力破解工具  🪟
- Medusa：速度快，支持大规模并行，模块化，爆破登陆，可以同时对多个主机，用户或是密码执行强力测试🐧
- Hashcat：基于GPU的Hash密码破解工具  🪟
- John：一个快速的密码破解工具，用于在已知密文的情况下尝试破解出明文的破解密码软件，支持大多数的加密算法 🪟
- Johnny：图形化John the Ripper 客户端 🪟
- Psudohash：一个用于编排暴力攻击的密码列表生成器 🪟
- HashCalculator：哈希值批量计算/校验工具🪟
- BrowserGhost：一个抓取浏览器密码的工具 🪟
- HackBrowserData：一款可全平台运行的浏览器数据导出解密工具 🪟
- SecLists: 渗透测试人员密码字典表|fuzz|payload|shell  📖 🪟
- Wordlists：真实世界的信息安全字典 📖 🪟
- Weakpasss：在线暴力破解彩虹字典库，提供各种字典下载 🌐

**`[+] Vulnerability Search 漏洞查找:`**

- SPLOITUS：在线漏洞和黑客工具搜索引擎 🌐
- SearchSploit：一个用于Exploit-DB的命令行搜索工具,可以帮助我们查找渗透模块 🪟
- OSV： Google开源的在线漏洞库🌐
- Vulners：在线漏洞安全情报搜索引擎 🌐
- Getsploit：Vulners数据库的命令行搜索和下载工具（需自行注册输入API Key）💾

**`[+] Pentest Framework 渗透框架:`**

- Metasploit：模块化漏洞利用框架  🪟
- Yakit：一个高度集成化的 Yak 语言安全能力的安全测试平台 🪟
- Pocsuite3：开源的远程漏洞测试框架 💾
- Poc-T：渗透测试插件化并发框架 🪟
- MYExploit：OA类产品漏洞利用工具🪟
- Empire：一款针对Windows平台的、使用Powershell脚本作为攻击载荷的渗透攻击框架工具🐧
- Starkiller：Empire图形化界面工具，利用其RESTful API功能完成对Empire使用，方便渗透测试人员的使用🌐
  * 默认账号：empireadmin 默认密码：password123
  * 服务端empire开启前，请使用wslpp命令开启端口转发
- Cobaltstrike：一款商业化的渗透测试利器-CS 🪟
- Teamserver：CobaltStrike团队服务器 🐧
  * 默认账号：neo 默认密码：password
  * 服务端开启前请使用wslpp命令开启端口转发
  * 请修改客户端host访问地址为 localhost IP地址

**`[+] ExploitationTools 漏洞利用工具:`**

- Beef-XSS：非常强大的浏览器漏洞利用框架 🐧
  * 默认账号：beef 默认密码：beef-xss
  * 配置文件：/etc/beef-xss/config.yaml
- Bluelotus: php编写的XSS漏洞利用平台 💾
  * 默认密码：bluelotus
  * 请先启动laragon,再进行访问
- XSStrike：一款检测Cross Site Scripting的高级检测工具 v3.1.5 🪟
- XSSor2： XSS漏洞利用辅助工具 🪟
- PwnXSS：XSS漏洞扫描利用工具 🪟
- Dalfox：一款开源xss漏洞扫描器 v2.8.2 🪟
- SQLmap：自动化SQL注入工具 v-1.6.8-1 🪟
- SuperSQLInjection: 超级SQL注入工具 V1.0.20201214 🪟
- NoSQLmap：NoSQL数据库漏洞利用工具 v0.7 🪟
- Advanced-SQL-Injection-Cheatsheet：SQL注入的高级查询备忘单📖 🪟
- SQL-Injection-Payload-List：SQL注入Payload清单📖 🪟
- Commix： 自动化命令注入漏洞利用工具 🪟
- Shellfire：命令注入漏洞的漏洞利用工具，适用于 LFI、RFI、SSTI 等 v0.11💾
- LFISuite：本地文件包含漏洞利用工具 v1.13🪟
- Fuxploider: 文件上传漏洞扫描利用工具 v1 🪟
- XXEinjector: 自动化XXE漏洞利用工具🪟
- Ysomap:  Java 反序列化利用框架 v0.1.3 2022.04.15🪟
- MDUT: 数据库漏洞利用工具 🪟

**`[+] Maintaining Access 权限维持:`**

- PrintMyShell: 自动生成各种反向 shell 的python脚本 💾
- Girsh: 自动启动全交互式的反向Shell🪟
- NatPass: 主机管理工具，支持web shell和web桌面主机管理工具，支持web shell和web桌面 🪟
- Platypus: 🔨用 go 编写的现代多反向 shell 会话管理器 🪟
- Reverse_SSH: 基于SSH反向Shell管理工具🪟
- Govenom: Generate MSFVenom shells in command line :) 🪟

**`[+] Command and Control 命令控制:`**

- phpsploit:  php远程控制框架，旨在通过HTTP在客户端和web服务器之间提供一个隐蔽的交互式shell连接_🐧
- Sliver: 通用的跨平台植入型框架，支持 C2 over Mutual-TLS, HTTP(S) 和 DNS🪟
- godoh： A DNS-over-HTTPS C2🪟
- SharpStrike: 基于C#实现的后渗透漏洞利用研究工具 🪟
- Merlin: 基于Go语言开发的RAT 软件 🪟
- AsyncRAT: 开源远程管理工具 🪟
- revshell: 基于Go语言的反弹Shell命令生成工具 🪟
- C3: 自定义命令和控制，用于自定义 C2 通道快速原型设计的框架  🪟
- MeterPeter：具有内置命令的 C2 Powershell 命令和控制框架 🪟
- Covenant: .NET开发的C2(command and control)框架 🪟

**`[+] Bypass AV 免杀远控:`**

- AV_Evasion_Tool： 掩日 - 免杀执行器生成工具 v20230417 🪟
- ShellCodeLoader： windows 的 ShellcodeLoader v1.0  🪟
- BypassAntiVirus：远程控制防杀系列文章及配套工具📖🪟
- MazteuszEx：bypass AV生成工具 v1.0 🪟📅 
- shellter: 动态shellcode 注入工具 🪟

**`[+] Privilege Escalation Auxiliary 提权辅助:`**

- GFOBins: 一个精选的 Unix 二进制文件列表，可用于绕过错误配置系统中的本地安全限制 🌐
- LOLBAS:  在 Windows 机器上使用二进制文件查找可能的权限提升路径 🌐
- WADComs: 一个交互式备忘单，包含精选的攻击性安全工具列表及其各自的命令，用于针对 Windows/AD 环境 🌐
- Hijack Libs: 在线DLL 劫持库精选列表 🌐
- GTFOBLookup: [GTFOBins](https://gtfobins.github.io/)、[LOLBAS](https://lolbas-project.github.io/)、[WADComs](https://wadcoms.github.io/)和[HijackLibs](https://hijacklibs.net/)的离线命令行查找实用程序 🪟
- Linux-exp-Suggester: Linux内核提权漏洞查询工具，perl脚本 🪟
- Win-Kernel-EXP: Windows-kernel-exploits Windows平台提权漏洞集合 🪟
- Lin-Kernel-EXP: Linux-kernel-exploits Linux平台提权漏洞集合  📖🪟
- BeRoot:  Windows / Linux / Mac本地提权工具  v1.0.1 🪟
- WinPEAS: 在 Windows 环境中搜索可能的权限提升路径，需要目标系统（.Net >= 4.5.2）环境 v20230514-85dabdc9  🪟
- LinPEAS: 无需任何依赖的脚本，使用/bin/sh语法，用于搜索在 Linux/Unix*/MacOS 主机上搜索可能的权限提升路径 📖🪟
- PrintNotifyPotato: 又一个土豆，使用PrintNotify COM服务进行提权 v1.0.0  🪟

**`[+] Port Forwarding & Proxies 端口转发:`**

- Termite: 经典的隧道代理工具🪟
- Frps: 快速反向代理，可帮助您将 NAT 或防火墙后面的本地服务器暴露给互联网🪟
- NPS: 轻量级、高性能、强大的内网穿透代理服务器，带有强大的web管理终端🪟
- GoProxy: Go语言开发的高性能、全功能、跨平台的代理服务器🪟
- reGeorg: reDuh的继承者，通过DMZ创建 SOCKS 代理🪟
- Neoreg: reGeorg重构版本🪟
- Venom: 渗透测试多层代理跳板工具🪟
- Stowaway: 又一个渗透测试的多跳代理工具🪟
- Rportd: 远程管理工具，支持多级代理🪟
- PortForward: Golang 开发的端口转发工具🪟
- Proxychains：命令行代理工具，windows版本🪟
- Rustcat： 一款功能强大的端口监听工具🪟
- Socat: 多用途双向套接字数据转接工具🪟
- Netcat：一款强大的命令行网络工具，建立TCP/UDP连接 【启动命令：nc】 🪟 
- Websocat: 用于WebSocket的命令行客户端🪟
- Gost: 功能多样且实用的安全隧道工具🪟
- Wslpp: 用于从 wsl2 linux 到 windows 的代理端口的 TCP 解决方法工具🪟

**`[+] 内网渗透`**

- fscan: 一键自动化、全方位漏洞扫描的开源工具 🪟 
- kscan: 轻量级的资产发现工具，可针对IP/IP段或资产列表进行端口扫描以及TCP指纹识别和Banner抓取 🪟 
- LadonGo: 大型内网渗透的多线程插件化综合扫描神器 🪟 
- Netspy: 快速探测内网可达网段工具 🪟 
- ServerScan:  使用Golang开发的高并发网络扫描 🪟 
- Mimikatz:  一款功能强大的轻量级调试神器 🪟 
- Kerbrute:  一套用于对域名进行侦察的工具 🪟 
- Lazagne:  一键抓取目标机器上的所有明文密码的神器 🪟 

**系统截图**

### 工具列表
![Tools-Lists](./img/常用工具.png)

### 工具目录
![Directory](./img/工具目录.png)

### Chrome插件
![Chrome extensions](./img/Chrome%20extensions.png) 

### Burpsuite/Metasploit
![Burpsuite](./img/Burpsuite.png) 

### Empire\Starkiller

![Empire](./img/Empire.png)

### Netsparker

![Invicti](./img/Invicti.png)

### Yakit

![Yakit](./img/Yakit.png)

### Goby

![Goby](./img/Goby.png)

