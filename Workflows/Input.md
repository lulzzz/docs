---
title: Input
keywords: workflow, input

status: approved
created: 20171009
updated: 20171011
createdby: Kevin D. Wolf
updatedby: klworkman
---
[Home](../Index.md) > [Workflow](Index.md)

# Inputs

An Input is a value that comes from a [Device Message](../Messaging/Index.md) that has a specific [Type](../Messaging/TypeSystem/Index.md).      

When building your workflow, you can update your device data from data arriving from incoming messages.  After the
[Input Translator](../PipelineModules/InputTranslator.md) converts the raw message format into standard message format,
the fields on the standard message format are mapped to inputs within a [Route](../Routes/Route.md). 

In addition, you can provide a [Script](../Scripting/WorkflowInputOnSet.md) that will get executed when the input is set.

Finally within your scripts, you can [access the raw input values](../Scripting/WorkingWithWorkflowInputs.md).


### Mapping from Inputs

[To Attribute](./Mappings/InputToAttribute.md)  
[To Output Command](./Mappings/InputToOutputCommand.md)  
[To State Machine](./Mappings/InputToStateMachine.md)  

### Mapping from Inputs

None - an Input can only be a source for mappings
