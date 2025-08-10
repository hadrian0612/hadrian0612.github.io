---
title: Linux syntex
date: 2025-08-10 17:55:00 +0800
categories: [syntex]
tags: [Linux]     # TAG names should always be lowercase
---

# Linux 常用命令指南

以下是50条Linux系统中最常用的命令，包含其英语全称、功能说明和用法示例

## 文件与目录操作

1. **ls**
   - 英语全称：List
   - 功能：列出目录内容
   - 示例：`ls -l`（详细列出当前目录文件）、`ls /home`（列出/home目录内容）

2. **cd**
   - 英语全称：Change Directory
   - 功能：切换工作目录
   - 示例：`cd /usr/local`（切换到/usr/local目录）、`cd ~`（切换到用户主目录）

3. **pwd**
   - 英语全称：Print Working Directory
   - 功能：显示当前工作目录的绝对路径
   - 示例：`pwd`（输出当前所在目录）

4. **mkdir**
   - 英语全称：Make Directory
   - 功能：创建新目录
   - 示例：`mkdir documents`（创建documents目录）、`mkdir -p a/b/c`（创建嵌套目录）

5. **rmdir**
   - 英语全称：Remove Directory
   - 功能：删除空目录
   - 示例：`rmdir old_dir`（删除空目录old_dir）

6. **cp**
   - 英语全称：Copy
   - 功能：复制文件或目录
   - 示例：`cp file1.txt file2.txt`（复制文件）、`cp -r dir1 dir2`（递归复制目录）

7. **mv**
   - 英语全称：Move
   - 功能：移动或重命名文件/目录
   - 示例：`mv file.txt docs/`（移动文件到docs目录）、`mv oldname.txt newname.txt`（重命名文件）

8. **rm**
   - 英语全称：Remove
   - 功能：删除文件或目录
   - 示例：`rm file.txt`（删除文件）、`rm -rf dir/`（强制递归删除目录及内容）

9. **touch**
   - 英语全称：Touch
   - 功能：创建空文件或更新文件时间戳
   - 示例：`touch newfile.txt`（创建新文件）、`touch -d "2023-01-01" file.txt`（修改文件时间戳）

10. **ln**
    - 英语全称：Link
    - 功能：创建文件链接
    - 示例：`ln -s source.txt link.txt`（创建符号链接）、`ln file.txt hardlink.txt`（创建硬链接）

## 文件内容操作

11. **cat**
    - 英语全称：Concatenate
    - 功能：连接并显示文件内容
    - 示例：`cat file.txt`（显示文件内容）、`cat file1.txt file2.txt > combined.txt`（合并文件）

12. **tac**
    - 英语全称：Reverse Cat
    - 功能：反向显示文件内容
    - 示例：`tac file.txt`（从最后一行开始显示文件内容）

13. **head**
    - 英语全称：Head
    - 功能：显示文件开头内容
    - 示例：`head file.txt`（默认显示前10行）、`head -n 5 file.txt`（显示前5行）

14. **tail**
    - 英语全称：Tail
    - 功能：显示文件末尾内容
    - 示例：`tail file.txt`（默认显示最后10行）、`tail -f log.txt`（实时监控文件更新）

15. **more**
    - 英语全称：More
    - 功能：分页显示文件内容
    - 示例：`more longfile.txt`（分页查看长文件）

16. **less**
    - 英语全称：Less
    - 功能：分页显示文件内容（比more更强大）
    - 示例：`less largefile.txt`（分页查看文件，支持上下滚动）

17. **nano**
    - 英语全称：Nano
    - 功能：简单的文本编辑器
    - 示例：`nano file.txt`（编辑file.txt文件）

18. **vim**
    - 英语全称：Vi Improved
    - 功能：高级文本编辑器
    - 示例：`vim document.txt`（使用vim编辑文件）

19. **grep**
    - 英语全称：Global Regular Expression Print
    - 功能：在文件中搜索匹配的字符串
    - 示例：`grep "error" log.txt`（在log.txt中搜索"error"）、`grep -r "keyword" /home`（递归搜索目录）

20. **wc**
    - 英语全称：Word Count
    - 功能：统计文件的行数、单词数和字符数
    - 示例：`wc file.txt`（统计文件）、`wc -l file.txt`（只统计行数）

## 系统信息与管理

21. **uname**
    - 英语全称：Unix Name
    - 功能：显示系统信息
    - 示例：`uname -a`（显示所有系统信息）、`uname -r`（显示内核版本）

22. **hostname**
    - 英语全称：Host Name
    - 功能：显示或设置主机名
    - 示例：`hostname`（显示当前主机名）、`hostname newname`（临时设置主机名）

23. **date**
    - 英语全称：Date
    - 功能：显示或设置系统日期和时间
    - 示例：`date`（显示当前日期时间）、`date "+%Y-%m-%d %H:%M:%S"`（自定义格式显示）

24. **cal**
    - 英语全称：Calendar
    - 功能：显示日历
    - 示例：`cal`（显示当前月份日历）、`cal 2024`（显示2024年全年日历）

25. **df**
    - 英语全称：Disk Free
    - 功能：显示磁盘空间使用情况
    - 示例：`df -h`（以人类可读格式显示磁盘信息）

26. **du**
    - 英语全称：Disk Usage
    - 功能：显示目录或文件的磁盘使用空间
    - 示例：`du -sh directory/`（显示目录总大小）、`du -h *`（显示当前目录下各文件大小）

27. **free**
    - 英语全称：Free
    - 功能：显示内存使用情况
    - 示例：`free -h`（以人类可读格式显示内存信息）

28. **top**
    - 英语全称：Top
    - 功能：实时显示系统进程资源占用情况
    - 示例：`top`（启动实时进程监控）

29. **htop**
    - 英语全称：Human-friendly Top
    - 功能：增强版的top命令，交互性更好
    - 示例：`htop`（启动增强版进程监控）

30. **ps**
    - 英语全称：Process Status
    - 功能：显示当前进程状态
    - 示例：`ps aux`（显示所有进程）、`ps -ef | grep "python"`（查找python相关进程）

## 进程管理

31. **kill**
    - 英语全称：Kill
    - 功能：终止进程
    - 示例：`kill 1234`（终止PID为1234的进程）、`kill -9 1234`（强制终止进程）

32. **pkill**
    - 英语全称：Process Kill
    - 功能：根据进程名终止进程
    - 示例：`pkill firefox`（终止所有firefox进程）

33. **bg**
    - 英语全称：Background
    - 功能：将前台进程切换到后台运行
    - 示例：`bg %1`（将编号为1的任务放到后台）

34. **fg**
    - 英语全称：Foreground
    - 功能：将后台进程切换到前台运行
    - 示例：`fg %1`（将编号为1的后台任务调到前台）

35. **jobs**
    - 英语全称：Jobs
    - 功能：显示当前后台运行的任务
    - 示例：`jobs`（列出所有后台任务）

## 用户与权限管理

36. **sudo**
    - 英语全称：Superuser Do
    - 功能：以超级用户权限执行命令
    - 示例：`sudo apt update`（以管理员权限更新软件源）

37. **su**
    - 英语全称：Switch User
    - 功能：切换用户
    - 示例：`su - root`（切换到root用户）、`su - username`（切换到指定用户）

38. **chmod**
    - 英语全称：Change Mode
    - 功能：修改文件或目录的权限
    - 示例：`chmod 755 file.sh`（设置文件权限）、`chmod +x script.sh`（添加执行权限）

39. **chown**
    - 英语全称：Change Owner
    - 功能：修改文件或目录的所有者
    - 示例：`chown user:group file.txt`（修改文件的所有者和所属组）

40. **passwd**
    - 英语全称：Password
    - 功能：修改用户密码
    - 示例：`passwd`（修改当前用户密码）、`passwd username`（修改指定用户密码，需管理员权限）

## 网络操作

41. **ping**
    - 英语全称：Ping
    - 功能：测试网络连接
    - 示例：`ping google.com`（测试与google.com的连接）、`ping -c 4 192.168.1.1`（发送4个数据包）

42. **ifconfig**
    - 英语全称：Interface Configuration
    - 功能：配置或显示网络接口信息
    - 示例：`ifconfig`（显示所有网络接口信息）、`ifconfig eth0 up`（启用eth0接口）

43. **ip**
    - 英语全称：IP
    - 功能：网络配置工具（替代ifconfig）
    - 示例：`ip addr`（显示IP地址信息）、`ip route`（显示路由表）

44. **netstat**
    - 英语全称：Network Statistics
    - 功能：显示网络连接、路由表等信息
    - 示例：`netstat -tuln`（显示监听的端口）

45. **curl**
    - 英语全称：Client URL
    - 功能：用于URL传输数据
    - 示例：`curl http://example.com`（获取网页内容）、`curl -O http://example.com/file.zip`（下载文件）

46. **wget**
    - 英语全称：World Wide Web Get
    - 功能：从网络下载文件
    - 示例：`wget http://example.com/file.tar.gz`（下载文件）、`wget -c http://example.com/largefile.iso`（断点续传）

## 软件包管理

47. **apt**
    - 英语全称：Advanced Package Tool
    - 功能：Debian/Ubuntu系统的包管理工具
    - 示例：`sudo apt update`（更新软件源）、`sudo apt install package`（安装软件包）

48. **yum**
    - 英语全称：Yellowdog Updater Modified
    - 功能：RHEL/CentOS系统的包管理工具
    - 示例：`sudo yum install package`（安装软件包）、`sudo yum update`（更新系统）

49. **dpkg**
    - 英语全称：Debian Package
    - 功能：Debian系统的包管理工具，用于处理.deb文件
    - 示例：`sudo dpkg -i package.deb`（安装本地deb包）

50. **tar**
    - 英语全称：Tape Archive
    - 功能：打包和解压文件
    - 示例：`tar -czvf archive.tar.gz directory/`（压缩目录）、`tar -xzvf archive.tar.gz`（解压文件）

------


## Linux常用命令深度解析

本文详细解析Linux系统中最常用的命令，包括它们的高级用法、参数说明和实际应用场景，帮助你更高效地使用Linux系统。

### 文件压缩与归档命令

#### 1. tar
- **全称**：Tape Archive（磁带归档）
- **核心功能**：创建和提取归档文件，可与压缩算法结合使用

**基础语法**：tar [选项] 归档文件名 源文件/目录  
**常用选项**：
- `-c`：创建新归档
- `-x`：从归档中提取文件
- `-v`：显示详细过程（verbose）
- `-f`：指定归档文件名（必须放在选项最后）
- `-z`：使用gzip压缩/解压缩（.tar.gz）
- `-j`：使用bzip2压缩/解压缩（.tar.bz2）
- `-J`：使用xz压缩/解压缩（.tar.xz）
- `-t`：列出归档内容而不提取

**实用示例**：
- 创建gzip压缩的归档  
  `tar -czvf documents.tar.gz /home/user/docs`

- 提取tar.gz归档到当前目录  
  `tar -xzvf documents.tar.gz`

- 提取tar.gz归档到指定目录  
  `tar -xzvf documents.tar.gz -C /tmp/extracted`

- 查看归档内容而不提取  
  `tar -tzvf documents.tar.gz`

- 仅提取归档中的特定文件  
  `tar -xzvf backup.tar.gz home/user/file.txt`

#### 2. zip/unzip
- **全称**：Zip/Unzip
- **核心功能**：创建和提取ZIP格式的压缩文件（跨平台兼容）

**常用语法**：
- 创建zip压缩包  
  `zip [选项] 压缩包名 源文件/目录`

- 提取zip压缩包  
  `unzip [选项] 压缩包名`

**常用选项**：
- `zip -r`：递归压缩目录
- `zip -q`：安静模式，不显示压缩过程
- `unzip -l`：列出压缩包内容
- `unzip -d 目录`：指定解压目录
- `unzip -q`：安静模式解压

**实用示例**：
- 压缩目录及内容  
  `zip -r images.zip photos/`

- 排除特定文件压缩  
  `zip -r backup.zip docs/ -x "*.tmp"`

- 查看压缩包内容  
  `unzip -l images.zip`

- 解压到指定目录  
  `unzip images.zip -d /var/www/images`

- 测试压缩包完整性  
  `unzip -t backup.zip`

### 磁盘空间管理

#### 3. du
- **全称**：Disk Usage（磁盘使用）
- **核心功能**：查看文件和目录占用的磁盘空间

**常用选项**：
- `-h`：以人类可读格式显示（KB, MB, GB）
- `-s`：显示总计，不列出子目录
- `-c`：显示总计（与-s不同，可与其他选项结合）
- `-d N`：显示深度为N的目录大小（替代旧版的--max-depth=N）
- `-a`：包含所有文件，不仅仅是目录

**实用示例**：
- 查看当前目录总大小  
  `du -sh`

- 查看当前目录下各子目录大小（一级）  
  `du -h --max-depth=1`

- 查看所有.jpg文件的总大小  
  `du -ch *.jpg`

- 查找大于100MB的目录  
  `du -h --max-depth=2 | grep -E '^[0-9]+[MG]'`

- 按大小排序显示目录  
  `du -h --max-depth=1 | sort -hr`

#### 4. df
- **全称**：Disk Free（磁盘空闲）
- **核心功能**：查看文件系统的磁盘空间使用情况

**常用选项**：
- `-h`：人类可读格式
- `-T`：显示文件系统类型
- `-i`：显示inode使用情况（而非块使用情况）
- `-x 类型`：排除指定类型的文件系统

**实用示例**：
- 查看所有挂载的文件系统空间  
  `df -h`

- 查看文件系统类型  
  `df -hT`

- 查看inode使用情况（排查"磁盘未满但无法创建文件"问题）  
  `df -i`

- 仅显示ext4和xfs文件系统  
  `df -hT | grep -E 'ext4|xfs'`

- 排除tmpfs文件系统  
  `df -h -x tmpfs`

### 文本搜索与处理

#### 5. grep
- **全称**：Global Regular Expression Print（全局正则表达式打印）
- **核心功能**：在文本中搜索匹配正则表达式的行

**常用选项**：
- `-i`：忽略大小写
- `-v`：反向匹配（显示不匹配的行）
- `-r`：递归搜索目录中的文件
- `-n`：显示匹配行的行号
- `-w`：匹配整个单词
- `-c`：只显示匹配的行数
- `-E`：使用扩展正则表达式

**实用示例**：
- 在文件中搜索关键词（忽略大小写）  
  `grep -i "error" /var/log/syslog`

- 统计匹配行数  
  `grep -c "failed" /var/log/auth.log`

- 递归搜索目录中的关键词  
  `grep -r "TODO" /home/user/projects/`

- 显示匹配行及其前后5行  
  `grep -C 5 "critical" server.log`

- 搜索整个系统中的配置文件  
  `grep -r --include="*.conf" "port 80" /etc/`

- 反向匹配（排除注释和空行）  
  `grep -v '^#\|^$' /etc/nginx/nginx.conf`

### 权限管理

#### 6. chmod
- **全称**：Change Mode（更改模式）
- **核心功能**：修改文件或目录的访问权限

**权限表示方法**：
- 数字表示：r=4, w=2, x=1（rwx=7, rw-=6, r-x=5, 等）
- 符号表示：u(用户), g(组), o(其他), a(所有)；+(添加), -(移除), =(设置)

**实用示例**：
- 给文件添加执行权限（对所有者）  
  `chmod u+x script.sh`

- 给所有用户添加读写权限  
  `chmod a+rw document.txt`

- 设置目录权限（用户可读写执行，组和其他只读）  
  `chmod 755 /var/www`

- 递归修改目录及其内容的权限  
  `chmod -R 644 /home/user/docs`

- 仅给所有者添加执行权限，移除组和其他的写权限  
  `chmod u+x,go-w file.sh`

- 设置SGID（子目录继承父目录的组）  
  `chmod g+s /shared/directory`

### 软件包管理（Debian/Ubuntu）

#### 7. apt
- **全称**：Advanced Package Tool（高级包工具）
- **核心功能**：Debian/Ubuntu系统中管理软件包

**常用命令**：
- 更新软件包列表  
  `sudo apt update`

- 升级所有可更新的软件包  
  `sudo apt upgrade`

- 升级系统（包括内核）  
  `sudo apt full-upgrade`

- 安装软件包  
  `sudo apt install package_name`

- 安装多个软件包  
  `sudo apt install package1 package2`

- 卸载软件包（保留配置）  
  `sudo apt remove package_name`

- 彻底卸载（删除配置）  
  `sudo apt purge package_name`

- 搜索软件包  
  `apt search keyword`

- 查看软件包信息  
  `apt show package_name`

- 清理无用的依赖包  
  `sudo apt autoremove`

- 清理下载的安装包  
  `sudo apt clean`

**实用技巧**：
- 仅升级特定软件包  
  `sudo apt install --only-upgrade package_name`

- 下载软件包但不安装  
  `sudo apt download package_name`

- 模拟执行命令（测试效果）  
  `apt upgrade --dry-run`

- 查看哪些包需要升级  
  `apt list --upgradable`

### 其他高频使用命令

#### 8. find
- **功能**：在目录树中搜索文件
- **实用示例**：
  - 在当前目录查找所有.txt文件  
    `find . -name "*.txt"`

  - 在/var/log中查找24小时内修改过的文件  
    `find /var/log -mtime -1`

  - 查找大于100MB的文件  
    `find /home -size +100M`

  - 查找并删除所有.tmp文件  
    `find . -name "*.tmp" -delete`

  - 查找并更改权限  
    `find . -type f -name "*.sh" -exec chmod +x {} \;`

#### 9. ps
- **全称**：Process Status（进程状态）
- **功能**：查看系统中的进程
- **实用示例**：
  - 查看所有进程  
    `ps aux`

  - 查找特定进程  
    `ps aux | grep "nginx"`

  - 以树形结构显示进程  
    `ps -ef --forest`

  - 按内存使用排序  
    `ps aux --sort=-%mem | head -10`

  - 按CPU使用排序  
    `ps aux --sort=-%cpu | head -10`

#### 10. netstat/ss
- **全称**：Network Statistics（网络统计）
- **功能**：查看网络连接、端口监听等网络信息
- **实用示例**：
  - 查看所有监听端口  
    `netstat -tuln`

  - 现代替代命令  
    `ss -tuln`

  - 查看已建立的连接  
    `netstat -tulnp`

  - 查看特定端口的使用情况  
    `netstat -tuln | grep 80`

  - 查看路由表  
    `netstat -r`

#### 11. ssh
- **全称**：Secure Shell（安全外壳）
- **功能**：远程登录到其他计算机
- **实用示例**：
  - 基本远程登录  
    `ssh username@remote_host`

  - 指定端口登录  
    `ssh -p 2222 username@remote_host`

  - 免密码登录配置  
    `ssh-keygen -t ed25519`  
    `ssh-copy-id username@remote_host`

  - 远程执行命令  
    `ssh username@remote_host "df -h"`

  - 端口转发  
    `ssh -L 8080:localhost:80 username@remote_host`

#### 12. scp
- **全称**：Secure Copy（安全复制）
- **功能**：通过SSH在计算机之间复制文件
- **实用示例**：
  - 本地文件复制到远程  
    `scp local_file.txt username@remote_host:/remote/path/`

  - 远程文件复制到本地  
    `scp username@remote_host:/remote/file.txt /local/path/`

  - 复制目录  
    `scp -r local_directory/ username@remote_host:/remote/path/`

  - 指定端口  
    `scp -P 2222 file.txt username@remote_host:/path/`


通过`man 命令名`（如`man tar`）查看完整的手册页



## Appendix

- [菜鸟Linux](https://www.runoob.com/linux/linux-tutorial.html)
- [w3cschool Linux](https://www.w3cschool.cn/linux/linux-command-manual.html)
