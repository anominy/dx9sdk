# Legacy DirectX SDK
This is collection of headers & libraries of legacy DirectX 9 SDK.

## Install
To install this package, download the full repository and place it in your workspace. I typically create an additional `/ext/` directory for external code. In my case, I add `-I./ext/dx9sdk/inc` to my compilation flags to include the necessary headers. When linking the libraries, specify the library path as `-L./ext/dx9sdk/lib/x86`. You can then import the library either by using `#pragma` directives or by adding the appropriate `-l` flag to your compiler options.

## Include
```c
#include <dxsdk/d3d9.h>
#include <dxsdk/d3dx9.h>
```

## Import
```c
#pragma comment(lib, "dxsdk/dxguid.lib")
#pragma comment(lib, "dxsdk/d3d9.lib")
#pragma comment(lib, "dxsdk/d3dx9.lib")
```
