# Intelliroot's ProcessHunting Toolkit
Process hunting Toolkit is toolkit capable of hunting down malicious processes on Windows. It can be used for malware analysis, threat hunting and incident Response.

The toolkit contains the following three binaries:
1 - ProcMemScanner_Beta.exe - hunts for malicious pattern’s in processes
2 - ProcAnomalyScanner_Beta.exe- Detect suspicious processes on basic process attributes
3 - Injected_Code_Hunter_x64.exe/Injected_Code_Hunter_x86.exe - hunts all the processes for code injections

All the above executable need to be run in Administrator mode. Below is the description of the exe's.

Testing ProcMemScanner_Beta.exe
=================================
ProMemScan requires two files to work: "whitelist_process.txt"  and "sign.dat". To initially test the scanner, you need to paste this string "ScannerTestX5O-TEST-Mem" into the notepad. Then run this tool in administrator mode. Notepad Process should be detected as "notepad and see if the notepad process is detected as "mal_scanner_test".

See more details of the tool in our blog: https://intelliroot.com/blog
