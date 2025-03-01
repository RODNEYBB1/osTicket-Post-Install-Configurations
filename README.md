<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)


<h2>Configuration Steps</h2> 

AFTER INSTALLATION OF OS TICKET WE WILL NEED TO FIGURE ROLES FOR GROUPING PERMISSIONS.

*FIRST ON THE TOP RIGHT PANEL YOU CAN SEE ADMIN PANEL CLICK ON THIS TAB, NOW NAVIGATE TO >AGENTS > ROLES ADD A NEW ROLE. NAME THIS (SUPREME ADMIN). THEY WILL NEED ACCESS TO ALL COMPONETS. NEXT MOVE TO PERMISSIONS AND SELECT ALL BOXES AS THE SUPREME ADMIN WILL BE ALLOWED ACESS TO ALL AREAS IN TICKETS/TASKS/KNOWLEDGEBASE. ONCE COMPLETE CHOOSE ADD ROLE .

![image](https://github.com/user-attachments/assets/f117665a-9ef4-4ed8-9cac-57d02ed93811)

![image](https://github.com/user-attachments/assets/4ce0cad7-8d1c-42e9-ac4c-df4edf5a7e38)

NEXT WE WILL HAVE TO CONFIGURE DEPARTMENTS. THIS WILL BE FOR TICKET VISABILITY, HELPDESK VS SYSAdmin, VS NETWORKING. WE WILL GO TO DEPARTMENTS AND ADD NEW. NOW IN ADD DEPARTMENT UNDER PARENT SELECT TOP-LEVEL-DEPARTMENT AND NEXT NAME THIS SYSAdmins AND LEAVE SETTINGS THE SAME. SCROLL DOWNN AND CREATE A DEPARTMENT. AND NOW WE HAVE ADDED SYSadmins TO THE LIST OF DEPARTMENTS.

![image](https://github.com/user-attachments/assets/c6beee1d-fcb2-4dd6-a4b3-df2fae7537a7)

![image](https://github.com/user-attachments/assets/d311c276-3fa2-4c46-a87c-cc0d808301a2)

ONCE DEPARTMENTS ARE SETUP WE WILL NOW CONFIGURE TEAMS. FROM THE SAME SCREEN NOW NAVIGATE TO THE TEAMS TAB CHOOSE ADD NEW TEAM. NAME THIS TEAM ONLINE BANKING AND CREATE. WE WILL ALSO HAVE TO IMPLEMENT AND ALLOW ANYONE TO CREATE A TICKET SO THEY WILL NOT HAVE TO REGISTER.

![image](https://github.com/user-attachments/assets/40b67bdb-336b-4649-9152-b50c0f53a41e)

NOW WE WILL CREATE AND CONFIGURE AGENTS/WORKRS. ON THE AGENTS TAB CLICK AND ADDD NEW. FOR THIS PURPOSE WE WILL ADD TWO AGENTS WITH DIFFERENT PROFILES. THE FIRST AGENT IS JANE WHO SIS A SURPREME ADMI AND HAS ACCESS TO ALL AS AN ADMIN. ONT ACCOUNT FILLO OUT FIRST AND LAST NAME AS WELL AS EMAIL ADDRESS. NOW CREATE USER NAME & PASSWORD. ONCE YOU CHOOSE A PASSWORD *UNCHECK CHANGE AT NEXT LOGIN. 

![image](https://github.com/user-attachments/assets/4f7a5c70-27a9-4ce5-8ceb-a6d0cbc18f73)

NEXT WILL GO THROUGH THE ACCESS TAB ON THE DROP DOWN MENU SELECT SYSadmin AND THEN SUPREME ADMIN. UNDER PERMIISSONS MAKE SURE ALL TABS ARE SELECTED. FINALLY UNDER THE TEAMS TAB ON THE DROP DOW MENUS SELECT ONLINE BANKING.

![image](https://github.com/user-attachments/assets/1f1b8faa-19b1-421a-80ff-d49f1882d588) 

![image](https://github.com/user-attachments/assets/2d5045f3-a5ca-4b65-934a-52ee044be129)

![image](https://github.com/user-attachments/assets/b06363af-07b3-46dd-a70d-1fe07c7b87a9)

NEXT WE WILL CREATE THE SECOND AGENT JOHN WITH LIMITED ACCESS AS A WORKER. FROM THE AGENTS TAB CLICK ON A ADD NEW. JUST AS BEFORE FILL OUT ALL INFO AND SET PASSWORD. ON THE NEXT TAB UNDER THE DROP DOWN SELECT SUPPORT AND NOW VIEW ONLY ACCESS. NOW THE TABS FOR PERMISSONS AND TEAMS WE WILL LEAVE AS IS AND CREATE. ONCE YOU CREATE YOU CAN NOW SEE BOTH NEW AGENTS ARE ADDED.

![image](https://github.com/user-attachments/assets/784ddb7c-358b-416d-9e27-fd5a67edcfb0)

![image](https://github.com/user-attachments/assets/3da10a6b-77e1-4df1-9496-acff49275e78)

![image](https://github.com/user-attachments/assets/071c2a24-f6a1-4541-a1cd-f62230e21851)

![image](https://github.com/user-attachments/assets/a8fbdfa6-790c-4a6a-98d1-393a694f7c31)

WE WILL ALSO HAVE TO ADD USERS/CUSTOMERS, ON THE TOP RIGHT SELECT AGENT PANEL. ONCE THERE SELECT USERS AND ADD NEW USER. FILL OUT  USER INFO THEN PRESS ADD USER ONCE DONE YOU WLL SEE USER WAS ADDED.

![image](https://github.com/user-attachments/assets/8879fec7-cabd-48e5-9d1d-c1a18469e3a1)

ONCE THE STEPS ABOVE ARE CREATEDWE WILL NEED TO SET SLA PRIORITIES. THESE WILL DICTATE WHAT IS MOST IMPORTANT AND HOW LONG A HELP DESK WILL HAVE TO RESOLVE THE CUSTOMER ISSUES. NOW WE ARE BACK IN THE ADMIN PANEL TOP RIGHT SELECT AGENT AND THIS WILL SWITCH YOU BACK TO ADMIN. SELECT MANAGE AND THEN SLA. WE CREATE THREE DIFFERENT SLA GROUPS. SEV-A WITH A HIGH IMPORTANCE AND NEEDED RESPONSE TIME OF WITHIN ONE HOUR OF TICKET REQUEST WITH A 24/7 RESPONSE TIME.SEV-B WITH AFOUR HOUR RESPONSE TIME AND ALSO WITH A 24/7 RESPONSE TIME. AND LAST BUT NOT LEAST SEV-C WITH REPSONSE TIME OF EIGHT HOURS  AND ONLY WORKED DURING A MON-FRI 8AM-5PM WITH US HOILDAYS. NOW ONCE ALL SLA'S ARE ADDED THE ARE NOW VISIBLE IN THE SLA PLAN.

![image](https://github.com/user-attachments/assets/75090b5f-9457-4496-a21e-4df09dc76572)

![image](https://github.com/user-attachments/assets/6285931f-64a4-4406-9959-bae7abf5f1ff)

![image](https://github.com/user-attachments/assets/f152fc33-9c68-47ba-a144-8c436a595ceb)


FINALLY HELP TOPICS NEED TO BE CREATED TO HELP USERS SELECT AN APPROPIATE CATERGORY THAT DESCRIBES THEIR PROBLEM SO THAT AGENTS GET AN IDEA OF WHAT PROBLEM IS DESCRIBED IN THE TICKET. TO MAKE A NW HELP TOPIC, ENTER THE ADMIN PANEL AND OPEN MANAGE MENU. CLICK ON HELP, IN THIS CASE WE ADD THE FOLLOWING ORDER TO USE LATER FOR WHEN WE CREATE A NEW TICKET THAT HAVE TO BE RESOLVED : BUSINESS CRITICAL OUTAGE, PERSONAL COMPUTER ISSUES, EQUIPMENT RESET, AND PAASWORD RESET.

![image](https://github.com/user-attachments/assets/0d030975-5205-4a45-b2fb-e0fd052a7445)

![image](https://github.com/user-attachments/assets/14edeeca-da07-4b68-ae28-b37f3c39e5de)

![image](https://github.com/user-attachments/assets/af8f3260-a36e-4558-96a9-cecb89d3848a)


![image](https://github.com/user-attachments/assets/f90fb05f-384b-48d4-bfef-45785005361d)


osTICKET CONFIGURATIONS ARE COMPLETE ------


NOW THAT THE CONFGURATIONS HAVE BEEN SET IN PLACE , WE CAN NOW UTIILIZE osTICKET AS A PROPER TICKETING SYSTEM. WE CAN CREATE TICKETS AND BE ABLE TO TRIAGE THEM AS IF I/WE ARE IN A REAL ENVIROMENT. 











































































