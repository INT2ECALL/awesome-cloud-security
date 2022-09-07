<div align="center">
    <h1>云安全</h1>
    <p>收集与云安全相关的文章和工具</p>
</div>
<br/>

# 索引

- [文章](#文章)
- [红队](#工具)
    - [红队工具](#红队工具)
- [蓝队](#查杀工具)

- [交流讨论](#交流讨论)

# 内容

## 文章

- [一文看懂内存马](https://www.freebuf.com/articles/web/274466.html)


## 内存马

### Webshell

- [memShell](https://github.com/rebeyond/memShell) - a webshell resides in the memory of java web server
- [msmap](https://github.com/hosch3n/msmap) - Msmap是一个内存马生成器，兼容多种容器、组件、编码器、WebShell / Proxy / Killer 和管理客户端
- [MemShellDemo](https://github.com/jweny/MemShellDemo) - 本项目为各类内存马的Demo合集
- [JAVA_memshells](https://github.com/minhangxiaohui/JAVA_memshells) - java 内存马系列 实现（Servlets 、组件、Agent）
- [weblogic_memshell](https://github.com/keven1z/weblogic_memshell) - 一个基于javaagent+ASM的无文件落地的javaagent，兼容多种容器(weblogic,Tomcat,Springboot)
- [java_memshell](https://github.com/kuron3k0/java_memshell) - java各中间件的内存马、回显研究
- [JSP-WebShells](https://github.com/threedr3am/JSP-WebShells) - Collect JSP webshell of various implementation methods. 收集JSP Webshell的各种姿势
- [ZhouYu](https://github.com/threedr3am/ZhouYu) - SpringBoot 持久化 WebShell
- [MemoryShell](https://github.com/su18/MemoryShell) - JavaWeb MemoryShell Inject/Scan/Killer/Protect Research & Exploring
- [MemShell](https://github.com/ax1sX/MemShell) - A List of Memory Shell related component relationships for some middleware
- [MemShell](https://github.com/veo/wsMemShell) - WebSocket Webshell，一种新型WebShell技术
- [MemShell-1](https://github.com/changheluor007/MemShell-1) - 免杀Tomcat Filter型内存马
- [memShell](https://github.com/feihong-cs/memShell) - Java memShell

### 红队工具
- [shiro_attack](https://github.com/j1anFen/shiro_attack) - 利用shiro反序列化漏洞进行回显命令执行以及注入各类内存马
- [Dr4gonSword](https://github.com/ccdr4gon/Dr4gonSword) - 内存马利用工具
- [Shiro-EXP](https://github.com/Veraxy00/Shiro-EXP) - 基于Apache Shiro反序列化漏洞进行利用链的探测，附内存马。
- [ysoserial](https://github.com/su18/ysoserial) - 支持了一键打入 Spring/Tomcat/Jetty/JBoss/Resin/Websphere 内存马功能，内存马支持命令执行、冰蝎、哥斯拉、WebSocket 四种利用方式；并支持 Tomcat 回显命令执行、Neoreg 流量隧道内存马、Tomcat Websocket 内存马、Tomcat Executor 内存马、Tomcat Upgrade 内存马、RMI 内存马等；
防御绕过：在部分系统中使用了 WAF/RASP 等防御模式，本项目去除大多数原版特征，并在执行恶意动作时使用了多种能够绕过 RASP 的执行方式，绕过防护


### Webshell管理工具
- [Behinder](https://github.com/rebeyond/Behinder) - “冰蝎”动态二进制加密网站管理客户端
- [Godzilla](https://github.com/BeichenDream/Godzilla) - 哥斯拉webshell管理工具
- [As-Exploits](https://github.com/yzddmr6/As-Exploits) - 中国蚁剑后渗透框架
## 查杀工具
- [copagent](https://github.com/LandGrey/copagent) - A java memory web shell extracting tool
- [java-memshell-scanner](https://github.com/c0ny1/java-memshell-scanner) - 通过jsp脚本扫描并查杀各类中间件内存马，比Java agent要温和一些。
- [java-memshell-scanner](https://github.com/tovd-go/java-memshell-scan) - 简单的修改了一下c0ny1师傅的代码，添加了对websocket内存马查杀的支持
- [DuckMemoryScan](https://github.com/huoji120/DuckMemoryScan) - 一个简单寻找包括不限于iis劫持,无文件木马,shellcode免杀后门的工具
- [GuanYu](https://github.com/threedr3am/GuanYu) - JVM类加载监控agent，可配置黑名单，禁止恶意类加载（包括jsp webshell）


## JVM相关工具
- [jattach](https://github.com/apangin/jattach) - The utility to send commands to a JVM process via Dynamic Attach mechanism
- [arthas](https://github.com/alibaba/arthas) - Arthas is a Java Diagnostic tool open sourced by Alibaba

# 交流讨论

欢迎关注公众号，一起交流学习。
<p align="center">
    <img src="https://s1.ax1x.com/2022/08/27/vWFPpj.png" alt="vWFPpj.png" border="0" />
</p>

