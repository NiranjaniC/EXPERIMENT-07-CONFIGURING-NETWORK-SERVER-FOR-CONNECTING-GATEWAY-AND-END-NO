### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: 
To  configure the Network server and end device for transferring data on the network
## Components required: 
End node stm 32 development kit , Dragino LPS8, Network server 

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
 3. Click on the add gateway 
 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/47c2e08d-6598-4437-8b07-f213d6f3b8ac)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/e62ff028-99bc-485e-9808-fbb6e124f8b2)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/a2e3ae58-6402-49e8-8f96-679059c1842c)
4. Click on the lora options , lora - frequency plan 

5. Click on channels and create a new channel after which you can add a new end device
   
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1fb72be5-e48d-4cde-a329-0cfb0d29070f)

6. Add the attributes in the end device as  shown below 

 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/00bff30b-42fc-42d5-9540-285d270e41cb)
 
7.Using AT commands configure end device in serial port utility
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
<img width="1919" height="970" alt="image" src="https://github.com/user-attachments/assets/db3c5391-8a0e-43f4-9e34-b80d816e3323" />

<img width="1919" height="809" alt="image" src="https://github.com/user-attachments/assets/124e9fcb-e700-4e52-89e5-467601230815" />

<img width="1917" height="802" alt="image" src="https://github.com/user-attachments/assets/df9c9555-d329-4086-8b1d-f4dbaabc15fd" />

<img width="1435" height="797" alt="Screenshot 2025-11-14 101613" src="https://github.com/user-attachments/assets/152f590b-9c0b-48db-a1ca-1e9311e5857c" />

<img width="1919" height="811" alt="image" src="https://github.com/user-attachments/assets/c6248fa8-d6f9-4ee4-99f2-ee503f8e08be" />

<img width="1919" height="862" alt="image" src="https://github.com/user-attachments/assets/c166c6df-a31d-4f12-8f8b-3f394504ee45" />

<img width="1919" height="865" alt="Screenshot 2025-11-14 151631" src="https://github.com/user-attachments/assets/7bea8c85-f7c7-4c5d-849f-e05e5a4879f4" />

<img width="1917" height="1019" alt="image" src="https://github.com/user-attachments/assets/a487cbfb-f208-47ad-8a8b-41f8c835c7b9" />

<img width="1919" height="1013" alt="image" src="https://github.com/user-attachments/assets/b31f6a46-4132-4a3d-99b6-8458b39063cb" />

<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/bd10e38b-4785-4c14-965d-9c5801020d63" />

<img width="1919" height="1024" alt="image" src="https://github.com/user-attachments/assets/bf4d1841-6707-419e-9ca0-88a8d432fc07" />

<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/fdc10718-4bac-4221-b3f6-2d4f0a24dbf9" />

<img width="1919" height="1000" alt="image" src="https://github.com/user-attachments/assets/768fc268-543e-437d-aace-dc02ef61e270" />

<img width="1918" height="1019" alt="image" src="https://github.com/user-attachments/assets/34ba8642-a517-4e1e-bf8c-df00351ffbb7" />

<img width="1919" height="1000" alt="image" src="https://github.com/user-attachments/assets/9dca6bd0-6eb1-42de-9357-f3e6bb32a2e0" />

<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/7c4dcbe9-72f4-47e2-a2dc-51fc9132abb7" />

## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
