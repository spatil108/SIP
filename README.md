# SIP

EE 284 San Jose State University Project - Professor Balaji

This application will make call to a destination URI specified in the command line argument, and establish audio communication with remote party once the call is connected.

Below is the procedure, how to run the program, but if throws an error of pjsua import error and you are having trouble installing pjsua, you need to install the dependancies and install the pjsua library.
Steps to install dependencies:
http://stackoverflow.com/questions/11094718/error-command-gcc-failed-with-exit-status-1-while-installing-eventlet
Install Pjsip
http://lists.pjsip.org/pipermail/pjsip_lists.pjsip.org/2013-March/015917.html


Now you can call another softphone (such as ​pjsua) by specifying the SIP URI as command line argument. For example, if the other softphone is on "sip:192.168.0.15:5080", run the program as follows:

 python simplecall.py sip:192.168.0.15:5080
 
 
 Sample Output:
 
 13:05:25.718 os_core_win32. pjlib 0.9.0-trunk for win32 initialized
 13:05:25.718 sip_endpoint.c Creating endpoint instance...
 13:05:25.718          pjlib WinNT IOCP I/O Queue created (00D230A0)
 13:05:25.734 sip_endpoint.c Module "mod-msg-print" registered
 13:05:25.734 sip_transport. Transport manager created.
 13:05:25.968   pjsua_core.c pjsua version 0.9.0-trunk for win32 initialized
Call is  CALLING last code = 0 ()
Press <ENTER> to quit
Call is  EARLY last code = 180 (Ringing)
Call is  CONNECTING last code = 200 (OK)
Hello world, I can talk!
Call is  CONFIRMED last code = 200 (OK)
Call is  DISCONNCTD last code = 200 (Normal call clearing)

