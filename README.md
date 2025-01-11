# Information Gathering with Burp Suite 

<h2>Description</h2>
In this reconnaissance task, I was introduced to the Burp Suite tool for proxy use on firefox. I set the default proxy address to 127.0.0.1 in the HTTP Proxy field over port 8080 (Burp default port) and caught traffic between my kali VM firebox browser to tesla.com and microsoft.com. This enumerated a server and hostname that the tesla webpage was using. 

<h2>Languages and Utilities Used</h2>

- <b>Burp Suite</b>

<h2>Environments Used </h2>

- <b>Kali Linux</b> 

<br />
<br />
Starting a temporary project on burp suite for the first time. 

![1) starting burp suite for the first time](https://github.com/user-attachments/assets/22e88a14-6924-4835-84bc-24944f086e85)

<br />
<br />
Configuring firefox general network settings to include 127.0.0.1:8080 as the burp suite http proxy. 

![2) configuring entwrok proxy settings for firefox](https://github.com/user-attachments/assets/9235b69b-f266-4ae4-a902-7a28c921e8fa)

<br />
<br />  
Connected to https://burp to download the CA Certificate. 

![3) https burp save CA certificate](https://github.com/user-attachments/assets/5ff89733-2931-4350-bf91-4071a7b2ad90)

<br />
<br />
In my firefox Privacy & security settingsm I went to certificates>add/upload> selected the Burp CA certificate, and made sure both boxes were checked before clicking OK. 

![4) importing downloaded certificate, check both boxes in privacy and security certificate settings](https://github.com/user-attachments/assets/092a5343-bdf3-4ff2-a57a-6cf4dee60299)

<br />
<br />
With Burp up and running intercepting traffic, I visited tesla and microsoft to generate telemetry. 

![5) visited tesla and microsoft and captured site map](https://github.com/user-attachments/assets/35662d89-4b83-4afc-ac48-1762cc95679f)

<br />
<br />  
Diving deeper into tesla's pages shows a hostname and server that is used. 

![6) enumerating hostname and server for tesla](https://github.com/user-attachments/assets/448acc79-b3a9-4870-b69f-272367f4237b)

<br />
<br />
