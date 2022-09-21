# Test project with .NET MAUI

![maui](src/Maui.VSCode/Resources/Images/dotnet_bot.svg)

This is a test project about debugging .NET MAUI on linux with Visual Studio Code.

## Observations

Althoug debugging cs files works, hot reload of xaml or any other file does not.

## Versions

Everything was tested using [archlinux btw](https://archlinux.org/).

- Visual Studio Code Insiders (1.72.0-insider)
  - [visual-studio-code-insiders-bin (AUR)](https://aur.archlinux.org/packages/visual-studio-code-insiders-bin)
- Dotnet SDK, Dotnet Runtimes and Mono (7.0.0 Release Candidate 1)
  - [mono-msbuild](https://archlinux.org/packages/community/x86_64/mono-msbuild/)
  - [mono-msbuild-sdkresolver](https://archlinux.org/packages/community/x86_64/mono-msbuild-sdkresolver/)
  - [dotnet-runtime-preview-bin (AUR)](https://aur.archlinux.org/packages/dotnet-runtime-preview-bin)
  - [dotnet-sdk-preview-bin (AUR)](https://aur.archlinux.org/packages/dotnet-sdk-preview-bin)
  - [dotnet-targeting-pack-preview-bin (AUR)](https://aur.archlinux.org/packages/dotnet-targeting-pack-preview-bin)
- VS Code C# Extension (1.25.1 beta 1)*
  - [Marketplace](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp)
  - [Github Release v1.25.1-beta1](https://github.com/OmniSharp/omnisharp-vscode/releases/tag/v1.25.1-beta1)

\*Observation: That version of the extension is not currently available on the marketplace, I downloaded it from the link to the github repo, but the latest version is only needed for code completion and highlighting of net7.0 code, so it is not really that important.

## References

Most of the `launch.json` and `tasks.json` configurations was taken from the following sources:

- [.NET MAUI – Develop with Visual Studio Code](https://egvijayanand.in/2021/04/04/net-maui-project-debug-with-vs-code/)
