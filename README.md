# SIM800L-AT-Command
SIM800L   < == > Arduino
pin TX	  < == > pin 10 (SoftwareSerial RX)
pin RX	  < == > pin 11 (SoftwareSerial TX)
pin RST   < == > pin 13
 
pin VCC   < == > Batteray Li-po 18650 3,7V atau step down dari 5V Arduino
pin GND   < == > pin GND 

Description
AT+CREG AT command gives information about the registration status and access technology of the serving cell.
Possible values of registration status are,
0 not registered, MT is not currently searching a new operator to register to
1 registered, home network
2 not registered, but MT is currently searching a new operator to register to
3 registration denied
4 unknown (e.g. out of GERAN/UTRAN/E-UTRAN coverage)
5 registered, roaming
6 registered for "SMS only", home network (applicable only when indicates E-UTRAN)
7 registered for "SMS only", roaming (applicable only when indicates E-UTRAN)
8 attached for emergency bearer services only (see NOTE 2) (not applicable)
9 registered for "CSFB not preferred", home network (applicable only when indicates E-UTRAN)
10 registered for "CSFB not preferred", roaming (applicable only when indicates E-UTRAN)
Possible values for access technology are,
0 GSM
1 GSM Compact
2 UTRAN
3 GSM w/EGPRS
4 UTRAN w/HSDPA
5 UTRAN w/HSUPA
6 UTRAN w/HSDPA and HSUPA
7 E-UTRAN
 
Pastikan untuk hasil AT+CREG? adalah 1,1 untuk memastikan telah teregistrasi dan mendukung GPRS.
