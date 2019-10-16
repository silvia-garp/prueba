
			   University of Lisbon
			   Faculty of Sciences


				NetGuardian
				    by
			      Paulo Sergio Mena
			 Ricardo Machado de Oliveira
			      Rui Santos Antonio

			   (netguard@di.fc.ul.pt)
		       (http://www.fc.ul.pt/software)



		 Welcome to NetGuardian version 2.0 beta #3
		 ------------------------------------------

    This README.TXT file contains important information about NetGuardian.  
 For the latest information about the NetGuardian program, read this file 
 in its entirety. 
    The NetGuardian is a SNMP package that includes a manager, an agent and
 a graphic analyser. It is a part of a project developed for a Computer 
 Science course at the 'Faculdade de Ciencias-Universidade de Lisboa'. These
 applications were developed in Borland C++ 3.1.     
    These applications use Mr.Ling Thio's and Mr.Dirk Wisse's WINSNMP.DLL 
 and cannot be run without it.  ( DNPAP group / J.P.M.vOorschot@et.tudelft.nl)
  

			TABLE OF CONTENTS
			-----------------
			1.  How to Get Help
			2.  System requirements
			3.  Installation
			4.  How to Use
			5.  What's New  
			6.  Bugs and limitations 
			7.  How to Get it
			8.  ToDo
			9.  Acknowledgements


			    1. HOW TO GET HELP
			    ------------------

    If you have any problems using the package, please read this  
 document entirely, which will probably help you to solve your problem 
 quickly.
    You also have a online help that will help you soving your problems.
    If you have an urgent problem that you cannot solve by yourself, you 
 can contact us at:  netguard@di.fc.ul.pt
    

			    2. SYSTEM REQUIREMENTS
			    ----------------------

    You should have a 386 (or better computer) with Microsoft's Windows 3.1 
 (or a later version) to run it on.
    It was tested with Trumpet Winsock version 1.0 Final Beta #5 and #6. It 
 also run under Microsoft TCP/IP 32.

				 
				3. INSTALLATION
				---------------

    To install NetGuardian, change your current drive to the one that has 
 the NETG2b3.ZIP file on it and type: 

	PKUNZIP -d [Source path\NETG2b3.ZIP] [Destination path] 

    Now, you have a directory with the NetGuardian program. 
    To use it in Windows, run it in Program Manager or create a new item 
 and browse it.
    You are now able to run the NetGuardian program, enjoy it.



				4. HOW TO USE
				-------------

    These applications have a user friendly interface and are simple to
 work with. We are going to describe globally the three applications.


 NETGUARDIAN

    It's a SNMP Manager simple to use. We will now refer to the options 
 available on the menu :
 
 FILE
 ----
  New     : Open a new window.
  Open    : Open configuration file, bitmap or a view file.
  Save    : Save configuration file and view file.
  Save As : Save view file with other name.
  Close   : Close an active window.
  Print   : Print the current view.
  Exit    : Exit Netguardian application.

 EDIT
 ----
  Cut   : Remove the selected item and put it in the buffer.
  Copy  : Place a copy of the item on the buffer.
  Paste : Insert an item from the buffer to the active window.

 SNMP
 ----
  System     : Shows a System request for the current machine.
  Interfaces : Shows a Interfaces request for the current machine.
  At         : Shows a At request for the current machine.
  Dump       : Shows a Dump request for the current machine.
  Info       : Shows a System, Interfaces, At or Dump request.

 NET
 ---
  Discovery         : Discovers all the items in the requested net.
  Traceroute        : Shows a graphic traceroute between two net points.
  Router Hierarchy  : Shows the router hierarchy.
  Ping Delay        : Choose a time interval between ping requests.
  Immediate Refresh : Test Snmp and Ping in all the view items imediatly.
  Periodic Refresh  : Choose a time interval to make a periodic refresh.

 ITEM
 ----
  Insert        : Inserts an item in the net.
  Delete        : Deletes an item in the net.
  Update        : Update an item in the net.
  Arrange Items : Arrange items in the window.
  Refresh       : Test Snmp and Ping in the current item.
  Grab Items    : Grabs a set of items and move it.
  Undo Move     : Undo a move.
  Move          : Enables and Disables the item drag and drop.

 OPTIONS
 -------
  Show/Hide Events     : Shows and Hides the Snmp and Ping events.
  Receive/Ignore Traps : Enables and Disables the reception of traps.
  Mibs                 : Insert or delete mibs.
  Start Graphic        : Shows a graphic performance for diferent kinds of 
			 Snmp variables.
  Start Agent          : Starts the Snmp Agent.
  Telnet               : Starts your favorite Telnet application !!
  Ftp                  : Starts your favorite Ftp application !!

 WINDOW
 ------
  Cascade       : Put the windows in a cascade mode.
  Tile          : Put the windows in a tile mode.
  Arrange icons : Arrange the icons.
  Close All     : Close all the windows.

 HELP
 ----
  NetGuardian : Shows help and teaches how to handle with the program.
  About...    : Displays the program information, Netguardian version number, 
		and the copyright.


 ShortCuts :

    There is a toolbar that allows you to use certain functions without accessing the    
 menus. It includes 15 self-explanatory buttons.

    Use the keys INSERT and DELETE in order to insert and delete 
 an item from the net.

    Clicking the mouse's left button on top of an item highlights it.

    The right mouse button is used to insert, update and delete connection.
 
    DoubleClicking the mouse's left button over an item allows the user to 
 make a SNMP request to that item. If it's a net it allows you to activate
 a view associated to this item.

    DoubleClicking the mouse's right button over an router item or Enter
 allows the user to choose a router interface and to enter that net.

    Use Shift+Delete to Cut, Control+Insert tp Copy and Shift+Insert to
 Paste.

    The F1 key gives you help about the application. 


 NETGUARDIAN AGENT

    The agent is prepared to answer simple requests for different kinds of
 managers.
    This application can be executed inside of the NETGUARDIAN application or
 externally. 
    There are three self-explanatory options avaiable on the menu (Start Agent,
 Stop Agent and Exit).

 NETGUARDIAN GRAPH

    The graphic is used to show the net performance, the scroll bar is used 
 to show the lastest recorded values. The values for the band and the band 
 numbers changes according to the variables values. When the window is 
 resizable the scale is automatically adapted.
    We will now refer to the options available on the menu :

 FILE
 ----
  Open : Opens a config file.
  Save : Saves the current configuration.
  Exit : Exits the application.

 SETUP
 -----
  Config    : Sets the hostname, IP address and community of the agent to 
	      query.
  Time      : Sets the update delay.
  Variables : Sets the variables you wish to monitor and to format their 
	      output.

 VIEW
 ----
  Legend : Enables or disables variables legend.
  Date   : Enables or disables date legend.
  Time   : Enables or disables time legend.
  Index  : Gets a recorded data interval.



				5. WHAT'S NEW
				-------------

    In this version we use the MDI frame windows. It allow the user to manage
 multiple views at the same time. A view can be opened,saved and closed. You
 can also print the active window in a printer (what you see is what you get).
 With multiple views you can copy items between windows.

    You have the option of print the dump results in a printer. We have 
 decided to replace the Physical Address by the IP Address in Interfaces. You 
 can also set a variable using System or Dump.        

    The net discovery was improved. There is an SNMP traceroute to help you
 obtaining a way from a machine to another. You can navigate between routers.
 It allow you to change the ping delay. You can refresh all the items in the
 view immediatle or peridically.

    We also improve the management of the items, in the last version the items
 were static. Now, they can be moved and changed. You can arrange the items in
 the view, refresh each one. You can grab a set of items and move them to 
 another place in the view. It was also useful to enable or disable sometimes 
 the movement.

    This new version has an event report that will be useful to obtain
 information about the states of the items.

    The SNMP Graphic Analyser is more powerfull than the one in the first 
 version. It can save data by a certain time, for you to see the latest 
 requests. You can monitor for one to five variables from the interfaces
 group at the same time.

    We developed a SNMP Agent with the basic variables (system,interfaces,at).

    This version has an online help that can be useful to obtain some 
 information about the application. This was a great improvement.
     
    Finally the WINSNMP.DLL has some modifications, because it had some memory
 problems. In the last version the trap unregistration wasn't properly 
 implemented, now it is correct. 
   

			   6. BUGS AND LIMITATIONS
			   -----------------------

    This application runs over Microsoft Windows 3.1 or better, we have 
 noticed some problems with Windows NT. We recommend more than a 4 Mb RAM/SWAP
 memory.

    However, due to the unavailability of RAW_SOCKETS in Microsoft TCP/IP 32,
 this application simulates a ping request using an UDP datagram sent to the
 port 7 (echo service). 

    The traceroute uses the SNMP routing tables, doesn't use ICMP. For real
 answers all the machines discovered must have a SNMP agent running. 

    There are some problems with scroll and we didn't found the cause of them.

    In the last version we didn't noticed a big memory problem with the
 WINSNMP.DLL. In this verison we have solved part of the problems, there is 
 one that we don't solve. When we send a SNMP request some memory is lost. To 
 solve this problem we test the memory when some SNMP response is received, if 
 the memory is critical we stop the application execution.

    Should you bump into further bugs (wich is highly unlikely !) please
 contact us. You can do this by E-mail, letter, phone, fax etc...
    Please be shure to include a full description of the problem encountered, 
 the system you are running on, memory available to Windows, Windows Version,     
 mode it is running in, display information, and any other information you
 consider relevant.

    You can reach us at :

    NetGuardian
    Faculdade de Ciencias da
    Universidade de Lisboa
    (Departamento de Informatica)
    Campo Grande - Bloco C5
    1700 LISBOA
    PORTUGAL

    Tel: +351 1 7510003
    Fax: +351 1 7577831


			    7. HOW TO GET IT
			    ----------------
			    
    NETG2b3.ZIP is available by anonymous FTP from ftp.fc.ul.pt at 
    /pub/networking/snmp/netg2b3.zip


				8. TODO
				------- 

    This version has some things that can be improved. We'll enumerate the 
 list of items to develop in latter versions:
  
    -An ICMP traceroute, the actual one uses the SNMP routing tables.

    -An agent with real values, the current agent has only a real value 
 obtained  by it self, this value is the sysUpTime. The other values are in
 the mib file used by the agent and inserted by the user.

    -Run a script when some kind of event occur.

    -Solve the scroll problem.

    -Solve the WINSNMP memory problem.
     

			    9. ACKNOWLEDGEMENTS
			    -------------------

    We would like to thank Mr.Ling Thio and Mr.Dirk Wisse for the use of 
 WINSNMP.DLL without which we would not have been able to develop this 
 application.
    We would also like to thank our colleagues for the hints and tips they 
 might have given us.
    And, last but not the least, we would like to thank Mr.Carlos Picoto, our 
 teacher, who introduced us to the wonderful world of SNMP, and without 
 whose pressure and patience we would never have completed this assignement. 
 


		That's all folks ...

