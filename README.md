
![BLOG_IMAGE_1](https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/github.png)
# Azure-SSL-Certificates 
This tutorial outlines how to create an Azure key vault and use it to store an SSL certificate 

## Environments and Technologies Used 

- Microsoft Azure key vault 

## High-Level Steps

- Create a key vault 
- Create a self-signed certificate 
- Import and build your self-signed certificate to your web application.
- Create and bind an app service managed certificate

<h2>Installation Steps</h2>

<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step1-project1.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create an Azure key vault.


<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step4-project1.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
</p>

Returned to the command line to use OpenSSL.


<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step5-project1.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
</p>
OpenSSL to generate a certificate called a self-signed certificate.

<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step7-project1.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
</p>
After creating a self-signed certificate, I imported my certificate into Azure key vault 

<p>
<img src="https://github.com/kleeloy/Azure-Cloud-Web-Application-/blob/main/Diagrams/step8-project1.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
</p>
Finding multiple security risks, I replaced my first certificate by using Azure's services to add a more secure certificate, an app service managed certificate, directly to my web application. 

