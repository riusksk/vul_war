# Vulnerability War: The Essence of Software Vulnerabilities Analysis
By riusksk(@riusksk)
## Content Abstract
 Vulnerability War: The Essence of Software Vulnerabilities Analysis systematically explain all kinds of tools, techniques and practical methods in software vulnerability analysis and exploit, mainly related to Windows and Android platform. The book is classfied according to the different vulnerabilities, such as stack overflow, sandbox escape, types confusion, UAF , kernel vulnerability etc., at the same time, in view of the current popular mobile security, add Android platform vulnerability analysis and exploit into it. The author carefully chosen classic Vulnerabilities to share analysis techniques and tools about the cause of these vulnerabilities analysis, exploit and fix methods in detail. The biggest characteristic of this book is the actual combat based on the various types of classical vulnerabilities and discard useless theory, it's almost "a book written out by debugger".

This book is suitable for students of computer science related, somebody worked in information security, software security and mobile security related areas, software developer and hackers to read.

## Directory
### Chapter 1: Basic Knowledge 
1.1 The Concepts of Vulnerability  
1.1.1	What is The Vulnerability   
1.1.2 The Value of Vulnerabilities  
1.1.3 0day Vulnerability  
1.1.4 PoC and Exploit  
1.2 Why to analysis vunerabilities  
1.3 The commonly analysis tools  
1.3.1 IDA: the disassembly tool  
1.3.2 OllyDbg: the crack and reverse analysis tool  
1.3.3 Immunity Debugger: vulnerability analysis debugger  
1.3.4 Windbg: Microsoft Windows Debugger  
1.3.5 GDB: Linux Debugger  
1.3.6 JEB: Android Decompilater  
1.3.7 Other  
1.4 The common vulnerability analysis method  
1.4.1 Static analysis  
1.4.2 Dynamic debugging  
1.4.3 Source code analysis  
1.4.4 Patch compare  
1.4.5 Taint track  
1.5 Learning resources  
1.5.1 Some security sites  
1.5.2 Recommended books  
1.6 Summary 
### Chapter 2: Stack Overflow Vulnerability Analysis
2.1 A brief history of stack overflow  
2.2 The principle of stack overflow  
2.3 CVE-2010-2883 Adobe Reader TTF Font SING Table Stack Overflow  
2.3.1 LuckyCat APT Attacks  
2.3.2 Vulnerability Description  
2.3.3 Analysis environment  
2.3.4 The Vulnerability Analysis Method Based On String Search  
2.3.5 Exploit Technical Analysis of Sample  
2.3.6 Shellcode Malicious Behavior Analysis of Sample  
2.3.7 Vulnerability Fixes  
2.4 CVE-2010-3333 Microsoft RTF File Stack Overflow  
2.4.1 Linsanity Attack Event  
2.4.2 Vulnerability Description  
2.4.3 Analysis Environment  
2.4.4 RTF File Format  
2.4.5 The Vulnerability Analysis Method Based On Stack Backtrace  
2.4.6 Vulnerability Exploit  
2.4.7 Office 2003 and Office 2007 Commonality Exploit Technical Research  
2.4.8 Vulnerability Fixes  
2.5 CVE-2011-0104 Microsoft Excel TOOLBARDEF Record Stack Overflow  
2.5.1 Vulnerability Description  
2.5.2 Analysis Environment  
2.5.3 The Vulnerability Analysis Method Based On Taint Track  
2.5.4 Vulnerability Fixes  
2.6 AliWangWang ActiveX Control imageMan.dll Stack Overflow  
2.6.1 Vulnerability Description  
2.6.2 Analysis Environment   
2.6.3 ActiveX Control Vulnerability Analysis Method  
2.6.4 Vulnerability Exploit  
2.7 CVE-2012-0158 Microsoft Office MSCOMCTL.ocx Stack Overflow  
2.7.1 Lotus Blossom Operation  
2.7.2 Vulnerability Description  
2.7.3 Analysis Environment   
2.7.4 Office Vulnerability Analysis With OffVis  
2.7.4 Vulnerability Fixes  
2.8 Summary  
### Chapter 3: Heap Overflow Vulnerability Analysis
3.1 A Brief History of Heap Overflow  
3.2 The Principle of Heap Overflow  
3.3 Heap Debugging Skills  
3.3.1 Heap Tail Check  
3.3.2 Page Heap  
3.4 CVE-2010-2553 Microsoft Cinepak Codec CVDecompress Heap Overflow  
3.4.1 Vulnerability Description  
3.4.2 Analysis Environment  
3.4.3 Heap Vulnerability Analysis Method Based On HeapPage  
3.4.4 Vulnerability Fixes  
3.5 CVE-2012-0003 Microsoft Windows Media Player winmmdll MIDI File Heap Overflow  
3.5.1 About Zhi-Zhu Exploit Pack  
3.5.2 Vulnerability Description  
3.5.3 Analysis Environment  
3.5.4 MIDI File Format  
3.5.5 Vulnerability Analysis Method Based On Mapping Calculated  
3.5.6 Vulnerability Exploit  
3.5.7 Patch Different  
3.6 CVE-2013-0077 Microsoft DirectShow quartz.dll M2P File Heap Overflow  
3.6.1 Vulnerability Description  
3.6.2 Vulnerability Analysis With HTC  
3.6.3 Vulnerability Fixes  
3.7 CVE-2012-1876 Internet Exporter MSHTMLdll CalculateMinMax Heap Overflow  
3.7.1 The Vulnerability Used to Break IE9 Browser in Pwn2Own Hacking Contest  
3.7.2 Analysis Environment  
3.7.3 Vulnerability Analysis With HPA  
3.7.4 Vulnerability Exploit Based On Infomation Leakage  
3.7.5 Vulnerability Fixes  
3.8 Summary  
### Chapter 4: Integer Overflow Vulnerability Analysis
4.1 A Brief History of Integer Overflow  
4.2 The Principle of Integer Overflow  
4.2.1 Integer Overflow In Stack   
4.2.2 Integer Overflow In Heap  
4.3 CVE-2011-0027 Microsoft Data Access Components Integer Overflow  
4.3.1 The Vulnerability Used to Break IE8 Browser in Pwn2Own Hacking Contest  
4.3.2 Vulnerability Analysis Method Based On Heap Allocation Record  
4.3.3 Patch Different  
4.4 CVE-2012-0774 Adobe Reader TrueType Font Integer Overflow  
4.4.1 Vulnerability Description  
4.4.2 PDF File Format and Commonly Analysis Tools  
4.4.3 Vulnerability Analysis Method Based On Condition Records Breakpoint   
4.4.4 Patch Analysis  
4.5 CVE-2013-0750 Firefox String Replace Integer Overflow  
4.5.1 Vulnerability Description  
4.5.2 Vulnerability Analysis Method Based On Source Code Debugging  
4.5.3 Source Code Diff  
4.6 CVE-2013-2551 Internet Explorer VML COALineDashStyleArray Integer Overflow  
4.6.1 The Vulnerability Used to Break IE10 Browser in Pwn2Own Hacking Contest  
4.6.2 Vulnerability Analysis Method Based On Class Function Search  
4.6.3 Used Info Leak to Exploit  
4.7 Summary  
### Chapter 5: Format String Vulnerability Analysis  
5.1 A Brief History of Format String Vulnerability  
5.2 The Principle of Format String Vulnerability  
5.3 CVE-2012-0809 Sudo sudo_debug Format String Vulnerability  
5.3.1 Vulnerability Description  
5.3.2 Analysis Vulnerability By Source Code Diff  
5.4 CVE-2012-3569 VMware OVF Tool Format String Vulnerability  
5.4.1 Vulnerability Description  
5.4.2 Vulnerability Analysis Method Based On Output Message  
5.4.3 Vulnerability Exploit  
5.5 Summary  
### Chapter 6: Double Free Vulnerability Analysis
6.1 A Brief History of Double Free Vulnerability  
6.2 The Principle of Double Free Vulnerability  
6.3 CVE-2010-3974 Windows Fax Cover Editor fxscover.exe Double Free  
6.3.1 Vulnerability Description  
6.3.2 Used Stack Backtrack and Heap State to Detect Vulnerability Type  
6.3.3 Used Patch Diff to Analysis Vulnerability Causes and Fix Method  
6.4 CVE-2014-0502 Adobe Flash Player Double Free  
6.4.1 GreedyWonk Operation  
6.4.2 Static Analysis Attack Sample  
6.4.3 Automation Simulation Shellcode Execution  
6.4.4 Trace Back Analysis Based on ROP Instruction Address  
6.5 Summary  
### Chapter 7: Use After Free Vulnerability Analysis
7.1 A Brief History of Use After Free(UAF)  
7.2 The Principle of UAF  
7.3 CVE-2011-0065 Firefox mChannel UAF Vulnerability  
7.3.1 Vulnerability Description  
7.3.2 Through Dynamic debugging to Rapid Positioning Source Code Which Lead to Bug  
7.3.3 Vulnerability Exploit  
7.3.4 Source Code Compare  
7.4 CVE-2013-1347 Microsoft IE CGenericElement Use After Free  
7.4.1 Watering Hole Attack Event  
7.4.2 Rapid Positioning Vulnerability Object With HPA  
7.4.3 Reverse Analysis IE JavaScript Engine   
7.4.4 Analysis The Cause of Vulnerability  
7.4.5 Vulnerability Exploit  
7.5 CVE-2013-3346 Adobe Reader ToolButton UAF Vulnerability  
7.5.1 "Epic Turla" Cyber Espionage Attacks  
7.5.2 Analysis Malicious PDF Sample With peepdf  
7.5.3 Vulnerability Exploit  
7.6 CVE-2015-0313 Adobe Flash Player Workers ByteArray UAF Vulnerability  
7.6.1 Vulnerability Description  
7.6.2 Analysis ActiveScript VM Source Code to Help Vulnerability Debugging  
7.6.3 Flash JIT Debugging Plugin and Symbol File  
7.6.4 Vulnerability Exploit  
7.6.5 Vulnerability Fixes  
7.7 Summary  
### Chapter 8: Array Out-of-Bound Vulnerability Analysis
8.1 The Relationship Between Array Out-of-Bound and Overflow  
8.2 The Principle of Array Out-of-Bound Vulnerability  
8.3 CVE-2011-2110 Adobe Flash Player Array Out-of-Bound Access Vulnerability  
8.3.1 Vulnerability Description  
8.3.2 Solve The Problem of Restriction to Install The Old Version Flash Player  
8.3.3 Use Perl Script to Analysis Sample  
8.3.4 Setup The Server to Reproduce Bug  
8.3.5 Modify Sample Code to Analysis Vulnerability  
8.3.6 Constructing Info Leak to Exploit  
8.3.7 Search Instruction Sequence to Analysis Patch  
8.4 CVE-2014-0160 OpenSSL TLS Array Out-of-Bound Vulnerability("Heart Bleeding")  
8.4.1 Vulnerability Description  
8.4.2 Vulnerability Analysis Method Based On Source Code Contrast and Tracking  
8.4.3 Exploit Vulnerability to Steal Site Account  
8.5 Summary  
### Chapter 9: Kernel Vulnerability Analysis
9.1 Talk About Windows Kernel Vulnerability  
9.2 Build Windows Kernel Debugging Environment  
9.3 Common Kernel Vulnerability Principle And Exploit  
9.3.1 Vulnerability Cause Analysis  
9.3.2 vulnerability Exploit  
9.4 360 Security Guards bregdrv.sys Local Privilege Escalation Analysis  
9.4.1 Vulnerability Description  
9.4.2 Tracking Analysis With Export Function and IO Control Code  
9.5 CVE-2011-2005 Windows Afd.sys Local Privilege Escalation  
9.5.1 Vulnerability Description  
9.5.2 From Exploit Code to Vulnerability Function Positioning Analysis  
9.5.3 Patch Different  
9.6 CVE-2013-3660 Windows win32ksys EPATHOB Pointer Uninitialized Vulnerability  
9.6.1 Vulnerability Description  
9.6.2 Auxiliary Analysis With IDA Defined Structure   
9.6.3 Vulnerability Exploit  
9.7 CVE-2014-1767 Windows AFD.sys Double Free Vulnerability (Pwn2Own 2014)  
9.7.1 The Best Privilege Escalation Bug in Pwnie Awards 2014  
9.7.2 Vulnerability Analysis Method Based on IOCTL Handler Automatically Track Record  
9.7.3 Vulnerability Exploit  
9.7.4 Patch Analysis  
9.8 Summary  
### Chapter 10: Android Platform Vulnerability Analysis
10.1 A Brief History of Android Platform Vulnerability  
10.2 Android Platform Vulnerability Type  
10.3 The Common Vulnerability Analysis Methods  
10.3.1 APK Static Analysis  
10.3.2 Smali Dynamic Debugging  
10.3.3 so Library Dynamic Debugging  
10.3.4 Patch Source Code Different  
10.3.5 System Java Source Code Debugging  
10.3.6 System C/C++ Source Code Debugging  
10.3.7 Android Kernel Source Code Debugging  
10.4  Smart Outlet Vulnerability Analysis  
10.4.1 Vulnerability Description  
10.4.2 Static Reverse Analysis  
10.4.3 Exploit Vulnerability to Control Arbitrary Outlet in Network  
10.4.4 Summary  
10.5 CVE-2013-4787 Android Signature Vulnerability  
10.5.1 Vulnerability Description  
10.5.2 Android Signature Mechanism  
10.5.3 Reproduce Bug  
10.5.4 Vulnerability Analysis  
10.5.5 Vulnerability Fixes  
10.6 CVE-2010-1119 Android WebKit UAF Vulnerability  
10.6.1 Vulnerability Description  
10.6.2 Vulnerability Exploit  
10.6.3 Analysis Patch Source Code to Positioning Cause  
10.7 CVE-2014-3153 Android Kernel Futex Privilege Escalation (Towelroot)  
10.7.1 Android Devices Root Tool —— Towelroot  
10.7.2 Analysis Vulnerability With Kernel Source Code Debugging  
10.7.3 Vulnerability Exploit  
10.7.4 Vulnerability Fixes  
10.8 Summary  
### Chapter 11: Other Types of Vulnerability Analysis
11.1 Introduction  
11.2 CVE-2013-2423 JAVA Applet Reflection Type Confusion Code Execution Vulnerability  
11.2.1 Vulnerability Description  
11.2.2 Type Confusion Vulnerability  
11.2.3 Java Security Mechanism  
11.2.4 Vulnerability Analysis and Exploit  
11.2.5 Vulnerability Fixes  
11.2.6 The King of Vulnerability in 2013 —— Java  
11.3 CVE-2014-0257 Microsoft Internet Explorer 11 dfsvc Component Sandbox Escape   
11.3.1 Vulnerability Description  
11.3.2 IE Sandbox Protect Principle  
11.3.3 IE Sandbox Attack Surface Analysis  
11.3.4 CVE-2014-0257 Vulnerability Analysis and Exploit  
11.4 CVE-2014-9150 Adobe Acrobat Reader MoveFileEx IPC Hook Race Condition Vulnerability  
11.4.1 Therac-25 Medical Accident  
11.4.2 Race Condition Principle  
11.4.3 CVE-2014-9150 Vulnerability Description  
11.4.4 Adobe Sandbox Introduction  
11.4.5 Exploit Vulnerability to Escape Sandbox  
11.5 Summary  
### Chapter 12: The Development Trend of Software Vulnerabilities 
12.1 New Challenges in The Field of Software Vulnerabilities  
12.2 The Development Trend of Mobile Terminal Vulnerability  
12.3 The Development Trend of Cloud Computing Platform  
12.4 The Development Trend of IoT Vulnerability  
12.5 Summary  
