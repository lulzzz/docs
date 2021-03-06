---
title: Gloassary
keywords: help, glossary

status: inprocess
created: 20171116
updated: 20171116
createdby: bytemaster-0xff
updatedby: bytemaster-0xff
---
# Glossary

**Attributes**  
As part of processing messages from our device, you can define Attributes within your Device Workflows.  You can think of
Attributes as variables where you can store data that is saved with the device after the message is done processing.  You can
also write small JavaScript functions to perform actions when the attribute is set.

**Device**  
We define a device as anything that is external to our system that generates and receives messages to and from NuvIoT.

**Device Configuration**  
A device configuration is a defintion of how messaages that are received should be processed.  A device configuration also
define a set of Device Properties that define run time values that you can set for individual devices that you can use in
your workflows.   

**Device Message**  
A device message is a set of text or binary data that is sent to and from our devices.  You define the messages as part of building our IoT application and we support many different formats.

**Device Type**  
A device type is a specific model and part number that you can use to manage your devices.  A device type must have a device configuration.

**Device Workflow or Workflow**  
The Device Workflow Pipeline Module is where you can build functionality where you can take actions based on the data that is received in your messages.  You 
can store data for future use, make decisions based on the content of data, build up messasges that can be sent to other system as well as handle input 
commands to perform other actions on our devices.

**Host**  
A host is a compute resource that either hosts the entire runtime for your instance or manages the cluster of machines or vms that run the 
individual pipeline modules.  In most cases you won't have to work with hosts directly but will rather manage your instances and how they 
should be deployed.  In most cases hosts are simply compute resources that run the containers that run the NuvIoT runtime. 

**Input**  
An Input is the entry point from the Device Message into the Device Workflow.  Since your workflows are reusable across different IoT applications, we 
don't tightly couple the messages with how they are processed.  Using the Input Translator you map the Device Message Field to the Input on the Workflow,
once the Input is set it can be mapped to different components within the Device Workflow.

**Input Translator**  
The Input Translator is a Pipeline Module this is used to take Device Messages received from the Listener and parse the contents of those messages into 
Strongly Typed Named Value Pairs that can then be used to map to Inputs on a Device Workflow through a Route.

**Instance**  
An instance is an instance of a solution that is running on a host. After you build your app, you will deploy your instance to execute the runtime to process
incoming messages.  You can have many instances of the same solution.

**Input Commands**  
Input Comamnds are REST basd endpoints that are dynamically defined as part of your workflow.  Input Commands can be invoked on devices (including a payload)
that can perform actions within the workflow or send messages to the device. 

**Listener**  
The listener is Pipeline Module and is where message enter our system.  Listeners either listen on port or protocol such as REST, TCP, UDP or connect to
an external server and subscribe or handle messages.  Once the listener receives a message it hands it off to the Planner to identify how the message
should be processed. 

**Pipeline Module**  
A pipeline module is a defined set of functionality that knows how to act on and process a pipeline message execution messaage.  As messages are 
processed through NuvIoT they are handled be a set of modules that performs a task or action on them.  Each pipeline module listens on a queue, performs
it's actions and passes the message to the next pipeline module via it's queue.

**Output Command**  
The Output Command is a component of a Device Workflow.  As part of building up your workflow you can define Output Commands to contain fields that will
makeup messages that can be sent back to the device or an external system.  Once your Output Command has been constructed and sent it will be handed off
to the Output Translator that wil map the fields from the Output Command to the format of the outgoing message that your Transmitter will send.

**Output Translator**  
The Output Translator is a Pipeline Module that is used to take Output Commands that are constructed from the Device Workflow, build outgoing messages
and map the fields from the Output Command to the Outgoing Device Messages that will eventually be sent with the Transmitter pipeline module.

**Planner**  
The Planner is a Pipeline Module and is used identify the type of message that was received, once we have the message we find the device configuration assocaited with the device
and then identify the route for that message to build the route that should be followed to process it.

**Sentinel**  
The Sentinel Pipeline Modue is used to authenticate that the message received was actually sent from the device that claimed it sent it.  If the
sentinel module detects an unauthorized message, the message will not be processed.

**Solution**   
A solution is where you assemble all the components that make up your IoT application.  A solution consists of a set of Listeners that 
receive incoming messages, a Planner to identify messages and devices and Device Configuration that define how those messages should be proceessed.

**Stongly Typed Named Value Pairs**  
When messages arrive through a Listener, they can come in many different formats.  To create an environment where messages can be processed
in a consistent manner, the Input Translator uses the Device Message Defintions to extract data from those messages and turn them into objects that have three parts.
A name, that was identified in Device Message Field Definition, the Value that was extracted from the message and finally a type to define the data type of the field.

**Transmitter**  
The Transmitter is a Pipeline Module that is used to take outgoing messages constructed by the Output Translator from Output Commands and send them back to the device or a
third party system.

  
