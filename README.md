![cloud2](https://github.com/user-attachments/assets/bfb02120-7283-49b3-850a-5f6497fbd5e9)
<p align="center">
 
</p>

<h1>Creating a Windows and Linux Virtual Machine in the Cloud (Microsoft Azure)</h1>
In this walkthrough, we will create a Windows and Linux virtual machine (VM) in Azure. This skill set will be vital and a key component to all of the IT projects listed. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)

<h2>Operating Systems Used </h2>

- MacOS 
- Windows 10 Pro (21H2)
- Ubuntu Server 22.04

<h2>List of Prerequisites</h2>

- <a href="https://azure.microsoft.com/en-us/pricing/purchase-options/azure-account/search?ef_id=_k_Cj0KCQjwzYLABhD4ARIsALySuCTvMpKHbOeSo9lv81A8vCg1XGDNwpOIuOsD2o8pmLnyl7dVku-Yn3IaApK-EALw_wcB_k_&OCID=AIDcmmfq865whp_SEM__k_Cj0KCQjwzYLABhD4ARIsALySuCTvMpKHbOeSo9lv81A8vCg1XGDNwpOIuOsD2o8pmLnyl7dVku-Yn3IaApK-EALw_wcB_k_&gad_source=1&gbraid=0AAAAADcJh_uVoYZIZMJRJFQ3v8k-BGmp2&gclid=Cj0KCQjwzYLABhD4ARIsALySuCTvMpKHbOeSo9lv81A8vCg1XGDNwpOIuOsD2o8pmLnyl7dVku-Yn3IaApK-EALw_wcB)">Microsoft Azure account</a> 

<h2>High-Level Steps</h2>

- Step 1: Create a Resource Group in Azure
- Step 2: Create the Windows VM in Azure
- Step 3: Create the Linux VM in Azure

<h2>Walkthrough Demonstration</h2>

<h3> Step 1: Create a Resource Group in Azure </h3>

<p>
<img width="750" alt="CVM RG1" src="https://github.com/user-attachments/assets/1c6e64ad-18da-497c-8ccc-3fe556fd6325" />
</p>
<p>
- After creating an account with Microsoft Azure and getting logged in, you will end up at the Quickstart Center screen. Welcome to Azure!
</p>
<br />

<p>
<img width="750" alt="CVM RG2" src="https://github.com/user-attachments/assets/225c4871-81f4-4c60-8cd1-f60c93de7d8c" />
</p>
<p>
- Locate the Search Bar at the top of your screen. We will use this to find the Resourse Groups. Notice the options that populate as you type "resource" into the search bar. Select Resource Groups.
</p>

<br />

<p>
<img width="750" alt="CVM RG3" src="https://github.com/user-attachments/assets/72a12b56-b80c-4cd8-85ea-20661e028bd0" />
</p>
<p> - Oops! The resource groups seem to be missing... Have no fear, IT is here! 😎 Click the + Create button and let's get this party started!</p>
<br />
<br />

<p>
<img width="750" alt="CVM RG4" src="https://github.com/user-attachments/assets/f1b182f0-e9db-475e-9036-6241d4c9366e" />
</p>
<p>
- The Subscription box should reflect whatever you chose when setting up your Azure account. If you do not see that, click the drop down arrow to find it. Now, name your Resource Group (RG). This RG is where our VMs will be stored in the Cloud. Next, choose the Region. *Pro Tip: Select (US) East US 2 for ALL Region options. Making sure the Region matches for eveything we create will save you from future headaches.* Now click next at the bottom of the screen.
</p>
<br />

<p>
<img width="750" alt="CVM RG5" src="https://github.com/user-attachments/assets/4d913c40-61ef-4e03-8488-d6ab4bb06540" />
</p>
<p>
- Review the Resource Group information and click Create. Make note of the name and region you used for future reference. 
</p>
<br />

<p>
<img width="750" alt="CVM RG6" src="https://github.com/user-attachments/assets/541f3928-a25c-473c-9b4e-e0ca9805304b" />
</p>
<p>
- After clicking Create you will be directed back to the RG section. You have successfully created your Resource Group in the Cloud. Now let's get to the good part and the real reason we're all here. To create some VMs! </p>
<br />

<h3> Step 2: Create a Windows VM in Azure </h3><p>
<img width="750" alt="CVM 1" src="https://github.com/user-attachments/assets/b801376c-5ef5-4c92-bfc1-75d2b3112549" />
</p>
<p>
  Deselect SSH public key and select password instead. Enter in a username and password for the Linux VM. Preferably the same one as the Windows VM for ease of memory.
</p>
<br />


<p>
<img width="750" alt="Screenshot 2025-01-07 at 11 07 44 PM" src="https://github.com/user-attachments/assets/c6017b09-d820-481a-88b0-26dd70d4badb" />
</p>
Scroll to the top and select the Networking tab. Make sure that this VM is in the same Virtual Network as the Windows VM. There may have been a Virtual Network that was created with the Windows VM and this will be one of the options for the Linux VM. In this step, be sure to select the same Virtual Network that the Windows VM is on. In this case, the Windows VM-net is the only option so it will be the same network.
</p>
<p> Finally, click Review+Create and create once the review has passed. It will take a few minutes for the Linux VM to deploy.</p>
<br />

<p>
<img width="750" alt="Screenshot 2025-01-07 at 11 28 44 PM" src="https://github.com/user-attachments/assets/b1ad41b7-709a-468e-bc40-0f9035fc14ee" />
</p>
<p>
  Once both VMs are deployed, they should appear in the Virtual Machines homepage. To confirm that they are on the same Virtual Network, click on each Virtual Machine and you will be brought to their configurations. From there you can confirm their Virtual Networks are the same.
</p>
<br />
