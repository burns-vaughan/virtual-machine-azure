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

<img src="https://i.ibb.co/jZL6b6M/os-Ticket-prereqs1.jpg" alt="os-Ticket-prereqs1" border="0" />br>
<br><br>
Here's a screenshot showing the next screen, and the first field to fill out which is the resource group: <br>
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

Fill out the first screen completely using the info above, and hit review and create. There are additional tabs such as 'disk' and 'network'. But, these can all be left as default. It will create a default virtual network.

Here's a screenshot showing the final screen:<br><br>

<img src="https://i.ibb.co/d6nskmx/3.jpg" alt="3" border="0">

Hit 'review and create'. It will take a few minutes to create it for you. If you get any error messages you have likely accidentally left something out or filled out a field incorrectly. A common one, is accidentally not selecting that you have a Windows license. You simply need to tick the box and hit review and create a gain.

<h3>3. Log into remote machine</h3>
Your virtual machine is all set up. Now, let's log into it. The vast majority of people use Windows, so I will explain how to log into it using Windows. For Mac or Linux, do a quick Google search for what program to use.

Open Windows Remote Desktop by searching for it in your Windows start menu. Below, is a screenshots showing how to open it:<br><br>

<img src="https://i.ibb.co/jr0Vf4L/4.jpg" alt="4" border="0">

Next, you need to grab the public address for the virtual machine you created in the network settings in Azure. To access click on the virtual machine you created and it will show the basic info about. Below, is a screenshot showing where to find it: <br><br>

<img src="https://i.ibb.co/1sf7QQb/5-public-ip.jpg" alt="5-public-ip" border="0">

Input that into the Windows Remote Desktop, shown in the screenshot below:<br>
<img src="https://i.ibb.co/6RrbF33/remote-desktop-input-ip.jpg" alt="remote-desktop-input-ip" border="0">

Next, you need to click on 'more choices', shown in the screenshot below:<br>
<img src="https://i.ibb.co/xGTFcX3/6-change-username-remote-desktop.jpg" alt="6-change-username-remote-desktop" border="0">

Now, input the username and password for you that you set when you created it. And select connect. Below, is a screenshot showing how it should look:<br>

<img src="https://i.ibb.co/GTGVZnS/7-input-new-login-info.jpg" alt="7-input-new-login-info" border="0">
It will then log you into your virtual machine. It will a minute or so to completely log in. It will ask you about a few settings to set up Windows 10 for the first time. Use all the defaults or change them based on your personal preference.

That's it all done. It's important to note that you will want to delete all the resources created afterwards if you do not intend to use your VM. This is because it will charge you some credits from your free account. Or, charge on pay as you go based on your current subscription. The cost is very cheap - about 20 cents per hour, but it's not worth keeping it on your account if you don't intend to use it. 

That's it, congratulations on setting up your VM!
