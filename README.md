# Splunk SIEM Lab - SSH Log Analysis 🔍


<h2>Description</h2>
In this hands-on project, I explored the basics of Splunk Cloud, a powerful SIEM platform, by uploading log data, running search queries, and performing log analysis to detect security issues.
Acting as a security analyst for Buttercup Games, a fictional e-commerce company, I investigated failed SSH login attempts for the root account on the organization's mail server. This activity simulated a real-world scenario where a SOC analyst would need to respond to suspicious login behavior and determine whether a brute-force or unauthorized access attempt had occurred.

<h2>Tools Used</h2>

- <b>Splunk Cloud</b> 
- <b>SPL (Search Processing Language)</b>


<h2>Skills Practiced: </h2>

- <b>SIEM Log Analysis</b>
- <b>Incident Response Techniques</b>
- <b>Pattern Recognition in Logs</b>
- <b>Threat Hunting & Detection Queries</b>

<h2>Key Tasks</h2>

- ### Uploaded and indexed log data (tutorialdata.zip)
![image](https://github.com/user-attachments/assets/987980ea-261b-46f1-9665-0094b97d2845)

  
- ### Queried using index=main and applied filters using wildcards and fields
![Splunk index=main](https://github.com/user-attachments/assets/5a995bd2-66cc-4185-a681-1fc6af1391ee)


- ### Identifying Event Origins by Host
  
This screenshot displays the host field, which indicates the origin of each event in the network. In this search, we are seeing events from five distinct hosts used by Buttercup Games:

<b>mailsv</b> – The mail server for Buttercup Games. Focus on events from this host for potential email-related threats or login activity.

<b>www1</b> – One of Buttercup Games' web application servers.

<b>www2</b> – Another web application server, likely part of a load-balanced environment.

<b>www3</b> – A third web application server, reinforcing redundancy and availability.

<b>vendor_sales</b> – Contains data related to retail and sales systems, such as third-party vendor activity.

![Splunk host](https://github.com/user-attachments/assets/6d66f586-51c1-492e-8328-7b0f25fc6736)


- ### Identified failed SSH login attempts from external IPs targeting the mail server
![Failed passwords](https://github.com/user-attachments/assets/00893df1-67f6-4f28-be7b-d72358b6800c)


- ### Investigated scan patterns pointing to potential recon or exploitation attempts


<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
