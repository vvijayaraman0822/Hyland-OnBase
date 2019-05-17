# Hyland OnBase 
## Author - Vasudev Vijayaraman 
This document is to simply assist users with the basic knowledge of HYLAND OnBase. I by no means claim to be an expert. I like exploring interesting software's that are in existence and this is one among them. This document will be updated as and when needed. 

### What is Hyland OnBase?
It is a enterprise content management and process management software suite developed by HYLAND to manage your content, services, processes and cases. It is currently used in the healthcare, financial, insurance, government, higher education and manufacturing industries. 

### What makes it unique?
- One Platform - It is based on a single platform for building content-enabled applications. 
- Low code configuration - It reduces developer time with very limited code which is easily manageable. 
- Anywhere, any way - It could be deployed On-Premises and in the Cloud. Supports mobile devices and integrates exisiting applications.

### What are its statistics?
- Customer retention rate - 96% 
- Customer driver innovation - 85%
- Experience - 25+ years

## ONBASE SPECIFIC KNOWLEDGE

### What Enterprise applications are supported by OnBase?
Oracle E-Business Suite, SAP, Workday, PeopleSoft, Microsoft Dynamics, CAD Services, Infor Lawson, Deltek, ESRI ArcGIS and JD Edward EnterpriseOne.

### Where are files stored in OnBase?
OnBase offers a variety of choices as to where and how your files will be stored and managed, from simple network file shares on Windows or Linux file servers to purpose-built storage devices.

### Where to find Delete files in OnBase?
In the OnBase client, click Admin >> Utilities >> Document Maintenance to begin. Document Maintence is very similar to Recycle Bin found on Windows. 

### What are its file archiving and storage solutions?
EMC Centera, IBM Tivoli, Kom Networks KOMpliance, Document transfer and CD/DVD/Blu-ray authoring and export.

### How to access documents and data?
OnBase offers multiple ways to access documents and data easily. 
- Document Retrieval allows keyword-based searching of all available documents to a user.
- Custom Queries allow business users to search document types needed for specific business functions, simply by selecting commonly used  keyword criteria.
- Cross References can be used to link groups of document types together if one or more specific keyword values match. Very similar to inner join in a DBMS.
- File Cabinets and Folders - Documents can be grouped together using File Cabinets and Folders.

### How to integrate application with OnBase?
- Service Oriented Architecture (SOA) Integration - SOA enables business applications and databases to exchange information in a standardized format using centralized web services using SOAP and REST.
- Enterprise Integration Server - It provides real-time, data-level integration with other business applications using a configurable user interface that eliminates the need for custom code.
- Create your own Integration - The OnBase suite of APIs gives you the flexibility to create your own integrations with OnBase, providing your programmers with access points to integrate with OnBase documents, processes and more.

## TECHNICAL KNOWLEDGE 

### Difference between HTTP and HTTPS?
HTTP is a means of communcation that establishes a connection between the client and the server using a web browser. HTTPS is HTTP but secure, because it uses SSL to move data. SSL(Secure Sockets Layer) is an encrypted link between server and the browser that ensure the data passed between them are secure. 

### What is DNS?
Domian Name System is kind of like a phone book for the internet. It associates various information with domain names and their addresses. 

### What is the difference between a proxy and a VPN?
Both help you connect to a remote computer. Proxies hide your IP addresses by acting as a middlemen in the flow of internet traffic so you appear to be using it from a different location. For example, if you are trying to access a region restricted Youtube video, then Proxy is a good choice. They only act as a middlemen, they do not strip away your identity. 

VPN also acts as a middlemen between the computer and the server but it goes through a heavily ecrypted tunnel between the VPN Server and the computer remote network. This is ideal to use if the information, security and privacy is of high importance. 

### What is a Firewall?
It is a system designed to prevent unauthorized access to or from a private network. It monitors incoming and outgoing network traffic and decides whether to allow or block specific traffic based on a defined set of security rules.

### What is RAID?
It is a data storage technique which combines multiple physical hard disk drives into one for the purpose of data redundancy. 
- RAID 0 - Striping (Data is split into multiple blocks to offer superiod I/O performance.
- RAID 1 - Mirroring (Data is copied exactly to another drive in case of data backup.

### TCP vs IP?
IP is responsible for the logical addressing whereas TCP makes sure the packets are delivered successfully. 

# Internet Information Services (IIS)

### What is IIS and when is it used?
IIS is a web server that runs on the .NET platform on the Windows OS. If you want to host applications on a server that everybody can use, then IIS comes into play. It can be managed remotely with the use of CLI or PowerShell. 

### What protocols does it support?
It supports HTTP, HTTPS, FTP, FTPS, SMTP, etc.

### What is Application Pool in IIS?
They are used to seperate different workers accessing the same IIS resources and configuration. They are used to isolate our web applications for better security, performance and to keep running without affecting each other. 

### What is the name of the Default Application Pool in IIS?
It is called DefaultAppPool.

### What is Recycling of Aplication Pool?
Recycling application pool means recycle the worker process and the memory used for web application. By default, they recycle every 29 hours. 

### What are the main layers of IIS?
Two type of layers are Kernel Mode and User Mode. 

### What uses memory in the process?
Everything on the stack and heap—static variables and properties, anything in the memory cache, any objects that are referenced by another object, any blocks of memory waiting to be garbage collected.

### What is overlapped recycle?
No new requests would be handled until the current requests completed or the configurable timeout period elapsed (90 seconds by default).

### IIS CLI Commands? (Windows 2000)
- Display tasks - findweb and disptree
- Find Virtual website - findweb -c MachineName www.DomainName.com
- Display Admin Tree - disptree -a IIS://ComputerName OR disptree -a IIS://LocalHost/w3svc -n
- Create Tasks - mkw3site and mkwebdir
- Create Virtual website - Mkw3site -r RootDirectory DriveLetter:\FolderName -t NewServerName -h HostName www.MyNewWebsite.com
- Create Virtual web dir - Mkwebdir -c ComputerName -w "WebSiteName" -v DirectoryName,DriveLetter:\FolderName
- Stop a Virtual Site Without Interrupting the Entire Web Service - adsutil STOP_SERVER W3SVC/Server#
- Start a Virtual Site Without Interrupting the Entire Web Service - adsutil START_SERVER W3SVC/Server#




