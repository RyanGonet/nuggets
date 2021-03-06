# Nuggets

This is where I record the tips, tricks and tools (free unless indicated otherwise :moneybag:) I've accumulated over the years.

I'm also shamelessly promoting some of my projects that nobody else is using (indicated with :trollface:)

## Tips and tricks

- :trollface: [Cake build][cake-build] - demonstrate a basic build of a `.NET Core` `NuGet` package using [Cake][cake]
- [Cake Intellisense](docs/cake-intellisense/README.md) - Intellisense for `Cake` in `Visual Studio Code`
- [Git][git-tutorial] - getting started with `Git` on `Windows`
- [Markdown][markdown-tutorial] - writing nice `Markdown`
- [ngrok][ngrok-tutorial] - expose a local server behind a `NAT` or firewall to the internet
- :trollface: [Serilog ASP.NET Core quick start](docs/serilog-aspnet-core/README.md) - configure `Serilog` in `ASP.NET Core` like a boss
- [PowerShell][powershell-tutorial] - pretend you know `PowerShell`
- [Splunk](docs/splunk/README.md) - run `Splunk` locally
- [SSH key pair](docs/ssh-key-pair/README.md) - generate / import a `SSH` key pair
- [TLS certificate](docs/tls/README.md) - generate a `TLS` server certificate on `Windows` and `macOS`
- [Visual Studio Code][vs-code-tutorial] - `Visual Studio Code` configuration and extensions
- [WinDbg][windbg-tutorial] - a brief guide (i.e. you are on your own)
- [WireMock][wiremock-tutorial] - mock `HTTP` server

## Practices

- `.NET`
  - [Coding convention](docs/dotnet/coding-convention/README.md) - easily enforceable `.NET` coding convention
  - [Layout](docs/dotnet/layout/README.md) - layout of a `.NET Core` project
- [Code review](docs/code-review/README.md) - guidelines for valuable code reviews
- [Documentation](docs/documentation/README.md) - help your future self
- [Logging](docs/logging/README.md) - an insider guide
- [Security](docs/security/README.md) - it doesn't matter until it does
- [The way we work](docs/the-way-we-work/README.md) - agree as a team on the importance of each task

## ASP.NET Core and Angular cookbook

- [Mitigate CSRF](docs/aspnet-core/csrf/README.md)
- [SPA routing](docs/aspnet-core/spa-routing/README.md)

## Instant nuggets

### Clear HSTS in Chrome

Navigate to `chrome://net-internals/#hsts`

### Query Azure Diagnostics Table

Query the `PartitionKey` of the `WadLogsTable`:

```csharp
$"0{DateTime.UtcNow.AddMinutes(-5).Ticks}".Dump();
```

## Software for developers on Windows

- :trollface: [Azure DevOps Linux build agent][azure-dev-ops-linux-agent] - provision a `Linux` `Docker` `Azure DevOps` build agent with the `AWS CLI` capability
  - Becoming less relevant since `Azure DevOps` offers [Linux hosted agents][linux-hosted-agents] and `Amazon` released [AWS Tools for Microsoft Visual Studio Team Services][aws-tools]
- [Azure Storage Explorer][azure-storage-explorer] - Manage `Azure Storage Accounts` (`Windows`, `macOS` and `Linux`)
- :trollface: [Beanstalk Seeder][beanstalk-seeder] - Emulates the `SQS` Daemon surrounding an `Elastic Beanstalk Worker Tier` (`Windows`, `macOS` and `Linux`)
- [Cmder][cmder] - Portable console emulator for Windows (`Windows`)
- [Docker for Windows][docker-windows] - Containerization platform (`Windows`, `macOS` and `Linux`)
  - Requires `Microsoft Windows 10 Professional or Enterprise 64-bit` and `Hyper-V`
  - For unsupported `OS` you can use [Docker Toolbox][docker-toolbox] instead
- [dotPeek][dot-peek] - Decompiler (Windows)
  - [Navigate to compiled source][dot-peek-navigate-compiled] when used with `ReSharper`
  - [Symbol server][dot-peek-symbol-server]
- [Fiddler][fiddler] - `HTTP` debugging proxy server (`Windows`)
  - Requires an **email address**
  - :moneybag: **Buy** the book [Debugging with Fiddler, Second Edition][debugging-with-fiddler] by Eric Lawrence (the creator of `Fiddler`)
- [Git][git] - Distributed version control system (`Windows`, `macOS` and `Linux`)
  - [Git Credential Manager for Windows][git-credential-manager]
  - I wrote a `Git` [tutorial][git-tutorial]
- [GraphiQL][graphi-ql] - A graphical interactive in-browser `GraphQL` `IDE` (`Windows`, `macOS` and `Linux`)
- [LINQPad][linq-pad] - Instantly test any `C#`/`F#`/`VB` snippet or program (`Windows`)
  - :moneybag: I highly recommend the **paid** [Developer Version][linq-pad-developer] which adds `NuGet` integration
  - `LINQPad` is maintained by Joseph Albahari an independent software developer
- [MailHog][mail-hog] - email testing tool for developers (`Windows`, `macOS` and `Linux`)
- [Microsoft Message Analyzer][microsoft-message-analyzer] - Capture, display, and analyze protocol messaging traffic (`Windows`)
  - [Operating Guide][microsoft-message-analyzer-operating-guide]
  - I covered Microsoft Message Analyzer in a [blog post][blog-netsh]
- [MSBuildStructuredLog][ms-build-structured-log] - A logger for `MSBuild` that records a structured representation of executed targets, tasks, property and item values (`Windows`)
- [ngrok][ngrok] - Expose a local server behind a `NAT` or firewall to the internet (`Windows`, `macOS` and `Linux`)
  - I wrote a [tutorial][ngrok-tutorial] for `ngrok`
- [NuGet Package Explorer][nuget-package-explorer] - Create, update and deploy `Nuget` packages with a `GUI` (`Windows`)
- [Log Parser][logparser] - `CLI` mainly used to query `IIS` logs (`Windows`)
- [Open Broadcaster Software][open-broadcaster-software] - Free and open source software for video recording and live streaming (`Windows`, `macOS` and `Linux`)
- [P4Merge][p4-merge] - Merge tool and diff tool (`Windows`, `macOS` and `Linux`)
  - I'm using it as a `merge.tool` and `diff.tool` in `Git` and wrote a [tutorial][p4-merge-tutorial] on how to configure it
- [Paint.NET][paint-dotnet] - image and photo editing (`Windows`)
  - :moneybag: Buy it on the [Windows Store][paint-dotnet-store] to support `Paint.NET`
- [PerfView][perfview] - CPU and memory performance-analysis tool (`Windows`)
- [Postman][postman] - A graphical `HTTP` client (`Windows`, `macOS` and `Linux`)
- :moneybag: [ReSharper Ultimate][resharper-ultimate] - **Paid** extension for `Visual Studio`. Find and fix errors and code smells; navigate and refactor; run unit tests (`Windows`)
  - Includes:
    - [dotTrace][dot-trace] - performance profiling
    - [dotMemory][dot-memory] - memory profiling
- :moneybag: [Rider][rider] - **Paid** cross-platform `.NET` `IDE` (`Windows`, `macOS` and `Linux`)
  - Replaced `Visual Studio` as my `IDE` of choice
- [ScreenToGif][screen-to-gif] - Quick and small screen recorder (`Windows`)
  - This is what I use on my [blog][blog]
- [Service Bus Explorer][service-bus-explorer] - Connect to a Service Bus namespace and administer messaging entities (`Windows`)
- [Sysinternals][sysinternals] - Manage, troubleshoot and diagnose your `Windows` systems and applications (`Windows`)
  - Most commonly used utilities:
    - [Autoruns][autoruns] - Shows what programs are configured to startup automatically when your system boots and you login
    - [ProcDump][proc-dump] - Process dump utility
    - [Process Explorer][process-explorer] - List currently active processes
    - [Process Monitor][procmon] - Shows real-time file system, registry and process/thread activity
- [Visual Studio Code][visual-studio-code] - Editor (`Windows`, `macOS` and `Linux`)
  - My editor of choice to edit markdown, `csproj`, `Cake build`... files
  - Read my [guide][vs-code-tutorial]
- [WinDbg][windbg] - The `Windows` Debugger (`Windows`)
  - For the rare occasions when you need to go thermonuclear
  - Also available in preview in the [store][windbg-store]
  - I wrote a *succint* [tutorial][windbg-tutorial] for `WinDbg`
- [WinDirStat][win-dir-stat] - Disk usage statistics viewer (`Windows`)
- [Windows Magnifier][windows-magnifier] - Magnifier makes part or all of your screen bigger so you can see words and images better (`Windows`)
- [WireMock][wiremock] - Mock `HTTP` server (`Windows`, `macOS` and `Linux`)
  - I wrote a [tutorial][wiremock-tutorial] for `WireMock`
- [Windows Subsystem for Linux][wsl] - Lets developers run `Linux` environments - including most command-line tools, utilities, and applications - directly on `Windows`, unmodified, without the overhead of a virtual machine (`Windows`)
- :trollface: [xUnit to JUnit][xunit-to-junit] - This `Extensible Stylesheet Language Transformations` can transform a `xUnit.net v2 XML` test results file into a `JUnit` test results file (`Windows`, `macOS` and `Linux`)

## .NET libraries

Yes I know they're all mine. I might add some real ones at some point.

- :trollface: [Simple Routing][simple-routing] - Allows to route a `SQS` message to a specific endpoint on the `Elastic Beanstalk Worker`
  - I wrote a blog [post][post-simple-routing] about `Simple Routing`
- :trollface: [Unsupported Types][unsupported-notes] - `Azure Table storage` supports a limited set of data types (namely `byte[]`, `bool`, `DateTime`, `double`, `Guid`, `int`, `long` and `string`). `Unsupported Types` allows to store unsupported data types

[linux-hosted-agents]: https://github.com/actions/virtual-environments/blob/master/images/linux/Ubuntu1804-README.md
[aws-tools]: https://marketplace.visualstudio.com/items?itemName=AmazonWebServices.aws-vsts-tools
[cake-build]: https://github.com/gabrielweyer/cake-build
[cake]: https://cakebuild.net/
[ngrok-tutorial]: docs/ngrok/README.md
[azure-dev-ops-linux-agent]: https://github.com/gabrielweyer/vsts-linux-build-agent
[wiremock-tutorial]: docs/wiremock/README.md
[azure-storage-explorer]: https://azure.microsoft.com/en-au/features/storage-explorer/
[cmder]: http://cmder.net/
[docker-windows]: https://store.docker.com/editions/community/docker-ce-desktop-windows
[docker-toolbox]: https://docs.docker.com/toolbox/overview/
[dot-peek]: https://www.jetbrains.com/decompiler/
[fiddler]: https://www.telerik.com/fiddler
[debugging-with-fiddler]: https://gumroad.com/l/dwf2/
[dot-peek-symbol-server]: https://www.jetbrains.com/help/decompiler/Using_product_as_a_Symbol_Server.html
[dot-peek-navigate-compiled]: https://www.jetbrains.com/help/decompiler/Navigation_and_Search__Navigating_to_External_Sources.html
[git]: https://git-scm.com/downloads
[git-credential-manager]: https://github.com/Microsoft/Git-Credential-Manager-for-Windows
[graphi-ql]: https://github.com/graphql/graphiql
[linq-pad]: https://www.linqpad.net/
[linq-pad-developer]: https://www.linqpad.net/Purchase.aspx
[nuget-package-explorer]: https://github.com/NuGetPackageExplorer/NuGetPackageExplorer
[ngrok]: https://ngrok.com/
[p4-merge]: https://www.perforce.com/products/helix-core-apps/merge-diff-tool-p4merge
[postman]: https://www.getpostman.com/
[resharper-ultimate]: https://www.jetbrains.com/dotnet/
[dot-trace]: https://www.jetbrains.com/help/profiler/Introduction.html
[dot-memory]: https://www.jetbrains.com/help/dotmemory/Introduction.html
[rider]: https://www.jetbrains.com/rider/
[screen-to-gif]: http://www.screentogif.com/
[blog]: https://gabrielweyer.net/
[sysinternals]: https://docs.microsoft.com/en-us/sysinternals/
[autoruns]: https://docs.microsoft.com/en-us/sysinternals/downloads/autoruns
[procmon]: https://docs.microsoft.com/en-us/sysinternals/downloads/procmon
[process-explorer]: https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer
[proc-dump]: https://docs.microsoft.com/en-us/sysinternals/downloads/procdump
[visual-studio-code]: https://code.visualstudio.com/
[markdownlint]: https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint
[editor-config]: https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig
[windbg]: https://developer.microsoft.com/en-us/windows/hardware/download-windbg
[windbg-store]: https://www.microsoft.com/en-au/store/p/windbg-preview/9pgjgd53tn86
[win-dir-stat]: https://windirstat.net/
[wiremock]: http://wiremock.org/
[microsoft-message-analyzer]: https://www.microsoft.com/en-au/download/details.aspx?id=44226
[microsoft-message-analyzer-operating-guide]: https://technet.microsoft.com/en-us/library/jj649776.aspx
[blog-netsh]: https://gabrielweyer.net/2016/07/16/capture-network-packets-with-netsh/
[wsl]: https://docs.microsoft.com/en-us/windows/wsl/install-win10
[git-tutorial]: docs/git/README.md
[ms-build-structured-log]: https://github.com/KirillOsenkov/MSBuildStructuredLog
[beanstalk-seeder]: https://github.com/gabrielweyer/beanstalk-seeder
[simple-routing]: https://github.com/gabrielweyer/simple-routing
[xunit-to-junit]: https://github.com/gabrielweyer/xunit-to-junit
[unsupported-notes]: https://github.com/gabrielweyer/unsupported-types
[post-simple-routing]: https://gabrielweyer.net/2018/01/28/simple-routing-elastic-beanstalk-worker/
[p4-merge-tutorial]: https://github.com/gabrielweyer/nuggets/tree/master/git#difftool-and-mergetool
[windbg-tutorial]: docs/windbg/README.md
[vs-code-tutorial]: docs/vs-code/README.md
[service-bus-explorer]: https://github.com/paolosalvatori/ServiceBusExplorer
[windows-magnifier]: https://support.microsoft.com/en-au/help/11542/windows-use-magnifier
[open-broadcaster-software]: https://obsproject.com/
[perfview]: https://github.com/Microsoft/perfview
[logparser]: https://www.microsoft.com/en-us/download/details.aspx?id=24659
[paint-dotnet]: https://www.getpaint.net/
[paint-dotnet-store]: https://www.microsoft.com/store/apps/9NBHCS1LX4R0?ocid=badge
[markdown-tutorial]: docs/markdown/README.md
[mail-hog]: https://github.com/mailhog/MailHog
[powershell-tutorial]: docs/powershell/README.md
