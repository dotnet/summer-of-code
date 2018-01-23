## Improve .NET and ASP.NET documentation

**Complexity:** Medium

The .NET and ASP.NET docs team is responsible for a vast set of articles, tutorials and API reference documentation for the following technologies:
* C#
* F#
* Visual Basic
* .NET Core
* .NET Framework
* .NET Standard
* ASP.NET Core
* ASP.NET

The main goal of this project is to create new interactive lessons for users to learn how to program in C# using our new .NET REPL (Read Evaluate Print Loop). These lessons will take the students through a series of steps and build code for a specific C# topic. First, the lessons are all web-based and then they move on to show the students how to build that code on their own machines. To see existing lessons, visit [aka.ms/csharp-quickstarts](https://aka.ms/csharp-quickstarts).

You could also pick and choose from our backlog, tasks that would appeal most to your skills and interests. It can be more heavily focused on content, code or both.

Deliverables:
* New C# interactive beginner lessons similar to the ones found at [aka.ms/csharp-quickstarts](https://aka.ms/csharp-quickstarts).
* (Optional) Create new samples (interactive or non-interactive) for the API reference documentation.
* (Optional) Create new articles.
* (Optional) Fix documentation bugs.
* (Optional) Enhance existing content.

**Mentors**: [Maira Wenzel](https://github.com/mairaw), [Bill Wagner](https://github.com/BillWagner), [Rick Anderson](https://github.com/Rick-Anderson)

## Implement Programmatic API for Documentation Repo

**Complexity:** Medium

`mdoc` is used to scan .NET and UWP assemblies and create a repository of EcmaXML which can be source controlled. This repository is then used as the source to publish documentation to end users (via web and otherwise). Many engineering teams write scripts that read this source in order to create statistics and analysis of their APIs, or even automatically document their library based on business heuristics. This task would build a programmatic interface to create, update, and query these repositories; all of these scenarios and others would benefit from the presence of this API. 

Deliverables:
An API that lets you create, read, and update an EcmaXML repository. Updates will use a batching system, so you can collect changes to a file and write all at once. Querying would be implemented with a custom IQueryable provider, so that you can easily search repositories with LINQ without running out of memory. Additionally, Unit tests will be required.

**Mentors:** Joel Martinez
