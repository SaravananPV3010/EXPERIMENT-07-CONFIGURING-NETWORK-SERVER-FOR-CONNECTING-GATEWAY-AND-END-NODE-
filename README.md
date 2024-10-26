 ### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: 
To  configure  the Network server and end device for traferring data on the network
## Components required: 
End node stm 32 development kit , dragino LPS8, network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1bd434ca-1426-4102-8384-94473483543e)
 3. click on the add gateway 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/47c2e08d-6598-4437-8b07-f213d6f3b8ac)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/e62ff028-99bc-485e-9808-fbb6e124f8b2)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/a2e3ae58-6402-49e8-8f96-679059c1842c)
4. click on the lora options , lora - frequency plan 
5. click on channel s and create a new channel after which you can add a new end device 
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1fb72be5-e48d-4cde-a329-0cfb0d29070f)
6. add the attributesin the end device as  shown below 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/00bff30b-42fc-42d5-9540-285d270e41cb)

7.using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)



## OUTPUT 
### Home Page
![Screenshot 2024-10-26 102316](https://github.com/user-attachments/assets/bec0e82b-0680-4be2-975e-017e32795c0b)
### Gateway
![Screenshot 2024-10-26 104602](https://github.com/user-attachments/assets/311a92ba-a87d-42d7-9d51-fe5dea0736f4)
![Screenshot 2024-10-26 104632](https://github.com/user-attachments/assets/816e8192-b69d-4cf6-98ff-ea63877a419a)
### Channel
![Screenshot 2024-10-26 105212](https://github.com/user-attachments/assets/043490f2-8434-461c-bcda-c02680e1c5be)
### End Device
![Screenshot 2024-10-26 111002](https://github.com/user-attachments/assets/5731b3a2-bfe6-434c-8116-69e3f975bd64)
![Screenshot 2024-10-26 111016](https://github.com/user-attachments/assets/a3dba77a-332e-4211-a946-de50e00d7764)
![Screenshot 2024-10-26 111614](https://github.com/user-attachments/assets/62bf2de7-37a5-4c3b-b667-430e6b6be264)






## Results: 

  The Network server and end device for traferring data on the network has been accomplished.

