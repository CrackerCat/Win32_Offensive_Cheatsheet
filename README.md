# Win32_Offensive_Cheatsheet
Win32 and Kernel abusing techniques for pentesters



**Windows Binary Documentation**

- [PE structure⏳](#pe-headers)
 - [PE Headers ⏳](#pe-headers)
 - [Export Address Table (EAT) ⏳]()
  - [Resolve function address ⏳]()
    - [Using address (Obvious :D)]()
    - [Using ordinal number]()
    - [Using function name]()
 - [Import Address Table (IAT) ⏳]()
 - [Import Lookup Table (ILT) ⏳]()



**Execute some binary**

- [Classic shellcode execution⏳]()
- [DLL execute ⏳]()
- [Reflective DLL execution ⏳]()
- [RAW file to PE ⏳]()


**Code injection techniques**

- [CreateRemoteThread injection ⏳]()
- [Process Hollowing ⏳]()
- [APC technique⏳]()
 - [Early Bird ⏳]()
- [Reflective DLL Injection ⏳]()
- [Dll injection ⏳]()
- [Process Doppelganging ⏳]()
- [Fibers ⏳]()
- [CreateThreadPoolWait ⏳]()
- [Thread Hijacking ⏳]()
- [MapView code injection ⏳]()
- [Module Stomping ⏳]()
- [Function Stomping ⏳]()
- [Complete PE injection in remote process ⏳]()

**Hooking techniques**
- [Inline hooking ⏳]()
- [IAT hooking ⏳]()


**AV Bypass techniques (Signature based)**

- [Call and Strings obfuscation ⏳]()
- [Manual function resolves ⏳]() 
- [Win32 API Hashing ⏳]()


**EDR/Endpoint bypass**

- [Direct syscall ⏳]()
- [High level languages ⏳]()
- [Patch inline hooking ⏳]()
- [Patch ntdll hooking ⏳]()
- [Detect hooks ⏳]()
- [Patch ETW ⏳]()
- [Sandbox bypass ⏳]()
- [Debugging Bypass ⏳]()
- [Patch Kernel callbacks ⏳]()
- [VirtualProtect techniques ⏳]()
- [Fresh copy unhook ⏳]()
- [Hell's Gate ⏳]()
- [Heaven's Gate ⏳]()
- [PPID spoofing ⏳]()


**Driver Programming basics**

- [General concepts ⏳]()
- [Driver entry ⏳]()
- [IO (Input/Output) ⏳]()
- [Symlinks ⏳]()
- [Communicate with driver ⏳]()
- [Client code to kernel code ⏳]()
- [Driver signing (Microsoft) ⏳]()

**Offensive Driver Programming**

- [Process protection removing ⏳]()
- [Patch kernel callback (dev way) ⏳]()
- [Integrity and privileges levels ⏳]()
- [Enable SeDebug privilege ⏳]()

**Using Win32 API to increase OPSEC**

- [Persistence ⏳]()
 - [Scheduled Tasks ⏳]()
- [Command line spoofing ⏳]()

<br>
<br>

  
    
      
       

# Useful tools and Websites/Books


**Websites/Books**

:skull: https://www.ired.team/ (Awesome red team cheatsheet with great code injection notes)

:skull: https://undocumented.ntinternals.net/ (Undocumented NT functions)

:skull: https://docs.microsoft.com/en-us/windows/win32/api/ (Microsoft Official Doc)

:skull: Windows Kernel Programming - Pavel Yosifovich
<br>
<br>

## PE Headers

```
DOS_HEADER : First Header of PE, contains MS DOS message ("This programm cannot be run in DOS mode...."), MZ Header (Magic bytes to identify PE) and some stub content.
```
