# Envia — Third-Party Notices

**Last updated: October 2026**

Envia is proprietary software developed by Nahid. This document lists third-party package references found in the supplied `Envia.csproj`. It is a project-file inventory, not yet a complete audit of every file redistributed in the final installer. The exact shipped artifacts and all required notices must be checked before release.

The proprietary Envia license applies only to materials owned by Nahid. Third-party components remain subject to their respective licenses. Nothing in the Envia EULA or proprietary license modifies or restricts rights granted by applicable third-party licenses.

## NuGet package references in Envia.csproj

| Component | Version in project file | Notes |
|---|---:|---|
| CommunityToolkit.Mvvm | 8.4.2 | Microsoft Community Toolkit component |
| CommunityToolkit.WinUI.Animations | 8.2.251219 | Windows Community Toolkit component |
| H.NotifyIcon.WinUI | 2.3.0 | Windows tray icon component |
| Microsoft.Extensions.Configuration.UserSecrets | 6.0.1 | Microsoft.Extensions component |
| Microsoft.Extensions.DependencyInjection | 10.0.10 | Microsoft.Extensions component |
| Microsoft.Graphics.Win2D | 1.4.0 | Win2D graphics component |
| Microsoft.Windows.SDK.BuildTools | 10.0.28000.2270 | Windows SDK build tools |
| Microsoft.WindowsAppSDK | 2.2.0 | Windows App SDK |
| NAudio | 2.3.0 | Audio library |
| System.Management | 10.0.10 | .NET/WMI management APIs |

This list is transcribed from the supplied project file. It does not by itself establish which package assemblies or runtime components are included in a particular published build.

## Bundled Night Light Utility — win-nightlight-cli

**Component:** `win-nightlight-cli` (`Tools\\NightLight\\wnl.exe`)  
**Author:** Kevin Xiao  
**Copyright:** Copyright (c) 2025 Kevin Xiao  
**License:** MIT License  
**Source:** https://github.com/kvnxiao/win-nightlight-cli

Envia bundles this third-party utility to support Windows Night Light functionality. Its MIT license permits use and redistribution, subject to preservation of the copyright and permission notice. The license below applies to the utility, not to Envia's proprietary code.

### Full MIT License — win-nightlight-cli

MIT License

Copyright (c) 2025 Kevin Xiao

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## win-nightlight-cli (NightLight utility)

- **Project:** [kvnxiao/win-nightlight-cli](https://github.com/kvnxiao/win-nightlight-cli)
- **Copyright:** Copyright (c) 2025 Kevin Xiao
- **License:** MIT License
- **Bundled utility:** `Tools\NightLight\wnl.exe`

The following license notice is reproduced from the text supplied for this utility:

```text
MIT License

Copyright (c) 2025 Kevin Xiao

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## Microsoft and .NET components

The project targets .NET 8 for Windows and enables the self-contained Windows App SDK deployment option. The published application may therefore include runtime components beyond the direct package references. Check the actual publish output and the applicable Microsoft/.NET notices for the exact distribution.

## License information and verification

Before publishing each release:

1. Check each package's upstream license and required attribution for the exact version used.
2. Check transitive dependencies in the restored NuGet dependency graph, not only direct references in the project file.
3. Inspect the final publish output and installer payload to determine which components are redistributed.
4. Include the required license texts and notices. The bundled win-nightlight-cli MIT license is reproduced above; verify other packages' notice requirements.
5. Update this document when package versions or shipped components change.

Useful upstream project pages include:

- CommunityToolkit: https://github.com/CommunityToolkit
- H.NotifyIcon: https://github.com/HavenDV/H.NotifyIcon
- Win2D: https://github.com/microsoft/Win2D
- Windows App SDK: https://github.com/microsoft/WindowsAppSDK
- NAudio: https://github.com/naudio/NAudio
- .NET: https://github.com/dotnet/runtime

These links are provided for locating upstream information. The applicable license is the license shipped with or published for the exact component version.

## Important notice

The presence of third-party components does not grant permission to modify or redistribute Envia's proprietary code or branding. Conversely, the proprietary Envia license does not remove or restrict rights granted by licenses applicable to third-party components.

Envia — developed by Nahid  
https://github.com/Hajime-GG

Copyright (c) 2026 Nahid.
