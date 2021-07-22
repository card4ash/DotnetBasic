Create console Application
```dotnet new console -n BasicConsole```
Add below nuget

        dotnet add package Microsoft.Extensions.Hosting
        dotnet add package Serilog.Extensions.Hosting
        dotnet add package Serilog.Settings.Configuration
        dotnet add package Serilog.Sinks.Console
        dotnet add package Serilog.Sinks.File


Add below item group in csproj file

        <ItemGroup>
            <None Update="appsettings.json">
                <CopyToOutputDirectory>Always</CopyToOutputDirectory>
            </None>
        </ItemGroup>