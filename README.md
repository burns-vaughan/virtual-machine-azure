<p align="center">
<img src="https://i.ibb.co/9yNG8wG/1.png" alt="1" border="0">
</p>

<h1>Microsoft Azure - How to Create a Virtual Machine</h1>
This tutorial outlines how to create a virtual machine in Microsoft Azure. As well as, the minimum resources you should assign to it, such as the RAM and CPU.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10 or 11</b> (21H2)

<h2>High level Deployment and Configuration Steps</h2>

1. Initiate creating a virtual machine
2. Configure resource group, and network
3. Log into remote machine

<h3>1. Initiate creating a virtual machine</h3>
The first step is to initiate creating a virtual machine in Azure. To do that log in to your Azure portal. There are multiple ways to access it. In this example, we will get there by clicking it from your Azure portal homepage.<br><br>

<h3>2. Configure resource group, and network</h3>

After that it will ask you to fill out the key info. For convenience here's a short list of what to set everything to in order.
Resource group - create new, name is something convenient
Virtual machine name - name it something convenient
Region - leave as default or change to your region. Not very important for creating the VM and can be edited later.
Image - Windows 10
Size - Standard_E2s_v3 - 2 vcpus, 16 GiB memory. Giving it 2 virtual CPUs and 16GB of RAM.
Authentication type - change to password
Username and password: Name is something convenient and ensure you note it down somewhere
Licensing - confirm you have a license for Windows 10.

Here's a screenshot showing the final screen:<br><br>

<img src="https://i.ibb.co/d6nskmx/3.jpg" alt="3" border="0">

Some can be left as default, so if a setting is not listed above, then leave it as the default.

Below, is a screenshot showing the first setting to change which is the resource group. I almost always create a new resource group. Name is something convenient. For this example, I named I named the resource group: Resource-group-1. <br>

From there fill out the first screen completely using the info above, and hit review and create.

<img src="https://i.ibb.co/HxMqFd1/2.jpg" alt="2" border="0">

<h3>3. Log into remote machine</h3>
