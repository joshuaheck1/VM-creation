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
- After creating an account with Microsoft Azure and loging in, you will end up at the Quickstart Center screen. Welcome to Azure!
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
<img width="750" alt="Screenshot 2025-01-07 at 11 00 54 PM" src="https://github.com/user-attachments/assets/be842a97-4b65-471b-85ce-b40fefdd8f25" />
</p>
<p>
For size, anything with at least 2 vCPU's and 8 GiB of memory will be sufficient. Next, enter in a username and password that you would like to use for the Windows VM.
</p>
<p> Finally, scroll down to the bottom of the page and check the box for licensing, click Review+Create and Create once the review is passed. The Windows VM will now take a few minutes to deploy. </p>
<br />

<h3>Step 2: Create the Linux VM in Azure </h3>
<p>
<img width="750" alt="Screenshot 2025-01-07 at 11 02 26 PM" src="https://github.com/user-attachments/assets/41a917cd-1b2e-4489-8bcb-429dd1780120" />
</p>
<p>
Going back to the Virtual Machines home page, create another virtual machine. Be sure that it is under the same Resource Group as the Windows VM. 
</p>
<p> Name this VM to indicate that it is the Linux VM, pick the same region as the Windows VM, and leave the zone selection as is unless prompted by Azure. </p>
<br />

<p>
<img width="750" alt="Screenshot 2025-01-07 at 11 04 11 PM" src="https://github.com/user-attachments/assets/186ec692-9fc4-418c-a13c-ac4735f504b5" />
</p>
<p>
For the image, please select Ubuntu Server 22.04. 2 vCPU's and 8Gib memory will suffice. </p>
<br />


<p>
<img width="750" alt="Screenshot 2025-01-07 at 11 05 01 PM" src="https://github.com/user-attachments/assets/bf019ab9-ea77-4d05-b4a6-814a92e0b083" />
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
