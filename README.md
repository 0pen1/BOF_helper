# Beacon Object File (BOF) Creation Helper

修复原项目中失效的url，具体可以参考原项目链接：https://github.com/dtmsecurity/bof_helper

**依赖**

Use *install.sh* to check and sort this but all that is required is the following:

- python3
- requests python library
- git clone [https://git.code.sf.net/p/mingw/mingw-org-wsl](https://git.code.sf.net/p/mingw/mingw-org-wsl) mingw-mingw-org-wsl to current directory.

**使用方法**

```
python3 bof_helper.py <API Method>
```

**示例**

```bash
python3 bof_helper.py DsGetDcNameA
██████╗  ██████╗ ███████╗
██╔══██╗██╔═══██╗██╔════╝
██████╔╝██║   ██║█████╗
██╔══██╗██║   ██║██╔══╝
██████╔╝╚██████╔╝██║
╚═════╝  ╚═════╝ ╚═╝
BOF Helper by @dtmsecurity

[Library] DsGetDcNameA is probably in NetApi32

[Declaration] DWORD WINAPI DsGetDcNameA(LPCSTR, LPCSTR, GUID*, LPCSTR, ULONG, PDOMAIN_CONTROLLER_INFOA*);

[BOF Helper]
DECLSPEC_IMPORT DWORD WINAPI NETAPI32$DsGetDcNameA(LPCSTR, LPCSTR, GUID*, LPCSTR, ULONG, PDOMAIN_CONTROLLER_INFOA*);
```

**原项目链接**

- https://github.com/dtmsecurity/bof_helper

