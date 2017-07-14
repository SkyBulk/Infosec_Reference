##Forensics & Incident Response


#####TOC
* General
* Tools
* [Presentations/Talks](#talks)
* [Anti-Forensics](#anti)
* [Mobile Device Forensics](#mobile)
	* [Android](#android)
	* [iOS](#ios)
	* [Blackberry](#bb)
[PDF Forensics](#pdf)
[Photo Forensics](#photo)
[Tools](#tools)
[OS Forensics](#os)
	* [Linux Forensics](#linux)
	* [OS X Forensics](#osx)
	* [Windows Forensics](#windows)



* Better security - Mean time to detect/Mean time to respond


#### CULL

https://forensiccontrol.com/resources/free-software/

Forensics wiki
Yelp/Github - OSX Collector - Mass style forensics/management


[Know your Windows' Processes](https://sysforensics.org/2014/01/know-your-windows-processes.html)

[Santoku Linux How-Tos'](https://santoku-linux.com/howtos)

hackingexposedcomputerforensicsblog.blogspot.com/2015/02/automating-dfir-how-to-series-on_21.html)

#### End Cull










#### Sniper Forensics
http://windowsir.blogspot.com/2013/11/sniper-forensics-memory-analysis-and.html

[Malware Management Framework - Sniper Forensics Toolkit](http://sniperforensicstoolkit.squarespace.com/malwaremanagementframework/)

[The Malware Management Framework](https://malwarearchaeology.squarespace.com/mmf/)
* The Malware Reporting Standard](https://static1.squarespace.com/static/552092d5e4b0661088167e5c/t/55220280e4b0170ec8b526b6/1428292224531/Malware+Reporting+Standard+vApril+2015.pdf)
* BSidesLV Presentation](https://static1.squarespace.com/static/552092d5e4b0661088167e5c/t/552200afe4b0e4ad5008b943/1428291802554/Malware+Mgmt+Framework+v2.0.pdf)

[Sniper Forensics](https://digital-forensics.sans.org/summit-archives/2010/2-newell-spiderlabs-sniper-forensics.pdf)
* Pg10 and onward
* [Link](https://sniperforensicstoolkit.squarespace.com/storage/logging/Windows%20Logging%20Cheat%20Sheet%20v1.1.pdf)





### General

[Introduction to DFIR](https://sroberts.github.io/2016/01/11/introduction-to-dfir-the-beginning/)

[File Signature Table](http://www.garykessler.net/library/file_sigs.html)
* This table of file signatures (aka "magic numbers") is a continuing work-in-progress. I have found little information on this in a single place, with the exception of the table in Forensic Computing: A Practitioner's Guide by T. Sammes & B. Jenkinson (Springer, 2000); that was my inspiration to start this list in 2002. See also Wikipedia's List of file signatures. Comments, additions, and queries can be sent to Gary Kessler at gck@garykessler.net.

[IRMA - Incident Response & Malware Analysis](http://irma.quarkslab.com/index.html)
* IRMA intends to be an open-source platform designed to help identifying and analyzing malicious files.  However, today's defense is not only about learning about a file, but it is also getting a fine overview of the incident you dealt with: where / when a malicious file has been seen, who submitted a hash, where a hash has been noticed, which anti-virus detects it, ...  An important value with IRMA comes from you keep control over where goes / who gets your data. Once you install IRMA on your network, your data stays on your network.  Each submitted files is analyzed in various ways. For now, we focus our efforts on multiple anti-virus engines, but we are working on other "probes" (feel free to submit your own).

[No Easy Breach: Challenges and Lessons Learned from an Epic Investigation](https://archive.org/details/No_Easy_Breach#)

[Forensics on Amazon’s EC2](https://sysforensics.org/2014/10/forensics-in-the-amazon-cloud-ec2.html)

[Attrition Forensics](http://2014.video.sector.ca/video/110334184)

[Less is More, Exploring Code/Process-less Techniques and Other Weird Machine Methods to Hide Code (and How to Detect Them)](https://cansecwest.com/slides/2014/less%20is%20more3.pptx)




### Writeups
[Handler Diaries - Another Hunting Post(DFIR)](http://blog.handlerdiaries.com/?p=775)
* Good post on not only knowing the layout, but knowing expected behaviours.

#### Hacking Exposed - Automating DFIR Series

[Automating DFIR - How to series on programming libtsk with python Part 1 - ](http://hackingexposedcomputerforensicsblog.blogspot.com/2015/02/automating-dfir-how-to-series-on.html)

[Automating DFIR - How to series on programming libtsk with python Part 2](http://hackingexposedcomputerforensicsblog.blogspot.com/2015/02/automating-dfir-how-to-series-on_19.html)
[Automating DFIR - How to series on programming libtsk with python Part 3](http://

[THE CIDER PRESS:EXTRACTING FORENSIC ARTIFACTS FROM APPLE CONTINUITY](https://www.sans.org/summit-archives/file/summit-archive-1498146226.pdf)






### Tools
[MIG: Mozilla InvestiGator](https://http://mig.mozilla.org/)
* Mozilla's real-time digital forensics and investigation platform.

[SSDeep](http://ssdeep.sourceforge.net/)
* ssdeep is a program for computing context triggered piecewise hashes (CTPH). Also called fuzzy hashes, CTPH can match inputs that have homologies. Such inputs have sequences of identical bytes in the same order, although bytes in between these sequences may be different in both content and length. 

[binwally](https://github.com/bmaia/binwally)
* Binary and Directory tree comparison tool using the Fuzzy Hashing concept (ssdeep)


[PDF Tools - Didier Stevens](http://blog.didierstevens.com/programs/pdf-tools/)

[Xmount](https://www.pinguin.lu/xmount)
* What is xmount? xmount allows you to convert on-the-fly between multiple input and output harddisk image types. xmount creates a virtual file system using FUSE (Filesystem in Userspace) that contains a virtual representation of the input image. The virtual representation can be in raw DD, DMG, VHD, VirtualBox's virtual disk file format or in VmWare's VMDK file format. Input images can be raw DD, EWF (Expert Witness Compression Format) or AFF (Advanced Forensic Format) files. In addition, xmount also supports virtual write access to the output files that is redirected to a cache file. This makes it possible to boot acquired harddisk images using QEMU, KVM, VirtualBox, VmWare or alike.

[Extensible Metadata Platform](https://en.wikipedia.org/wiki/Extensible_Metadata_Platform)
* The Extensible Metadata Platform (XMP) is an ISO standard, originally created by Adobe Systems Inc., for the creation, processing and interchange of standardized and custom metadata for digital documents and data sets.

[PEview](http://wjradburn.com/software/)
* PEview provides a quick and easy way to view the structure and content of 32-bit Portable Executable (PE) and Component Object File Format (COFF) files. This PE/COFF file viewer displays header, section, directory, import table, export table, and resource information within EXE, DLL, OBJ, LIB, DBG, and other file types.

[firepwd.py](https://github.com/lclevy/firepwd)
* firepwd.py, an open source tool to decrypt Mozilla protected passwords




### Firmware 
[Firmware Forensics: Diffs, Timelines, ELFs and Backdoors](http://w00tsec.blogspot.com/2015/02/firmware-forensics-diffs-timelines-elfs.html)

[Firmware Forensics: Diffs, Timelines, ELFs and Backdoors](http://w00tsec.blogspot.com/2015/02/firmware-forensics-diffs-timelines-elfs.html)






### Bitlocker
[NVbit : Accessing Bitlocker volumes from linux](http://www.nvlabs.in/index.php?/archives/1-NVbit-Accessing-Bitlocker-volumes-from-linux.html)



### IR

[Rapier](https://code.google.com/p/rapier/)
* RAPIER is a security tool built to facilitate first response procedures for incident handling. It is designed to acquire commonly requested information and samples during an information security event, incident, or investigation. RAPIER automates the entire process of data collection and delivers the results directly to the hands of a skilled security analyst 

[triage-ir](https://code.google.com/p/triage-ir/)
* Triage: Incident Response automatically collect information from a system that needs basic triage functions performed upon it. The script allows for easy modification for customization to your needs, in an easy to comprehend and implement language. This tool uses a lot others to get its information. Eventually I hope to eliminate the need for them, but use them as verification. This tool requires you to download the Sysinternals Suite if you want full functionality to it.

[Fully Integrated Defense Operation (FIDO)](https://github.com/Netflix/Fido)
* FIDO is an orchestration layer used to automate the incident response process by evaluating, assessing and responding to malware. FIDO’s primary purpose is to handle the heavy manual effort needed to evaluate threats coming from today's security stack and the large number of alerts generated by them. As an orchestration platform FIDO can make using your existing security tools more efficient and accurate by heavily reducing the manual effort needed to detect, notify and respond to attacks against a network.

[Triaging Malware Incidents](http://journeyintoir.blogspot.com/2013/09/triaging-malware-incidents.html)
* Good writeup/blogpost from Journey into Incidence Response

[Computer Security Incident Handling Guide - NIST](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf)

[An Incident Handling Process for Small and Medium Businesses  - SANS 2007](https://www.sans.org/reading-room/whitepapers/incident/incident-handling-process-small-medium-businesses-1791)

[PowerForensics - PowerShell Digital Forensics](https://github.com/Invoke-IR/PowerForensics)
* The purpose of PowerForensics is to provide an all inclusive framework for hard drive forensic analysis. PowerForensics currently supports NTFS and FAT file systems, and work has begun on Extended File System and HFS+ support.

[Invoke-IR](http://www.invoke-ir.com/)






### IOC
[IOC Bucket](https://www.iocbucket.com/)
* IOC sharing platform





### Browser Forensics
[Firefox private browsing forensics](http://www.magnetforensics.com/forensic-implications-of-a-person-using-firefoxs-private-browsing/)

[MozillaRecovery](https://github.com/gtfy/MozillaRecovery)
* Recovers the master password of key3.db files, i.e. Thunderbird, Firefox

[Google Chrome Forensics-SANS](https://digital-forensics.sans.org/blog/2010/01/21/google-chrome-forensics#)

[Extension Finder](https://github.com/brad-anton/extension_finder)
* Python and PowerShell utilities for finding installed browser extensions, plug-ins and add-ons. Attempts to find installed browser extensions (sometimes called add-ons or plug-ins, depending on the browser).

[MozillaRecovery](https://github.com/gtfy/MozillaRecovery)
* Recovers the master password of key3.db files, i.e. Thunderbird, Firefox




### Memory Forensics
[Detekt](https://github.com/botherder/detekt)
* Detekt is a Python tool that relies on Yara, Volatility and Winpmem to scan the memory of a running Windows system (currently supporting Windows XP to Windows 8 both 32 and 64 bit and Windows 8.1 32bit). Detekt tries to detect the presence of pre-defined patterns that have been identified through the course of our research to be unique identifiers that indicate the presence of a given malware running on the computer. 

[Dshell](https://github.com/USArmyResearchLab/Dshell)
* An extensible network forensic analysis framework. Enables rapid development of plugins to support the dissection of network packet captures. 

[Mem forenics cheat sheet](http://forensicmethods.com/wp-content/uploads/2012/04/Memory-Forensics-Cheat-Sheet-v1.pdf)

[LiME - Linux Memory Extractor](https://github.com/504ensicsLabs/LiME)
* A Loadable Kernel Module (LKM) which allows for volatile memory acquisition from Linux and Linux-based devices, such as Android. This makes LiME unique as it is the first tool that allows for full memory captures on Android devices. It also minimizes its interaction between user and kernel space processes during acquisition, which allows it to produce memory captures that are more forensically sound than those of other tools designed for Linux memory acquisition.

[Volatility](https://github.com/volatilityfoundation/volatility)
* An advanced memory forensics framework

[evolve](https://github.com/JamesHabben/evolve)
* Web interface for the Volatility Memory Forensics Framework 

[How to Pull passwords from a memory dump](https://cyberarms.wordpress.com/2011/11/04/memory-forensics-how-to-pull-passwords-from-a-memory-dump/)

[Unmasking Careto through Memory Analysis - Andrew Case](http://2014.video.sector.ca/video/110388398)

[Windows Memory Analysis Checklist](http://www.dumpanalysis.org/windows-memory-analysis-checklist)







### Training material
[ENISA CERT Exercises and Training](http://www.enisa.europa.eu/activities/cert/support/exercise)
* ENISA CERT Exercises and training material was introduced in 2008, in 2012 and 2013 it was complemented with new exercise scenarios containing essential material for success in the CERT community and in the field of information security. In this page you will find the ENISA CERT Exercise material, containing Handbook for teachers, Toolset for students and Virtual Image to support hands on training sessions. 





### <a name="talks">Presentations & Talks</a>
| ** Forensic Imager Tools: You don't have the Evidence - Shmoocon 2014** | https://www.youtube.com/watch?v=zYYCv21I-1I

[Ways to Identify Malware on a System Ryan Irving](http://www.irongeek.com/i.php?page=videos/bsidestampa2015/201-ways-to-identify-malware-on-a-system-ryan-irving)

[Investigating PowerShell Attacks - Ryan Kazanciyan and Matt Hastings - DEFCON22](https://www.youtube.com/watch?v=qF06PFcezLs)
* This presentation will focus on common attack patterns performed through PowerShell - such as lateral movement, remote command execution, reconnaissance, file transfer, etc. - and the sources of evidence they leave behind. We'll demonstrate how to collect and interpret these forensic artifacts, both on individual hosts and at scale across the enterprise. Throughout the presentation, we'll include examples from real-world incidents and recommendations on how to limit exposure to these attacks.

[Human Hunting](http://www.irongeek.com/i.php?page=videos/bsidessf2015/108-human-hunting-sean-gillespie) 
* Much of what appears to be happening in information security seems to be focused on replacing humans with magic boxes and automation rather than providing tools to augment human capabilities. However, when we look at good physical security we see technology is being used to augment human capabilities rather than simply replace them. The adversary is human so we are ultimately looking for human directed behaviors. If analysts don't know how to go looking for evil without automated detection tools then they are not going to be able to effectively evaluate if the detection tools are working properly or if the deployment was properly engineered. An over reliance on automated detection also puts organizations in a position of paying protection money if they want to remain secure. We should be spending more resources on honing analyst hunting skills to find human adversaries rather than purchasing more automated defenses for human adversaries to bypass.

[Finding Bad Guys with 35 million Flows, 2 Analysts, 5 Minutes and 0 Dollars](http://www.irongeek.com/i.php?page=videos/bsidesknoxville2015/103-finding-bad-guys-with-35-million-flows-2-analysts-5-minutes-and-0-dollars-russell-butturini)
* There are a lot of proof of concepts out there for building open source networks forensics analysis environments. Taking them into production in an enterprise? Another story entirely. This talk will focus on my journey into constructing a large scale Netflow security analytics platform for a large healthcare management company's complex environment on no additional budget. Important points to be covered were technology considerations, scalability, and how to quickly break the collected data down to find malicious activity on the network with minimal effort.





### <a name="anti">Anti-Forensics</a>

| ** Destroying Evidence Before Its Evidence** | https://www.youtube.com/watch?v=lqBVAcxpwio&spfreload=1
| **And That's How I Lost My Other Eye...Explorations in Data Destruction** | https://www.youtube.com/watch?v=-bpX8YvNg6Y

[Secure Deletion of Data from Magnetic and Solid-State Memory](http://static.usenix.org/publications/library/proceedings/sec96/full_papers/gutmann/index.html)

[usbkill](https://github.com/stemid/usbkill)
* A tool that shuts down your computer if USB devices change, for example if you unplug or plug-in a device. 






### <a name="mobile">Mobile Device Forensics</a>

#### <a name="android">Android Forensics</a>
[Android Forensics class - OpenSecurity Training](http://opensecuritytraining.info/AndroidForensics.html)
* This class serves as a foundation for mobile digital forensics, forensics of Android operating systems, and penetration testing of Android applications. 

[Androick](https://github.com/Flo354/Androick)
* Androick is a python tool to help in forensics analysis on android. Put the package name, some options and the program will download automatically apk, datas, files permissions, manifest, databases and logs. It is easy to use and avoid all repetitive tasks!


####<a name="ios">iOS Forensics</a>

http://www.forensicswiki.org/wiki/Apple_iPhone

http://www.iosresearch.org/

[iOSForensic](https://github.com/Flo354/iOSForensic)
* iosForensic is a python tool to help in forensics analysis on iOS. It get files, logs, extract sqlite3 databases and uncompress .plist files in xml.

[iOS Forensics Analyis(2012) SANS Whitepaper](https://www.sans.org/reading-room/whitepapers/forensics/forensic-analysis-ios-devices-34092)

[iOS Forensic Investigative Methods Guide](http://www.zdziarski.com/blog/wp-content/uploads/2013/05/iOS-Forensic-Investigative-Methods.pdf)




### <a name="pdf">PDF Forensics</a>

http://countuponsecurity.com/2014/09/22/malicious-documents-pdf-analysis-in-5-steps/

[PDF Forensics](http://countuponsecurity.com/2014/09/22/malicious-documents-pdf-analysis-in-5-steps/)



###< a name="photo">Photo Forensics</a>





[jhead](http://www.sentex.net/~mwandel/jhead/)
* Exif Jpeg header manipulation tool


### <a name="tools">Tools:</a>

Ghiro 




[StegExpose](https://github.com/b3dk7/StegExpose)
* StegExpose is a steganalysis tool specialized in detecting LSB (least significant bit) steganography in lossless images such as PNG and BMP. It has a command line interface and is designed to analyse images in bulk while providing reporting capabilities and customization which is comprehensible for non forensic experts. StegExpose rating algorithm is derived from an intelligent and thoroughly tested combination of pre-existing pixel based staganalysis methods including Sample Pairs by Dumitrescu (2003), RS Analysis by Fridrich (2001), Chi Square Attack by Westfeld (2000) and Primary Sets by Dumitrescu (2002). In addition to detecting the presence of steganography, StegExpose also features the quantitative steganalysis (determining the length of the hidden message). StegExpose is part of my MSc of a project at the School of Computing of the University of Kent, in Canterbury, UK.








### <a name="linux">Linux Forensics</a>







### <a name="windows">Windows Forensics</a>

[SANS CHEAT SHEET- Windows Artifact Analysis](https://uk.sans.org/posters/windows_artifact_analysis.pdf)

[How to parse Windows Eventlog](http://dfir-blog.com/2016/03/13/how-to-parse-windows-eventlog/)




#### Windows Forensics Tools

[NTDSXtract - Active Directory Forensics Framework](http://www.ntdsxtract.com/)
* Description from the page: This framework was developed by the author in order to provide the community
with a solution to extract forensically important information from the main
database of Microsoft Active Directory (NTDS.DIT).
[Did it Execute? - Mandiant](https://www.mandiant.com/blog/execute/)
* You found a malicious executable! Now you’ve got a crucial question to answer: did the file execute? We’ll discuss a few sources of evidence you can use to answer this question. In this post, we will focus on static or “dead drive” forensics on Windows systems. We will cover four main sources of evidence: Windows Prefetch, Registry, Log Files, and File Information.


[HowTo: Determine Program Execution](http://windowsir.blogspot.com/2013/07/howto-determine-program-execution.html)

[Kansa -A Powershell incident response framework ](https://github.com/davehull/Kansa)
* A modular incident response framework in Powershell. Note there's a bug that's currently cropping up in PowerShell version 2 systems, but version 3 and later should be fine


[License to Kill: Malware Hunting with the Sysinternals Tools](http://channel9.msdn.com/Events/TechEd/NorthAmerica/2013/ATC-B308)

[Windows Program Automatic Startup Locations](http://www.bleepingcomputer.com/tutorials/windows-program-automatic-startup-locations/)

[Collection of Windows Autostart locations](http://gladiator-antivirus.com/forum/index.php?showtopic=24610)

[Spotting the Adversary with Windows Event Log Monitoring - NSA](http://cryptome.org/2014/01/nsa-windows-event.pdf)
* NSA 70-page writeup on windows event log monitoring

[DPAPIck](http://dpapick.com/)
* This is a forensic tool to deal, in an offline way, with Microsoft Windows® protected data, using the DPAPI (Data Protection API

[Techniques for fast windows forensics investigations](https://www.youtube.com/watch?v=eI4ceLgO_CE)
* Look at sniper forensics, skip around, 18min has resources you want to grab for snapshots

[Know your Windows Processes or Die Trying](https://sysforensics.org/2014/01/know-your-windows-processes.html)
* Excellent quick reference on Windows proccesses with a focus on Win7. Good resource.

[WinPrefetchView v1.25](http://www.nirsoft.net/utils/win_prefetch_view.html)
* Each time that you run an application in your system, a Prefetch file which contains information about the files loaded by the application is created by Windows operating system. The information in the Prefetch file is used for optimizing the loading time of the application in the next time that you run it. WinPrefetchView is a small utility that reads the Prefetch files stored in your system and display the information stored in them. By looking in these files, you can learn which files every application is using, and which files are loaded on Windows boot. 
[BTA - AD Security Audit Framework](https://bitbucket.org/iwseclabs/bta)
* BTA is an open-source Active Directory security audit framework. Its goal is to help auditors harvest the information they need to answer such questions as:
Who has rights over a given object (computer, user account, etc.) ?
Who can read a given mailbox ?
Which are the accounts with domain admin rights ?
Who has extended rights (userForceChangePassword, SendAs, etc.) ?
What are the changes done on an AD between two points in time ?

[Claimsman](Claimsman logs all file handle creation on Windows systems, and logs to both a local file and centralized log management system.)

[FastIR Collector](https://github.com/SekoiaLab/Fastir_Collector)
* This tool collects different artefacts on live Windows and records the results in csv or json files. With the analyses of these artefacts, an early compromission can be detected.

[FastIR Collector on advanced threats](http://www.sekoia.fr/blog/wp-content/uploads/2015/10/FastIR-Collector-on-advanced-threats_v1.4.pdf)

[Windows Attribute changer](http://www.petges.lu/home/)

[Event Tracing for Windows and Network Monitor](http://blogs.technet.com/b/netmon/archive/2009/05/13/event-tracing-for-windows-and-network-monitor.aspx)
* "Event Tracing for Windows, (ETW), has been around for quite a while now as it was introduced in Windows 2000. It's basically instrumented logging that describes what a component is doing. Conceptually, it’s something like the proverbial printf("here1") concept used by programmers, but it is present in retail builds. When you enable logging in a component the result is an ETL (Event Trace Log) file. What’s new is that that Network Monitor can read any ETL file. And with the supplied parsers many network oriented ETW providers can be decoded."




### <a name="osx">OS X Forensics Tools</a>

[OS X Audiotr](https://github.com/jipegit/OSXAuditor)
* OS X Auditor is a free Mac OS X computer forensics tool.

[OS X Forensics Generals](https://davidkoepi.wordpress.com/category/os-x-forensics-10-8/)

[OSX Lion User Interface Preservation Analysis](https://digital-forensics.sans.org/blog/2011/10/03/osx-lion-user-interface-preservation-analysis#)

#### Bootkit Disk Forensics
[Part 1](http://www.malwaretech.com/2015/02/bootkit-disk-forensics-part-1.html)
[Part 2](http://www.malwaretech.com/2015/03/bootkit-disk-forensics-part-2.html)

### Chrome Book Forensics

[Chromebook Forensics](http://www.dataforensics.org/google-chromebook-forensics/)










