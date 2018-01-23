## ASP.NET Core Analyzers
**Complexity:** Medium

[ASP.NET Core](https://github.com/aspnet/home) is a cross-platform, high-performance, open-source framework for building modern, cloud-based, we apps using .NET.

[Roslyn Analyzers](https://github.com/dotnet/roslyn-analyzers) provide design-time diagnostics, code fixes, and refactorings to developers based on a semantic understanding of the code. This project would build a set of analyzers for ASP.NET Core application development.

Deliverables:
 * MVC analyzer (https://github.com/aspnet/specs/issues/110)
   * Check for actions or page handlers that don't return IActionResult
   * Check for async actions or page handlers that return void instead of Task
 * Logging analyzer (https://github.com/aspnet/Logging/issues/712)
 * Middleware ordering analyzer

**Mentors**: [Daniel Roth](https://github.com/danroth27/), [Pranav Krishnamoorthy](https://github.com/pranavkm)

## Complete WebHooks Port
**Complexity:** Medium

The [ASP.NET WebHooks](https://github.com/aspnet/WebHooks) system allows for producing and consuming web hooks in .NET. A port to .NET Core has been started, but is not complete. This project would include completing the port to .NET core and creating updated integrations with webhook consumers and providers.

Deliverables:
 * Port additional WebHook receivers from ASP.NET WebHooks to ASP.NET Core WebHooks
 * Port sender-side WebHook functionality from ASP.NET WebHooks to ASP.NET Core WebHooks
 * Port ASP.NET Web Hooks samples to ASP.NET Core WebHooks

**Mentors**: [Daniel Roth](https://github.com/danroth27/), [Doug Bunting](https://github.com/dougbu)

## Blazor
**Complexity:** Medium

[Blazor](https://github.com/aspnet/blazor) is a new experimental framework for building browser-based web applications with .NET and [WebAssembly](http://webassembly.org).

Deliverables:
 * Build sample Blazor applications and provide feedback on the framework
 * Analysis and optimization of .NET runtime assemblies to determine optimal trimming of unneeded code
 * Tooling for generating strongly typed C# wrappers for JavaScript libraries based on TypeScript definitions

**Mentors**: [Daniel Roth](https://github.com/danroth27/), [Steven Sanderson](https://github.com/SteveSandersonMS)
