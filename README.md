
![BLOG_IMAGE_1](https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/github.png)
# Azure-SSL-Certificates 
This tutorial outlines how to build, host, and design a web application using Azure

## Environments and Technologies Used 

- Microsoft zure (web app)
- Domain name
- Container for the web app

## Operating Systems Used

- Windows Server 2022
- Windows 10 (21H2)

## High-Level Steps

- Create an Azure web app.
- Choose a domain.
- Deploy a container on the web app.
- Design your custom web application.

<h2>Installation Steps</h2>

<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step1-project1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step2-project1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/Creating%20web%20app-project1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

Begin by logging in to the Azure portal. Select "App Services" from the Azure search field at the top of the page. Selected "+ Create" to create my application, Under the "Basics" tab, made the following selections:
Name, Publish: Select "Code", Runtime Stack: Select "PHP 7.4.", Operating System: Select "Linux.", Region.


<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step4-project1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

Navigate to GoDaddy.com. Pick a website for your cyber-blog


<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step5-project1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step6-project1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Returned to the app where I created within Azure App Service. Select "Custom domains" from the left-hand menu, then click "Add custom domain." In the "Custom domain" text box, enter the new domain that I created on GoDaddy, and then click "Validate." After selecting "Validate," the page will confirm whether the hostname is available. Selected the hostname record type "A Record," and notice the TXT and A data under "Domain ownership," as shown in the following image:

<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step7-project1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Return to your GoDaddy.com products page and Below my existing DNS records, I selected "ADD" and added the custom domains:

<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step8-project1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
My new domain appeared under "Assigned Custom Domains," as the following image shows:

<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step9-project1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
For my web application, I used  a Docker container that has been added to Docker Hub:

```
cyberxsecurity/project1-apachewebserver
```

<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step10-project1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Next, I will use the Azure Cloud Shell to deploy this container to my web application. To open Azure Cloud Shell, click the shell logo in the tool bar at the top of the screen, as indicated by the red arrow in the following image:
Once clicked this icon, the Cloud Shell will be accessible at the bottom of my page.

       -  Select which shell to use (Bash or Powershell): Select "Bash."
       -  Create Storage: If a window appears, select "Create Storage."


<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step11-project1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
To configure my web app with this provided container, run the following: `az webapp config container set --name <name of your webapp> --resource-group <name of your resource group> --docker-custom-image-name <container-name> --enable-app-service-storage -t'. After pressing enter, this image appeared:


<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Applic
