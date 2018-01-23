## Define and author new templates
**Complexity:** Low
Dotnet/templating templates provide the ability to quickly generate customized "boilerplate" code. Templates lay the foundation for performing specific common programming tasks, allowing programmers to quickly get started on the functional aspects of their applications by providing code to deal with standard use cases on top of existing generic API's. For template authoring, this could be simply writing common-use high level wrappers around an existing library which only implements low level functionality, or as complex as creating new functionalty from scratch. Some possible template ideas include: high-level API's to interact with map services, search engines, or social media platforms; students are also encouraged to propose templates based on their areas of interest.

**Deliverables:**
 * Work with the mentors to define specific, common programming tasks that could be reasonably handled via templates. 
 * Implement the chosen tasks in a general-purpose manner.
 * Package the code into templates, setting up appropriate user customizations.

**Mentors:** Sean Peters, Mike Lorbetske


## Authoring tools for dotnet/templating
**Complexity:** Medium
There is currently very little feedback to template authors regarding what occurs internally during template processing. This makes it difficult for template authors to troubleshoot problems when creating or updating templates. Optionally providing details of how a template gets processed will make for a much easier template author debugging experience.

**Deliverables:**
 * Implement a framework for reporting about template processing.
 * Identify "interesting" aspects of template processing, and hook those scenarios into the reporting framework.
 * (Optional): Implement a UI to display & navigate the processing report data.

**Mentors:** Sean Peters, Mike Lorbetske


## Template primary output configuration version 2
**Complexity:** Medium
Template authors may define ceration template files as "primary outputs". This information may be referenced by author defined template post actions which allow template authors to specify steps to occur after template invocation finishes, for example opening a template-related file in a browser or editor. Currently the post-action configuration references the primary outputs by a numeric index, but the indexes of the primary outputs are not constant since each defined primary output may be conditionally included or excluded; this makes it difficult & unintuitive to refer to the outputs in post action configuration. A better design for primary output configuration would allow referencing the outputs by author defined names as opposed to positional indexes, making the post action configuration must more intuitive. More details available here: https://github.com/dotnet/templating/issues/1258

**Deliverables:**
 * Implement a new template configuration reader which can read the new primary output configuration format.
 * Implement related changes to the classes that store & proces the primary output information.
 * For the above deliverables, retain backwards compatibility with the existing configuration format, so that existing templates continue working appropriately.

**Mentors:** Sean Peters, Mike Lorbetske


## Implement output variables
**Complexity:** Medium
Template engine hosts currently receive very little information from the template engine regarding template instantiation. Authors would like to define symbols in templates, and have the template creation process report on whether the symbol was emitted, and if so, in what file(s) and at what position in those file(s). 
Motivating issue: https://github.com/dotnet/templating/issues/1249
Existing preliminary work: https://github.com/dotnet/templating/pull/1385/files

**Deliverables:**
 * Implement a way for template authors to define symbols to be reported on.
 * Implement an operation to identify these symbols and their locations in output template files.
 * Implement appropriate reporting in the output payload for template engine hosts to consume.

**Mentors:** Sean Peters, Mike Lorbetske


## Improvements to template and component installation
**Complexity:** Difficult
Installation of templates and components currently encounters some difficulty in reporting on exactly what was installed, and also in identifying some unsupported scenarios which sometimes result in corrupted configuration. Improving the install experience will be of great benefit to tempalte authors, providing feedback on template packaging problems which could otherwise go unnoticed in certain cases.

**Deliverables:**
 * Work with the mentors to identify existing problems in the installation process.
 * Implement fixes and/or error reporting as appropriate for each scenario.
 * Implement better identification of, and reporting on the templates and components installed with each command.

**Mentors:** Sean Peters, Mike Lorbetske
