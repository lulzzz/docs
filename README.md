# NuvIoT Documentation Project

This Project is used to Maintain Documentation Used for building projects with IoT App Studio

### Documentation Workflow

The top of each Markdown file will include meta data about the help file, here is an
example of that data. 
```
---
title: Input Translator
description: Provides a description of an Output Translator, what it does and how to add one.
keywords: listeners, inputtranslator, pipelinemodule

status: inprocess
created: 20170927
updated: 20170927
createdby: bytemaster-0xff
updatedby: bytemaster-0xff
---
```

The meta data will start out with three dashes (---) which will always be the first three
characters of the file.  The meta data will then be terminated by three dashes as well (---).

Here are a description of the meta data fields  

**title** - Title of the document, this will be used in search results.  
**description** (optional) - A one sentance description of the content of the document.  
**keywords** - Any applicable keywords that might be helpful in searching the document
**status** - We will have a set of status that define the workflow of publshing documentation
1. **new** - Documentation headers and place holders are created, not content was added.
2. **inprocess** - Documentation is currently being created by developers or engineers
3. **readyforreview** - Developers think that the content is complete and ready for QA/Technical writing cleanup.
4. **readyforapproval** - QA/Technical writers have reviewed the content for grammer and made sure it follows a the style guide.
5. **issues** - Developers, QA/Technical writers have found an issue that needs to be resolved in the document.  The actual issue itself can either be added as a Github issue or added as free form at the end of the metadata.  Once the issue has been resolve the issues should be removed from the meta data.   
6. **approved** - A project architect has approved the content and edits and the documentation is ready for publishing.

For now to find documents in different status, just search the repository by status name, in the future tooling might be available.

**created** - The date stamp when the documentation was created, this will always be 8 characters and be in the format YYYYMMDD.  
**updated** - The date stamp when the documentation was last updated, this will always be 8 characters and be in the format YYYYMMDD.  
**createdby** - The github user id of the user that created the document
**updatedby** - The github user id of the user that last updated the document
  
