---
title: Developer
keywords: development

status: readyforreview
created: 20171018
updated: 20171018
createdby: bytemaster-0xff
updatedby: bytemaster-0xff
---

# Developer Home Page

 #### *Configure More - Code Less* 

NuvIoT was architected from over 25 years of experience building custom software.  
Over those 25 years, we've seen many claims of "Build XYZ without a single line of code!". Most of those solutions aren't around today.

Our vision is based on *Configure More - Code Less*, not on false claims that you'll never have to write any custom code.  
A great deal of effort was expended to design a system that allows you to use our 
data driven architecture for as much as possible while providing a considerable number of integration points for both adding 
custom scripts via our IoT App Studio to building either custom containers to do processing or
end points that you provide to peform your custom logic.

Our IoT Application Architecture is based on a series of [Pipeline Modules](../PipelineModules/Index.md) that process messages via Pipeline Execution Messages.

#### The following Resources are Available as Custom Integration Points

* **Scripting** - A first and very powerful mechanism to provide your custom logic is the ability to add custom scripts to process your IoT data.  These scripts give you context senstive help as to your specific configurations and built in services via Intellisense.
* **REST API** - A REST API with well over 100 end points has been provided to configuration and control all aspects of your IoT Implementation.  In fact anything you can do through IoT App Studio, you can do through the API.
* **White Label Mobile Apps** - We provide a Xamarin SDK that will give you a great head start to building your custom mobile apps that leverage data produced from NuvIoT
* **Custom Public/Private End Points** - With this approach you can host an End Point on your infrastructure (either via Public IP or VPN) and pass it a Pipeline Execution Message for processing.  You'll have the best of both worlds, a robost fault redundent high performance IoT data capture, storage and conditioning engine and very custom and potentially proprietary services that don't make sense to host in NuvIoT.
* **Containers** - You can build a custom Docker Container that handles Pipeline Execution Messessage, host it on our servers and register it to participate in the Pipeline Execution Engine.