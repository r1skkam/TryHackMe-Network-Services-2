# TryHackMe | Network Services 2
`Enumerating and Exploiting More Common Network Services & Misconfigurations`

[TryHackMe | Network Services 2](https://tryhackme.com/room/networkservices2)

## Task 1 Get Connected
[TryHackMe | Network Services](https://tryhackme.com/room/networkservices)

[TryHackMe | Linux Fundamentals](https://tryhackme.com/module/linux-fundamentals)

[TryHackMe | Network Access](https://tryhackme.com/access)

[TryHackMe | Wifi Hacking 101](https://tryhackme.com/room/wifihacking101)

## Task 2 Understanding NFS
[How the NFS Service Works (System Administration Guide: Resource Management and Network Services)](https://docs.oracle.com/cd/E19683-01/816-4882/6mb2ipq7l/index.html)

[What is Network File System (NFS) File Share?](https://www.datto.com/blog/what-is-nfs-file-share)

[Linux NFS faq](http://nfs.sourceforge.net/)

[NFS - ArchWiki](https://wiki.archlinux.org/title/NFS)

## Task 3 Enumerating NFS 
[Infosec Resources &raquo; What is enumeration? [updated 2021] Comments Feed](https://resources.infosecinstitute.com/topic/what-is-enumeration/)

[Ubuntu – Details of package nfs-common in kinetic](https://packages.ubuntu.com/kinetic/nfs-common)

[TryHackMe | Nmap](https://tryhackme.com/room/furthernmap)

`/usr/sbin/showmount -e [IP] `

`sudo mount -t nfs IP:share /tmp/mount/ -nolock`

`ssh -i <key-file> <username>@<ip>`

## Task 4 Exploiting NFS
![./b -p](https://github.com/r1skkam/TryHackMe-Network-Services-2/blob/main/Screenshot%202022-05-26%20160958.jpg)

## Task 5 Understanding SMTP
[The SMTP Server | HowStuffWorks](https://computer.howstuffworks.com/e-mail-messaging/email3.htm)

[SMTP protocol Explained (How Email works?) - Afternerd](https://www.afternerd.com/blog/smtp/)

## Task 6 Enumerating SMTP
![smtp_version](https://github.com/r1skkam/TryHackMe-Network-Services-2/blob/main/Screenshot%202022-05-27%20222900.png)

![smtp_enum](https://github.com/r1skkam/TryHackMe-Network-Services-2/blob/main/Screenshot%202022-05-27%20223916.png)

![administrator](https://github.com/r1skkam/TryHackMe-Network-Services-2/blob/main/Screenshot%202022-05-27%20225035.png)

## Task 7 Exploiting SMTP
`hydra -t 16 -l administrator -P /usr/share/wordlists/rockyou.txt -vV 10.10.64.127 ssh`

![hydra](https://github.com/r1skkam/TryHackMe-Network-Services-2/blob/main/Screenshot%202022-05-27%20225942.png)

![smtp.txt](https://github.com/r1skkam/TryHackMe-Network-Services-2/blob/main/Screenshot%202022-05-27%20230146.png)

## Task 8 Understanding MySQL
[MySQL: SQL Query Execution](https://dev.mysql.com/doc/dev/mysql-server/latest/PAGE_SQL_EXECUTION.html)

[PHP: MySQL Database](https://www.w3schools.com/php/php_mysql_intro.asp)

## Task 9 Enumerating MySQL
[mysql-enum NSE script - Nmap Scripting Engine documentation](https://nmap.org/nsedoc/scripts/mysql-enum.html)

[MySQL - Remote User Enumeration - Multiple remote Exploit](https://www.exploit-db.com/exploits/23081)

[Enumerating MySQL](https://github.com/r1skkam/TryHackMe-Network-Services-2/blob/main/Enumerating%20MySQL)

```
root@ip-10-10-2-168:~# nc 10.10.24.180 3306
[
5.7.29-0ubuntu0.18.04.1J
.S
  R\ufffd\ufffd\ufffdvNd8;(K!,J>mysql_native_password
```

[mysql> show databases;](https://github.com/r1skkam/TryHackMe-Network-Services-2/blob/main/show%20databases)

## Task 10 Exploiting MySQL
[mysql_hashdump](https://github.com/r1skkam/TryHackMe-Network-Services-2/blob/main/mysql_hashdump)

[john hash.txt](https://github.com/r1skkam/TryHackMe-Network-Services-2/blob/main/john%20hash.txt)

[MySQL.txt](https://github.com/r1skkam/TryHackMe-Network-Services-2/blob/main/MySQL.txt)

## Task 11 Further Learning 
[Common Exploits and Attacks](https://web.mit.edu/rhel-doc/4/RH-DOCS/rhel-sg-en-4/ch-exploits.html)

[NSA Warns of Vulnerabilities in Multiple VPN Services - Nextgov](https://www.nextgov.com/cybersecurity/2019/10/nsa-warns-vulnerabilities-multiple-vpn-services/160456/)
