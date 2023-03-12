# Windows11 Penetration Suite Toolkit 

![image](https://img.shields.io/badge/Author-Arch3rPro-blueviolet.svg)  ![image](https://img.shields.io/badge/Release-v1.0-blue.svg)  ![image](https://img.shields.io/badge/Platform-Windows-red.svg) ![image](https://img.shields.io/badge/WSL-Kali-9cf.svg) ![image](https://img.shields.io/badge/Property-%E6%AD%A6%E5%99%A8%E5%BA%93-brightgreen.svg)

**系统简介**

- 系统介绍
  - 本环境旨在提供一个开箱即用的windows渗透测试环境；
  - 致谢：本文档结构参考优秀项目 [Windows10 Penetration Suite Toolkit within Kali Linux](https://github.com/makoto56/penetration-suite-toolkit)
- Release v2.0-Pre 版本介绍：
  * 基于Windows11_22H2_22621.1250不忘初心精简版镜像制作；
  * 精简系统自带软件，美化字体及部分图标，适度优化；
  * 镜像硬盘使用22.8G，使用单磁盘文件存储，提升性能；（制作中，尽量精简镜像大小）
  * 2.0版本更新部分工具，并进行工具图标重新构建，每个工具都有对应图标；
  * 2.0版本加入了Kali WSL，部分Linux工具使用 WSL运行；
  * 添加windows Alias，命令行工具直接在windows Terminal下输入工具名称+参数即可；
  * 下载链接：[https://www.123pan.com/s/q59KVv-iWApd.html](https://www.123pan.com/s/q59KVv-iWApd.html)提取码:j3KA
- 建议运行环境：
  * vmware：17.0
  * 运行内存：8G
  * 固态硬盘：100G

**系统封面v2.0**
![Desktop-v2](./DeskTop-v2.png)  

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

### 1. 编程环境及集成开发环境（D:\Base\）：

    - Python v3.10.10 (D:\Base\Python3)
         * 启动命令：python3 test.py
         * 已集成本镜像所有python3工具的依赖库
         * 使用pip3命令调用python3 pip
    - Python v2.7.13 (D:\Base\Python)
         * 启动命令：python test.py
         * 已集成本镜像所有python2工具的依赖库
         * 使用pip命令调用python2 pip
    - JRE v8u33 (D:\Base\Java\bin)
         * 已配置环境变量
    - Perl v5.36.0 （WIndows下使用频率不高，perl脚本用WSL运行）
    - Gcc v12.2.0 (由WSL安装内置)
    - phpEnv v8.3.9 (D:\Base\phpEnv\bin)
         * Nginx v1.18.0 默认启动
         * Apache v2.4.43 
         * PHP v7.4 
         * MySQL v5.7 默认启动
         * phpMyAdmin  v5.1.3 默认启动
    - Git v2.39.0 (D:\Base\Git)
    - Ruby v3.1.2p20 （WIndows下使用频率不高，ruby脚本用WSL运行）
    - Node v16.16.0 (D:\Base\Node)
    - Doskey (D:\Base\Alias)
    	 * D:\Base\Alias\alias_key.bat 文件定义了所有宏
    	 * 已设置注册表，开机自动设置命令alias
    - Curl v7.83.1 (D:\Base\Curl\bin)
    - Wget v1.21.3 (D:\Base\Wget)
    - Clink：Windows Cmd.exe Bash样式命令行编辑工具 v1.4.21.b59b76 (D:\Base\Clink)

### 2. 常用软件（D:\Program Files\）：

**系统增强:**

    - Bandizip：跨平台解压缩软件(支持暴力破解压缩密码) v7.30（果核剥壳）
    - FluentSearch：工作流、文件搜索启动器 v0.9.91.9995
    	 * 搜素快捷键：双击Ctrl启动
    - Windows Terminal：（已替换默认cmd）
    - VMware：VMware Tools 虚拟机客户机操作系统性能并改善虚拟机管理的实用工具

**系统优化:** 

    - AAct：Windows激活工具 v4.2.8 Portable
    - Dism++：Windows 系统管理优化工具 v10.1.1001.10
    - WiseCare365：系统优化工具绿色修改版 v6.5.1_Pro（果核剥壳）
    - Tools：自定义小工具
    	 * 右键管理：一键设置WIN10/WIN11右键模式
    	 * Autologin：Windows自动登录注册表
    	 * JDK环境变量配置脚本：一键设置JDK环境变量，需要修改reg文件内的目录

**文本编辑:** 

    - SublimeText：高效文本编辑器-汉化特别版 v4.4145 （果核剥壳）
    - Typora：Markdown编辑器 v1.4.8（果核剥壳）

**连接工具:** 

    - Navicat：多连数据库开发工具  v16.0.6.0 （果核剥壳）
    - NxShell：一款跨平台的SSH新终端工具 v1.6.1
    - WindTerm：专业的跨平台SSH/Sftp/Shell/Telnet/Serial终端 v2.6.0

**浏览器及插件：**

    - Chromium：BurpSuite内置提取版 v109.0.5414.120
      * 主要集成插件:
        - Bishop Vulnerability Scanner:Search websites for git repos, exposed config files, and more as you browse.
        - FOFA Pro View: FOFA Pro view
        - Funnel Search：Advance search operators for google search
        - Hack-Tools:The all in one Red team extension for web pentester
        - HackBar:HackBar for Chrome
        - IP, DNS & Security Tools: Quick access to IP, DNS & Network Tools.
        - Proxy SwitchyOmega:轻松快捷地管理和切换多个代理设置。
        - Shodan: The Shodan plugin tells you where the website is hosted (country, city), who owns the IP and what other services/ ports are open.
        - Vulners Web Scanner：Tiny vulnerability scanner based on vulners.com vulnerability database.
        - Wappalyzer: 网页技术分析工具
        - WhatRuns: 网页技术分析工具 
        - ZoomEye Tools: ZoomEye Tools provides a variety of functions to assist the use of Zoomeye
        - Octotree: 增强 GitHub 代码审查和探索的浏览器扩展
        - PostWoman：Http接口调试插件
     - Firefox：v91.11.0esr （已关闭自动更新）
       * 主要集成插件:
        - Country Flags & IP Whois：Displays country flag of website's server location, Whois and Geo info
        - FOFA Pro View: FOFA Pro view
        - Hack-Tools:The all in one Red team extension for web pentester
        - HackBar：A HackBar for google chrome/firefox browser. Small tool for pentesting websercurity.
        - Octotree: 增强 GitHub 代码审查和探索的浏览器扩展
        - Proxy SwitchyOmega:轻松快捷地管理和切换多个代理设置。
        - Shodan: The Shodan plugin tells you where the website is hosted (country, city), who owns the IP and what other services/ ports are open.
        - Supercopy：超级复制
        - Vulners Web Scanner：Tiny vulnerability scanner based on vulners.com vulnerability database.
        - Wappalyzer: 网页技术分析工具

### 3. Maye启动器（D:\Maye\）

```
- Maye：Windows快速启动工具，多文件拖拽添加启动、快捷键呼出、自动多列显示、lnk文件解析
- icon：应用图标集合，新增作者自制图标
- Kali-png：Kali Linux 2022.4 提取的应用图标库
```

### 4. 渗透测试类 （D:\Penetest Tools）：

> 137+ 常用的脚本、图形化工具均可在Maye工具箱中点击图标进行访问
>
>   * 已设置默认使用Windows Terminal启动CMD.exe
>   * 已设置脚本类工具Alias，使用工具名称+参数即可，具体命令可参考（D:\Base\Alias\alias_key.bat）
>   * 已设置脚本启动目录
>   * 已安装相应的依赖
>   * 已设置脚本启动时执行Help命令
>   * 部分工具会使用Kali WSL打开

**`[+] Information Gathering 信息收集:`**
    

    - Whois: 收集网络注册,注册域名,IP地址和自治系统的信息 【WSL启动】
    - DnsX：多用途DNS工具包 v1.1.2
    - Layer：子域名挖掘机 v5.0
    - ksubdomain：无状态子域名爆破工具 v1.9.5
    - Subfinder：高并发的DNS暴力枚举工具 v2.5.5
    - Oneforall：功能强大的子域收集工具 v0.4.5
    - ct：简单易用的域名爆破工具 v1.0.9
    - Gobuster：目录/文件, DNS、VHost爆破工具 v3.1.0  
    
    - GHDB：Google Hack 数据库搜索引擎
    - SearchDiggity：SearchDiggity is the primary attack tool of the Google Hacking Diggity Project v3.1
    - Katana：A Python Tool For google Hacking v1.5.3 【启动命令：kds】
    - GooFuzz：GooFuzz is a tool to perform fuzzing with an OSINT v1.2.1 【WSL启动】
    - Pagodo：pagodo (Passive Google Dork) - Automate Google Hacking Database scraping and searching .  v2.4.0
    - Google-Dorks:Web安全和漏洞查找相关的Google Dorks集合
    
    - SvnExploit：SVN源代码泄露全版本Dump源码
    - gitGraber：监控搜索GitHub敏感数据
    - Gitminer：Github敏感数据高级挖掘的工具 v2.0
    - GitHacker：.git文件夹利用工具 v1.1.7
    - Gitrob：GitHub organizations 侦察工具 v2.0
    - GitGot：半自动化、反馈驱动的工具，可快速搜索 GitHub 上的大量公共数据以查找敏感机密。
    
    - Amass：信息收集、主动侦察、资产发现工具  v3.19.2
    - Spiderfoot：自动化OSINT工具
    - theHarvester：邮箱、域名探测综合OSINT工具 v4.0.3

**`[+] PortScaner 端口扫描:`**
    

    - Nmap/Zenmap：端口扫描神器（功能强大，但扫描速度偏慢）  v7.92
    - Masscan：高并发TCP 端口扫描器 v1.3.2
    - Goby:端口扫描、资产收集、漏洞利用综合工具 1288Poc版本
    - NimScan：快速端口扫描器 v1.0.8
    - TXPortMap：端口扫描和Banner识别工具 v1.1.2
    - Sx:快速、现代、易于使用的网络扫描仪 v0.5.0 【WSL启动】
    - Scaninfo：开源、轻量、快速、跨平台的红队对外网打点扫描仪 v1.1.0
    - GoScan:交互式网络扫描仪 v2.4 【WSL启动】
    - Yujian：御剑端口扫描工具 v2020（Beta）
    - Naabu：用Go编写的快速端口扫描器，稳定、简单易用 v2.1.1

**`[+] Web Crawlers & Directory Brute Force 目录爆破:`**
    

    - Dirbrute：多线程WEB目录爆破工具（内置字典）v1.0
    - ffuf：快速Web Fuzzing工具  v1.5.0
    - Dirbuster：多线程图形化WEB目录爆破工具 v1.0-RC
    - Dirsearch：Web路径扫描工具 v0.4.2
    - Gobuster：目录/文件, DNS、VHost爆破工具 v3.1.0  
    - WebPathBrute：Web路径暴力探测工具 v1.62
    - Cewl:可指定URL地址和爬取深度并生成字典文件

**`[+] ExploitationTools 漏洞利用工具:`**
    
    - Metasploit：模块化漏洞利用框架 v6.2.7+20220714153328-1rapid7
    - ExploitPack：多平台漏洞利用框架 v15.07 PRO (已修改hosts关闭强制更新)
    - MYExploit：OA类产品漏洞利用工具
    
    - Sploitus：在线漏洞利用工具搜索引擎
    - GetSploit：vulners官方搜索工具（需自行注册输入API Key）
    - Searchsploit:Exploit-DB官方搜索工具（已修改使用git-bash启动，windows可用）
    - ExploitDBHelper: 图形化Exploit-DB搜索工具（已手动更新exploit.csv文件至2022/04/22版本）
    - HoundSploit: Exploit-DB 的高级图形化搜索引擎(点击图标启动服务，浏览器打开链接访问)
    - Xplfinder: 简单版searchsploit 
    
    - SQLmap：自动化SQL注入工具 v-1.6.8-1
    - SuperSQLInjection: 超级SQL注入工具 V1.0.20201214
    - NoSQLmap：NoSQL数据库漏洞利用工具 v0.7
    - Advanced-SQL-Injection-Cheatsheet：SQL注入的高级查询备忘单
    - SQL-Injection-Payload-List：SQL注入Payload清单


**`[+] Webshell管理工具`**
    

    - Antsword：蚁剑（已集成插件）v2.1.15（https://github.com/AntSwordProject/AntSword-Loader）
    - Behinder：冰蝎 v4.0（https://github.com/rebeyond/Behinder）
      * 添加server文件夹 （shell密码统一为rebeyond）
    - Skyscorpion：天蝎（shell默认密码统一为sky）（https://github.com/shack2/skyscorpion）
    - Godzilla：哥斯拉 v4.0.1（密码为默认pass + key）（https://github.com/BeichenDream/Godzilla）
    - Caidao：中国菜刀 v20160620 (默认密码caidao）
    - Weevely3：webshell管理工具 v4.0.1 (已安装pyreadline3取代readline依赖)(https://github.com/epinna/weevely3)
    - Pyshell：python版shell管理工具 (已安装pyreadline3取代readline依赖) （https://github.com/JoelGMSec/PyShell）
    - Awesome-shells：webshell收集项目，自行甄别后门 （https://github.com/abhinavprasad47/Awsome-shells）

**`[+] 其他工具清单整理中...`**

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
