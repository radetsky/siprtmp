I have patched the siprtmp.py to get the feature. 
Gateway must connect only to one SIP server anycase. 
Address to connect must be given in command line with -s --sipserver argument. 
If address of SIP server given, gateway do not register any user to SIP server, 
just bind and accept UDP socket. 
When call is arrived from RTMP-client we substitute 'rtmpgw' as username to make a call.
I forget to check SIP server in unregister method - it's bad, but it's work. 


