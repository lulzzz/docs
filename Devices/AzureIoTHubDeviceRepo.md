---
title: Azure IoT Hub Device Repository
keywords: device, devicerepo, azureiothub

status: approved
created: 20170922
updated: 20171011
createdby: bytemaster-0xff
updatedby: klworkman
---
[Home](../Index.md) > [Devices](Index.md)

# Azure IoT Hub Device Repository

If you are using Azure IoT Hub to connect your devices, you will need to use the Azure IoT Hub Device Repository.

To maintain consistent data, NuvIoT currently requires you to use the NuvIoT built-in Device Repository Editor to provision and update your devices.  
If you need afeature that is not available in our built-in Management Console, please [Contact Us](http://support.nuviot.com/contactus?source=auzreiothubrepo) so that we can work with you to meet your needs.

When you connect your NuvIoT repository to the Azure IoT Hub, you need to use a Shared Access Key that has registry read/write permissions.

### Required Fields

In addition to the [standard fields](../Topics/StandardFields.md) that are required, the following fields are required:

* **Resource Name** (required)    
The name of your Azure IoT Hub

* **Access Key Name** (required)  
The name of the Policy/Key that has "Registry write" permissions

* **Access Key** (required)     
The Shared Access Key for the policy/key that has "Registry Write" permissions as specified in the Access Key Name field.  This is a Base 64 encoded value.
