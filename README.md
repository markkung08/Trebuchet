# Trebuchet
MS15-076 (CVE-2015-2370) Privilege Escalation
Copies a file to any privileged location on disk

Compiled with VS2015, precompiled exe in Binary directory

Usage: trebuchet.exe C:\Users\Bob\Evil.txt C:\Windows\System32\Evil.dll

This is a lightly modified Proof of Concept by James Forshaw with Google, found here: https://code.google.com/p/google-security-research/issues/detail?id=325

CreateSymlink tool was written by James Forshaw found here:
https://github.com/google/symboliclink-testing-tools

Notes:
 - Microsoft.VisualStudio.OLE.Inerop.dll must be in the same directory
 - Exploit can only be one once every 2-3 minutes. This is because RPC can be help up by LocalSystem
 - Tested on x64/x86 Windows 7/8.1

