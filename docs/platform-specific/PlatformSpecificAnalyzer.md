---
title: UWP Platform Specific Analyzer
author: hermitdave
description: Platform Specific Analyzer is a Roslyn analyzer that analyzes and suggests code fixes to ensure that any version / platform specific API are guarded by correct runtime checks
keywords: windows 10, uwp, windows community toolkit, uwp community toolkit, uwp toolkit, plaform specific, platform specific analyzer, roslyn analyzer
dev_langs:
  - csharp
---

# Platform Specific Analyzer

The [writing version adaptive](https://docs.microsoft.com/windows/uwp/debug-test-perf/version-adaptive-code) code, the developers should ensure that code checks for presence of API before calling it.
The platform specific analyzer is a Roslyn Analyzer that can parse through code and suggest fixes where appropriate.

## Installation

The analyzer is available both as a nuget package and also as Visual Studio Extention

* References > Manage NuGet References > install [Microsoft.Toolkit.Uwp.PlatformSpecificAnalyzer](https://www.nuget.org/packages/Microsoft.Toolkit.Uwp.PlatformSpecificAnalyzer)


## Sample Output

The analyzer automatically kicks in when code is opened in Visual Studio.

![Code Analysis](../resources/images/CodeAnalysis.png)

![Code Analysis](../resources/images/CodeFixSuggestion.png)

## Requirements

| Device family | Universal, 10.0.15063.0 or higher   |
| ---------------------------------------------------------------- | ----------------------------------- |
| Namespace                                                        | Microsoft.Toolkit.Uwp.PlatformSpecificAnalyzer |
| NuGet package | [Microsoft.Toolkit.Uwp.UI.Animations](https://www.nuget.org/packages/Microsoft.Toolkit.Uwp.PlatformSpecificAnalyzer/) |

## API Source Code

- [Platform Specific Analyzer](https://github.com/Microsoft/UWPCommunityToolkit/tree/master/Microsoft.Toolkit.Uwp.PlatformSpecificAnalyzer)

## Related Topics

<!-- Optional -->

- [Platform Specific Differences Generator](https://docs.microsoft.com/dotnet/api/microsoft.toolkit.uwp.ui.platformspecificanalyzerdifferencesgen)