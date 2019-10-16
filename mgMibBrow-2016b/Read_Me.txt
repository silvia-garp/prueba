This is the "Read_Me.txt" file distributed with MG-SOFT MIB Browser 2016
Professional Edition with MIB Compiler, MIB Explorer and Visual
MIB Builder.

Copyright (C) 1995-2016  MG-SOFT Corporation.
All rights reserved.

========================================================================
Table of Contents
-----------------

1. About the Software
2. What's New in this Version
3. Important Licensing Information
4. Installing the Software
5. MG-SOFT Corporation on the Internet
6. Ordering the Software
7. Licensing Agreement
8. Contacting MG-SOFT Corporation


========================================================================
1. About the Software
---------------------

MG-SOFT MIB Browser Professional Edition with MIB Compiler is an 
SNMP MIB Browser available for 32-bit and 64-bit Microsoft Windows 
operating systems (Windows Vista, Windows Server 2008, Windows 7, 
Windows Server 2012, Windows 8.x, Windows 10), for Linux operating 
systems running on Intel x86 and x86_64 architectures (Red Hat,  
Ubuntu, SuSe...), for Apple Mac OS X operating systems (Intel x86_64 
platform), as well as for Solaris operating systems (Intel x86 and 
SPARC platforms).

MIB Browser lets you monitor and manage any SNMP device on the network 
(i.e., servers, routers, switches, modems, printers,...) by using the 
SNMPv1, SNMPv2c and SNMPv3 protocols over UDP and TCP in IPv4 and IPv6 
networks. MIB Browser supports also Diffie-Hellman key exchange model, 
so that DOCSIS-based SNMPv3 agents (e.g., cable modems, CMTS, set-top 
boxes etc.) can be seamlessly contacted and managed. Furthermore, besides 
the standard SNMPv3 User-based Security Model (USM), MG-SOFT MIB Browser 
now implements also the Transport Security Model (TSM), and supports 
SNMPv3 over TLS and SNMPv3 over DTLS protocol, as specified in RFC 6353.

MIB Browser allows you to perform the SNMP Get, SNMP GetNext, SNMP
GetBulk and SNMP Set operations. Besides, the software lets you capture
and display SNMP Trap and SNMP Inform packets that are sent from
arbitrary SNMP devices or applications on the network.

MIB Browser can monitor several SNMP devices simultaneously and contains
features like SNMP Table viewer, SNMP Table 'editor', logging capabilities,
real-time graphical presentation of queried numerical values, scan for
implemented MIBs in agents, comparison of SNMP agent snapshots, management
of SNMPv3 USM users on remote SNMP agents, etc.

Generic SNMP Trace window displays SNMP messages exchanged between MIB
Browser and SNMP agents. SNMP messages are displayed in raw hexadecimal
dump format as well as in the decoded, human-readable format. Therefore,
the Generic SNMP Trace window is particularly useful for debugging when
developing an SNMP agent and for resolving problems when agents do not
properly respond to MIB Browser's queries.

MIB Browser lets you take a snapshot of an SNMP agent on the network
and then simulate this agent on the computer where MIB Browser runs.
Simulating means that MIB Browser runs a separate process, which listens
for SNMP queries on a selected network interface and port and responds
to SNMP queries, returning exactly the same OIDs and values as the
"real" SNMP agent did at the time of taking its snapshot.

The enclosed MIB Compiler lets you compile any standard or vendor
specific MIB file. The compiled MIB file can then be loaded and
utilized by MIB Browser. Generally, MIB files are supplied by
vendors of SNMP manageable devices, and contain description of
the manageable object hierarchy and object attributes in the SNMP
device. In other words, MIB files serve as roadmaps for managing
SNMP devices.

The enclosed MIB Explorer is powerful and intuitive software for
comparing MIB definition files and for searching for dependencies
between them. With the user-friendly interface for specifying query
conditions, the user can search for any values and constructs in MIB
definitions. Besides, the software can create various reports and
export MIB definitions to HTML, DHTML, YANG, PDF, XML, MOSY, and TXT 
file formats.

The enclosed Visual MIB Builder is a software with which you can design
and edit MIB definition files in a highly productive way. Due to its
intuitive graphical drag-and-drop environment, where most of edits are
visual, you do not need much knowledge about ASN.1 syntax or MIB module
definition language to create MIBs. This means the software is suitable
for beginners in SMI. On the other hand, due to full support for SMIv1
and SMIv2 standards and advanced features like SMI revision control,
Visual MIB Builder is also suitable for experienced SMI gurus. MIB
definition module can be designed within minutes, no mater if it
contains table definitions or not. MIB modules designed with Visual
MIB Builder will be syntactically and semantically correct and will
compile with any SMI compliant MIB Compiler.


This product includes Apache Xerces XML Parser for C++ software.
This product includes software developed by the OpenSSL Project for 
use in the OpenSSL Toolkit (http://www.openssl.org/). This product 
includes cryptographic software written by Eric Young (eay@cryptsoft.com). 
This product includes software written by Tim Hudson (tjh@cryptsoft.com).
For full licensing information refer to the "THIRD-PARTY-LICENSES.TXT"
file located in the MIB Browser's \Doc subfolder.


========================================================================
2. What's New in this Version 
-----------------------------

Here is a brief description of the major new functions and features in
MG-SOFT MIB Browser 2016 Professional Edition release:

* Support for Microsoft Windows 10. 
  MIB Browser as well as other bundled applications (MIB Compiler, 
  MIB Builder and MIB Explorer) have been tested to successfully 
  install and run also on the latest Microsoft Windows operating 
  system - Windows 10. 

* Transport Security Model (TSM) with TLS and DTLS secure transports.
  Besides the standard SNMPv3 User-based Security Model (USM), MG-SOFT 
  MIB Browser now implements also the Transport Security Model (TSM), 
  and supports SNMPv3 over TLS and SNMPv3 over DTLS protocol, as 
  specified in RFC 6353. All retrieval and modification operations
  supported by MIB Browser can now be performed also by using SNMP 
  over (D)TLS. (D)TLS provides authentication, data integrity, and 
  privacy at the transport layer by establishing a secure "tunnel" 
  between two SNMP entities, over which SNMP messages are exchanged. 
  SNMP over (D)TLS enables leveraging the organization's existing 
  X.509 public key infrastructure for SNMP management and can be 
  configured to employ stronger security than SNMPv3 USM.

* SNMP over TCP.
  In addition to connectionless UDP transport protocol, MIB Browser
  now supports performing all SNMP operations also over connection-
  oriented TCP transport that ensures reliable data delivery,
  automatically handling packet retransmissions, reordering and 
  errors on the transport level. TCP transport can be used with 
  all versions of the SNMP protocol supported by MIB Browser
  (SNMPv1, SNMPv2c, SNMPv3 USM, and SNMPv3 TSM (via TLS)). 
  Using SNMP over TCP may be more efficient than SNMP over UDP, 
  especially when transferring bulk data using large SNMP packets.
  
* MIB tree node colors reflect the node access type.
  By default, the MIB tree node names are now colored according to 
  the node access/max.access value defined in the MIB (e.g. read-only, 
  read-write, read-create, not-accessible,...). This way, you can  
  tell at a glance which nodes (i.e., corresponding MIB object 
  instances) are writable, creatable, not accessible, etc., without 
  having to examine the detailed node properties to obtain this 
  information. Node access colors can be adjusted to your taste in 
  the program preferences. 
  
* DPI-aware GUI for best user experience on modern displays (4K-ready).
  MIB Browser and all bundled applications (Visual MIB Builder, 
  MIB Explorer, MIB Compiler) are now "aware" of the system display
  DPI settings (on Windows and Mac OS) and automatically scale 
  the size of their GUI components (buttons, icons) and text 
  accordingly to achieve the best visibility and usability also                  
  on today's high pixel density (HiDPI) displays. 

* Updated and enhanced user manuals and help files with numerous hints
  and usage examples will help you get the most from MG-SOFT's MIB
  Browser Pro. and other bundled MG-SOFT applications.

Besides, a number of minor improvements have been implemented in all
included applications, and all known problems occurring in older versions
have been fixed for this release.


========================================================================
3. Important Licensing Information
----------------------------------

This software package installs the following
MG-SOFT's applications:

* Visual MIB Builder,
* MIB Explorer,
* MIB Browser Professional Edition, and
* MIB Compiler.

Visual MIB Builder and MIB Explorer are available in
Standard and Developer's Edition, while MIB Browser
is available in the following five editions:

* MIB Browser Professional SNMPv1/v2c Edition
  (supporting SNMPv1 and SNMPv2c protocols).

* MIB Browser Professional SNMPv3 Edition
  (supporting SNMPv1, SNMPv2c and SNMPv3 USM protocols).

* MIB Browser Professional DOCSIS/DH Edition
  (supporting SNMPv1, SNMPv2c and SNMPv3 USM protocols
   and the Diffie-Hellman key exchange extension to USM
   for managing DOCSIS-based SNMPv3 agents. This edition
   support also SNMPv3 TSM with TLS and DTLS transports.
   Besides, this edition supports IPv6 protocol).

* MIB Browser Professional Developer's Edition
  (supporting SNMPv1, SNMPv2c and SNMPv3 USM protocols
   and the Diffie-Hellman key exchange extension to USM
   for managing DOCSIS-based SNMPv3 agents. This edition
   support also SNMPv3 TSM with TLS and DTLS transports, 
   as well as IPv6 protocol. Besides, this edition includes
   the Generic SNMP Trace debugging feature).

* MIB Browser Professional Simulator Edition
  (supporting SNMPv1, SNMPv2c and SNMPv3 USM protocols
   and the Diffie-Hellman key exchange extension to USM,
   SNMPv3 TSM with TLS and DTLS transports, IPv6 protocol,
   and the Generic SNMP Trace debugging option.   
   Furthermore, this edition incorporates the
   SNMP Agent Simulator feature).

Which of these applications and which features will be
available in the installed software, depends on the
purchased license.


========================================================================
4. Installing the Software
--------------------------

Make sure to install the latest version of the software as available
from http://www.mg-soft.com/download.html

You need administrative user privileges to install the software.

To install the software, unzip the distribution zip file. This 
software distribution package contains installers for 32-bit (x86) 
and 64-bit (x86_64) build of MG-SOFT MIB Browser Professional 
Edition with MIB Compiler for Windows.

- On 32-bit Windows operating systems install the 32-bit version 
  of the software by running the "setup-32.exe".

- On 64-bit Windows operating systems install either 64-bit or 
  32-bit version by running "setup-64.exe" or "setup-32.exe".

Follow the on-screen guidelines. You must reboot the computer if 
the setup procedure prompts you to do so.

In case of problems, please check the "Trouble_Shooting.txt" document 
located in the MIB Browser\Doc folder.


========================================================================
5. MG-SOFT Corporation on the Internet
--------------------------------------

* MG-SOFT Web Site              http://www.mg-soft.si/
* MG-SOFT Products              http://www.mg-soft.si/products.html
* MG-SOFT Sales Page            http://www.mg-soft.si/sales.html
* MG-SOFT Support Page          http://www.mg-soft.si/support.html
* MG-SOFT Corp. Profile         http://www.mg-soft.si/profile.html

* MIB Browser Professional      http://www.mg-soft.si/mgMibBrowserPE.html
* Trap Ringer Professional      http://www.mg-soft.si/tringer.html
* Net Inspector                 http://www.mg-soft.si/netinsp.html
* NETCONF Browser Professional  http://www.mg-soft.si/mgNetConfBrowser.html
* Visual YANG Designer Pro.     http://www.mg-soft.si/mgYangDesigner.html
* Visual MIB Builder            http://www.mg-soft.si/builder.html
* MIB Explorer                  http://www.mg-soft.si/mgMibExplorer.html
* SNMP Master Agent             http://www.mg-soft.si/agent.html
* SNMP Agent Simulator          http://www.mg-soft.si/mgSnmpAgentSimulator.html
* SNMP Proxy Agent              http://www.mg-soft.si/mgSnmpProxyAgent.html

Announcing New Releases
-----------------------
Visit http://www.mg-soft.si/news_announce.html for the latest
information about the scheduled software releases and updates.

Evaluation Software
-------------------
Evaluation software is available for downloading from MG-SOFT's web
site at http://www.mg-soft.si/download.html

To apply for a 30-day evaluation license key, fill in and submit the
on-line order form at http://www.mg-soft.si/evalKeyReq.html

For immediate software release notifications, subscribe to our mailing
list at http://www.mg-soft.si/maillist.html


========================================================================
6. Ordering the Software
------------------------

To obtain the latest ordering and licensing information, visit
http://www.mg-soft.com/sales.html or contact <sales@mg-soft.com>.

For details on licensing arrangements for licensing MG-SOFT's
software products visit http://www.mg-soft.com/licenseTypes.html


========================================================================
7. Licensing Agreement
----------------------

Check the "License_Agreement.txt" file that was installed with the
software. Also, check the "License_Types.txt" file or visit
http://www.mg-soft.com/licenseTypes.html for details on various
licensing arrangements for licensing MG-SOFT's software products.
Contact <sales@mg-soft.com> for additional information.


========================================================================
8. Contacting MG-SOFT Corporation
---------------------------------

For the latest information about our products, check our WEB
site at http://www.mg-soft.com/ or contact us directly.

You can subscribe to our mailing lists on-line by submitting the
application form at http://www.mg-soft.com/maillist.html


For additional information about MG-SOFT Corporation, please
contact the following address:

MG-SOFT Corporation          Phone:    +386 2 2506565
Strma ulica 8                Fax:      +386 2 2506566
2000 Maribor                 E-mail:   info@mg-soft.com
Slovenia                     Internet: http://www.mg-soft.com/


========================================================================
