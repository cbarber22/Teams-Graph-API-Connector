# Teams Graph API Connector
 Custom connector for Teams Graph API usage with the Power Platform

Purpose: 
The goal for this GITHUB repo and its contents are to provide you an alternative way to directly connect to Microsoft Teams via a Custom Connector action. Currently the actions in Power Automate for Microsoft Teams are still in Preview at the time of this posting hence the original development of this connector. If you are curious on how to configure the Custom Connector or the custom connector with the Graph API feel free to reach out or review the articles I’ve written on this topic.

Overview of the Custom Connector with Demo:

https://youtu.be/lxqpFYtHwOQ

Articles:

https://www.linkedin.com/pulse/creating-azure-app-registration-use-graph-api-barber-/

https://www.linkedin.com/pulse/microsoft-teams-graph-api-christopher-barber-/

https://www.linkedin.com/pulse/what-microsoft-graph-christopher-barber-/

Provided in the json file is a list of an original set of actions which I have outlined below. Feel free to download and reuse, I’ll be updating this connector as I develop it further. 

Actions:

•	GetTeams:

•	Delete Channel:

•	Retrieve Messages:

•	MessageReplies:

•	CloneTeam:

•	CreateChannel:

•	ArchiveTeam:

Steps for Configuration:

Configure App Registration in Azure Portal with the following permissions:
   Directory.ReadWrite.All
   Group.ReadWrite.All
   GroupMember.ReadWrite.All
   User.Read
   User.ReadWrite.All
   
Import Connector File Provided within PowerApps

Configure Connector
1.	Import the file provided.
2.	Within the General Tab, provide a new icon & description for the connector.
3.	Within the Security Tab select Auth Type of OAuth 2.0, select Azure Active Directory and fill in the required parameters.
   a.	Client ID: 
   b.	Client Secret: 
   c.	Tenant ID: 
   d.	Resource URL: https://graph.microsoft.com


•	GetTeamsApp:

•	RemoveMember:

•	AddOwner:

•	RemoveOwner:

•	AddMember:

•	AddTabs:

•	ChannelUpdates:
