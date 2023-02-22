# Windows11 Penetration Suite Toolkit 

![image](https://img.shields.io/badge/Author-Arch3rPro-blueviolet.svg)  ![image](https://img.shields.io/badge/Release-v1.0-blue.svg)  ![image](https://img.shields.io/badge/Platform-Windows-red.svg) ![image](https://img.shields.io/badge/WSL-Kali-9cf.svg) ![image](https://img.shields.io/badge/Property-%E6%AD%A6%E5%99%A8%E5%BA%93-brightgreen.svg)

**系统简介**

- 基于Windows 11 22621.160 Pro x64 zh-cn 俄大神tatata精简版镜像制作；
- 精简系统自带软件，美化字体及部分图标，适度优化；
- 镜像硬盘使用19.7G，使用单磁盘文件存储，提升性能；（制作中，尽量精简镜像大小）
- 本环境旨在提供一个开箱即用的windows渗透测试环境；
- 致谢：本文档结构参考优秀项目 [Windows10 Penetration Suite Toolkit within Kali Linux](https://github.com/makoto56/penetration-suite-toolkit)
- 建议运行环境：
  * vmware：16.0
  * 运行内存：8G
  * 固态硬盘：100G
- 下载链接：[https://pan.baidu.com/s/1FaKre9_sH9vDmH9D8XxXfw?pwd=dg4u](https://pan.baidu.com/s/1FaKre9_sH9vDmH9D8XxXfw?pwd=dg4u)
  * 下载文件为OVA，需导入到VMware虚拟机中使用
  * `MD5 (Windows11 Penetration Suite Toolkit.ova) = b5d232657999fdbef0505bd36be49e50`
  * `Shasum -a 256 = 78193d2fbf2331380b507c8f3d72adab4dbc8d2be48e8578b38ea7bd99702c42`
  
- Release v2.0 正在制作中,版本更新内容：
  * 更新部分工具
  * 工具图标重新构建，每个工具都有对应图标
  * 加入Kali WSL，部分Linux工具使用 WSL运行
  * 添加windows Alias，命令行工具直接在windows Terminal下输入工具名称+参数即可
  
      
**系统封面**
![Desktop](./Desktop.png)  

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

**编程环境及集成开发环境：**
    
    - Python v3.10.5
         * 启动命令：python3 test.py
         * 已集成本镜像所有python3工具的依赖库
         * 使用pip3命令调用python3 pip
    - Python v2.7.18
         * 启动命令：python test.py
         * 已集成本镜像所有python2工具的依赖库
         * 使用pip命令调用python2 pip
    - Go v1.18.4
    - JRE v8u33
         * 已配置环境变量
    - Strawberry-Perl v5.32.1.1
    - Gcc v8.3.0 (由perl安装内置)
    - phpEnv v8.3.9
         * Nginx v1.18.0 默认启动
         * Apache v2.4.43 
         * PHP v7.4 
         * MySQL v5.7 默认启动
         * phpMyAdmin  v5.1.3 默认启动
    - Git v2.37.1
    - Ruby v3.1.2-1
    - Node v16.16.0

### 2. 常用软件（D:\Program Files\）：

**系统增强:**

    - 7zip：高效无损解压缩 v22.00
    - Bandizip：跨平台解压缩软件(支持暴力破解压缩密码) v7.06 （果核剥壳）
    - 卡饭输入法：拼音和五笔，纯净无广告 v1.0.0.285（果核剥壳）
    - Maye：一个简洁小巧的快速启动工具 v1.3.3
    - Clink：Windows Cmd.exe Bash样式命令行编辑工具 v0.4.9
    - uTools：Windows效率搜索工具集合 v2.6.3
    - contextmenumanager：右键菜单管理工具 v3.3.3.1
    - Everything：快速文件搜索工具(结合uTools使用体验更加) v1.4.1.1017.x64
    - Windows Terminal：（已替换默认cmd）
    - He3：开发者必备的万能工具箱

**系统优化:** 

    - HEU_KMS_Activator：全能系统数字许可激活工具 v24.6.4
    - Dism++：Windows 系统管理优化工具 v10.1.1002.1
    - WiseCare365_Pro：系统优化工具绿色修改版 v6.3.2.610（果核剥壳）
    - Autologin：Windows自动登录注册表
    - MacType：Windows字体渲染软件 v2021.1-rc1
    - icons：自制和部分Kali_2022.4提取的图标包

**文本编辑:** 

    - SublimeText：高效文本编辑器-汉化特别版 v4.4126 （果核剥壳）
    - Typora：Markdown编辑器 v1.3.8（果核剥壳）


**连接工具:** 

    - Navicat：多连数据库开发工具  v16.0.6.0 （果核剥壳）
    - NxShell：一款跨平台的SSH新终端工具 v1.6.1
    - WindTerm：专业的跨平台SSH/Sftp/Shell/Telnet/Serial终端 v2.5.0
    
### 3. 浏览器及插件 （C:\Softwares）：

    - Chrome：浏览器绿色修改版 v99.0.4844.51 （果核剥壳）
      * 主要集成插件:
        - Bishop Vulnerability Scanner:Search websites for git repos, exposed config files, and more as you browse.
        - FOFA Pro View: FOFA Pro view
        - Hack-Tools:The all in one Red team extension for web pentester
        - HackBar:HackBar for Chrome
        - Infinity: Infinity 新标签页 (Pro)
        - IP, DNS & Security Tools: Quick access to IP, DNS & Network Tools.
        - Proxy SwitchyOmega:轻松快捷地管理和切换多个代理设置。
        - funnel search：google搜索工具
        - Shodan: The Shodan plugin tells you where the website is hosted (country, city), who owns the IP and what other services/ ports are open.
        - Vulners Web Scanner：Tiny vulnerability scanner based on vulners.com vulnerability database.
        - Wappalyzer: 网页技术分析工具
        - WhatRuns: 网页技术分析工具 
        - ZoomEye Tools: ZoomEye Tools provides a variety of functions to assist the use of Zoomeye
        - Octotree: 增强 GitHub 代码审查和探索的浏览器扩展
        - PostWoman：Http接口调试插件
        - Supercopy：超级复制
     - Firefox：v91.11.0esr （已关闭自动更新）
       * 主要集成插件:
        - Infinity: Infinity 新标签页 (Pro)

**4. 渗透测试类（D:\Penetest Tools）：**
    

> 常用的Python、Perl、Ruby脚本类工具均可在Maye工具箱中点击图标进行访问
>   * 已设置默认使用Windows Terminal启动CMD.exe
>   * 已设置脚本启动目录
>   * 已安装相应的依赖
>   * 已设置脚本启动时执行Help命令
>   * 部分工具会使用git bash打开

**`[+] Information Gathering 信息收集:`**
    
    - GHDB：Google Hack 数据库搜索引擎 
    - SearchDiggity：SearchDiggity 3.1 is the primary attack tool of the Google Hacking Diggity Project
    - Katana：A Python Tool For google Hacking
    - GooFuzz：GooFuzz is a tool to perform fuzzing with an OSINT
    - Pagodo：pagodo (Passive Google Dork) - Automate Google Hacking Database scraping and searching . 
    
    - Layer：子域名挖掘机 v5.0
    - ksubdomain：无状态子域名爆破工具 v0.7
    - SubDomainsBrute：高并发的DNS暴力枚举工具 v1.4
    - Sublist3r：高并发子域名枚举工具 v1.1
    - Oneforall：功能强大的子域收集工具 v0.4.5
    - ct：简单易用的域名爆破工具 v1.0.9
    
    - SvnExploit：SVN源代码泄露全版本Dump源码
    - gitGraber：监控搜索GitHub敏感数据
    - Gitmine：Github敏感数据高级挖掘的工具 v2.0
    - GitHacker：.git文件夹利用工具 v1.1.3 
    - Gitrob：GitHub organizations 侦察工具 v2.0
    
    - Amass：信息收集、主动侦察、资产发现工具  v3.19.2
    - Spiderfoot：自动化OSINT工具
    - theHarvester：邮箱、域名探测综合OSINT工具 v4.0.3


**`[+] PortScaner 端口扫描:`**
    
    - Masscan：高并发TCP 端口扫描器 v1.3.2
    - Nmap/Zenmap：端口扫描神器（功能强大，但扫描速度偏慢）  v7.92
    - NimScan：快速端口扫描器 v1.0.8
    - TXPortMap：端口扫描和Banner识别工具 v1.1.2
    - Scaninfo：开源、轻量、快速、跨平台的红队对外网打点扫描仪 v1.1.0
    - Yujian：御剑端口扫描工具 v2020（Beta）
    - Ports_number：常见端口合集


**`[+] Web Crawlers & Directory Brute Force 目录爆破:`**
    
    - Dirbrute：多线程WEB目录爆破工具（内置字典）v1.0
    - ffuf：快速Web Fuzzing工具  v1.5.0
    - Dirbuster：多线程图形化WEB目录爆破工具 v1.0-RC
    - Dirsearch：Web路径扫描工具 v0.4.2
    - Gobuster：目录/文件, DNS、VHost爆破工具 v3.1.0  
    - WebPathBrute：Web路径暴力探测工具 v1.62

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
![Tools-Lists](./img/Tools-Lists.png)

### 工具目录
![Directory](./img/Directory.png)

### Chrome插件
![Chrome extensions](./img/Chrome%20extensions.png) 

### Burpsuite/Metasploit
![Burpsuite](./img/Burpsuite.png) 
