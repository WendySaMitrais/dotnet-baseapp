# BaseApp.Core

This Class Lib project serves as the library that contains Core logics, interfaces and DTOs.

## Troubleshootings

* When I build the project, the build was failed and give me message: `"Package Microsoft.Net.Sdk.Compilers.Toolset is not downloaded but it is needed because your MSBuild and SDK versions are mismatched. Ensure version 9.0.200 of the package is available in your NuGet source feeds and then run NuGet package restore from Visual Studio or MSBuild."`
  <br> <u>Solution</u>: <br>
  Open Powershell terminal and ensure the current directory points to `BaseApp.Core`'s directory, then run ` dotnet restore /p:BuildWithNetFrameworkHostedCompiler=true` command. Confirm that the command finished successfully. Then, run `dotnet build` command. Confirm that the command also finished successfully.
* TBD