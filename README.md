<h1>Active Directory - DFS Namespaces</h1>
<h2>Description</h2>
In this lab, we will be setting up DFS Namespaces on our Windows Server. DFS allows us to manage shared folders across multiple servers and devices easily. It gives the user a single path to view the folders and files located on different servers.

<h2>Installing DFS Namespaces</h2>

<img src="https://imgur.com/VdjwpWl.png" height="80%" width="80%"/>

In Server Manager, select Manage and Add Roles and Features.

<img src="https://imgur.com/IOPToKC.png" height="80%" width="80%"/>

Select Next until you get to Server Roles. Select DFS Namespaces, which is nested under File and Storage Services and File and iSCSI Services. Click Next until the Install option is available.



<h2>Setting Up DFS Namespaces</h2>

<img src="https://imgur.com/lLxQNCM.png" height="80%" width="80%"/>

Under Tools, select DFS Management.

<img src="https://imgur.com/PFzkI2c.png" height="80%" width="80%"/> 

Select New Namespace.</br>

<img src="https://imgur.com/Ge7xzsF.png" height="80%" width="80%"/>

Type your server name.</br>

<img src="https://imgur.com/B4sbpF3.png" height="80%" width="80%"/>

Give your Namespace a name. Under Edit Settings you can edit user permissions.

<img src="https://imgur.com/3xHD5qv.png" height="80%" width="80%"/>

Select Domain-based Namespace.

<img src="https://imgur.com/Wu1gmH5.png" height="80%" width="80%"/>

Select Create.


<h2>Joining Shares</h2>

<img src="https://imgur.com/HNGfHVz.png" height="80%" width="80%"/>

We will be joining 2 shares, Accounts and Thumb. Accounts is a folder on the server. Thumb is an external storage drive.

<img src="https://imgur.com/j0x4uxp.png" height="80%" width="80%"/>

Select the created namespace and create a New Folder. Name it Accounts. Add a Folder target. Click Browse to view all shared folders.

<img src="https://imgur.com/vC1juhP.png" height="80%" width="80%"/>


Click Accounts.

<img src="https://imgur.com/FAyRGzv.png" height="80%" width="80%"/>

Click OK.

<img src="https://imgur.com/F61oo3c.png" height="80%" width="80%"/>

Accounts and Thumb have been added. Use the same steps above to create Thumb.



<h2>Mapping DFS for User Access</h2>

<img src="https://imgur.com/HqHXshm.png" height="80%" width="80%"/>

Type the path in file explorer.

<img src="https://imgur.com/bBBAhqW.png" height="80%" width="80%"/>

<img src="https://imgur.com/ZUnNFUU.png" height="80%" width="80%"/>



Right click on Network and select Map Network Drive.

<img src="https://imgur.com/QArnPxy.png" height="80%" width="80%"/>

Type the folder path, select the Drive letter and make sure Reconnect at sign-in is selected. The computer will automatically reconnect to the share when the user signs in, even after shutting down their pc.

<img src="https://imgur.com/KBFGFRY.png" height="80%" width="80%"/>

Mapping the drive saves it under Network Locations.

