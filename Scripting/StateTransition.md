---
title: State Machine - onTransition 
keywords: workflow, scripting, ontransition, statemachine

status: approved
created: 20171009
updated: 20171011
createdby: bytemaster-0xff
updatedby: klworkman
---
[Home](../Index.md) > [Scripting](Index.md)

# State Machine - onTransition

When a State Machine performs a transiton between States, a method will be called that you can customize.

```
function onTransition() {
    ...
}

- or -

function onTransition(value) {
    ...
}

- or -

function onTransition(latitude, longitude) {
    ...
}
```

The method can be called with an optional parameter.  The value that will be passed in will be added by the [Handle](StateMachineSendEvent.md) method that initiates 
the transition.  If the value is a geolocation, both the latitude and longitude will be provided.

You will also have access to the [Device Properties](WorkingWithAttributes.md), [Device Properties](WorkingWithProperties.md), [Property Bag](PropertyBag.md) and state machines and can invoke [Output Commands](https://github.com/LagoVista/docs/blob/master/Scripting/OutputCommandCreate.md). 
