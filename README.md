Serilog.Sinks.LINQPad
=====================

Serilog sink to publish colored output to the LINQPad Results panel. At present, most of the code has been shamelessly ripped from LiterateConsoleSink, with modifications to allow LINQPad to display colored results.

**Important:** This NuGet package is only useful (and usable) when using Serilog within LINQPad scripts.

```
PM> Install-Package Serilog.Sinks.LINQPad
```

Version 2.0
-----------
```csharp
Log.Logger = new LoggerConfiguration()
    .WriteTo.LINQPad()
    .CreateLogger();
```
