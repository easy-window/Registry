# Registry Libraries
A library for read and write registry based on the Windows API.

## Usage

```cpp
#include "Registry.h"
using namespace Easy;

Registry reg;

Registry registry(Registry::KEY_LOCAL_MACHINE);
CString sKey = _T("Userinit"), sData;
CString sOption = _T("SOFTWARE\\Microsoft\\Windows NT\\CurrentVersion\\Winlogon");

registry.Read(sOption, sKey, sData);    // C:\Windows\system32\userinit.exe,
registry.Write(sOption, sKey, sData);


```
