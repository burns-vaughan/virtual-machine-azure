<p align="center">
<img src="https://i.ibb.co/9yNG8wG/1.png" alt="1" border="0">
</p>

<h1>Microsoft Azure - How to Create a Virtual Machine</h1>
This tutorial outlines how to create a virtual machine in Microsoft Azure. As well as, the minimum resources you should assign to it, such as the RAM and CPU. We will then log into it to test it<br />

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

Below, is a screenshot showing where to create the virtual machine in Azure. As well as, the first screen you should see:<br><br>

<img src="https://i.ibb.co/jZL6b6M/os-Ticket-prereqs1.jpg" alt="os-Ticket-prereqs1" border="0" />
<br><br>

<img src="https://i.ibb.co/HxMqFd1/2.jpg" alt="2" border="0">

<h3>2. Configure resource group, and network</h3>

After that it will ask you to fill out the key info. For convenience here's a short list of what to set everything to in order.
- <strong>Resource group</strong> - create new, name is something convenient
- <strong>Virtual machine name</strong> - name it something convenient
- <strong>Region</strong> - leave as default or change to your region. Not very important for creating the VM and can be edited later.
- <strong>Image (.iso image)</strong> - Windows 10
- <strong>Size</strong> - Standard_E2s_v3 - 2 vcpus, 16 GiB memory. Giving it 2 virtual CPUs and 16GB of RAM.
- <strong>Authentication type</strong> - change to password
- <strong>Username and password</strong> - Name is something convenient and ensure you note it down somewhere
- <strong>Licensing</strong> - confirm you have a license for Windows 10.

Here's a screenshot showing the final screen:<br><br>

<img src="https://i.ibb.co/d6nskmx/3.jpg" alt="3" border="0">

From there fill out the first screen completely using the info above, and hit review and create.


<h3>3. Log into remote machine</h3>
