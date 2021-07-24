Host.CreateDefaultBuilder() do the following

Initializes a new instance of the HostBuilder class with pre-configured defaults.

The following defaults are applied to the returned HostBuilder:

• set the IHostEnvironment.ContentRootPath to the result of Directory.GetCurrentDirectory()

• load host IConfiguration from "DOTNET_" prefixed environment variables

• load app IConfiguration from 'appsettings.json' and 'appsettings.[IHostEnvironment.EnvironmentName].json'

• load app IConfiguration from User Secrets when IHostEnvironment.EnvironmentName is 'Development' using the entry assembly