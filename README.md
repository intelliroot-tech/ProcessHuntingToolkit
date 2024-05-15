# Intelliroot's ProcessHunting Toolkit
Process hunting Toolkit is toolkit capable of hunting down malicious processes on Windows.
It can be used for malware analysis, threat hunting and incident Response.
**Note**: All the the exe's in the toolkit needs to be executed in administrator mode

The toolkit contains the following three binaries:<br />
1 - **ProcMemScanner_Beta.exe** - hunts for malicious pattern’s in processes
      `` - This tool can be used to scan the system for malicious processes 
       ``- If code is injected into clean process then the process is detected as malware
       ``- tool should be executed in administrator mode 
      `` - tool can be used for classifying malwares and used for threat attribution 
       ``- It can be used in sandboxes and endpoint 
       ``- Malware signatures in sign.dat file. We would be updating the signature files
       ``- signature in "sign.dat" has signature for following malwares 
              ``- AgentTesla 
              ``- Blacknet RAT
              ``- XWorm RAT
              ``- Redline Stealer
              ``- Stealc stealer
              ``- Formbook
              ``- LummaStealer
        -

2 - **ProcAnomalyScanner_Beta.exe**- Detect suspicious processes on basic process attributes
    - Finds processes which violates basic rules of windows processes
    
3 - **Injected_Code_Hunter_x64.exe/Injected_Code_Hunter_x86.exe** - hunts all the processes for code injections
    - Detects and dumps injected code in live system

All the above executable need to be run in Administrator mode. Below is the description of the exe's.

Testing ProcMemScanner_Beta.exe
=================================
ProMemScan requires two files to work: "whitelist_process.txt"  and "sign.dat". To initially test the scanner, you need to paste this string "ScannerTestX5O-TEST-Mem" into the notepad. Then run this tool in administrator mode. Notepad Process should be detected as "notepad and see if the notepad process is detected as "mal_scanner_test".

See more details of the tool in our blog: https://www.intelliroot.com/blog/process-hunting-toolkit
