#
#
#
# **<em>Currently Work-in-Progress On Documentation For This Project.</em>**
#
#
#
# Phishing Email: Intelligence Analyst @@@ AP Solutions

#### - On November 29th, 2024, I received a suspicious job listing from a recruiter by the name of "Vijay Kiran" representing "AP Solutions." The email seemed very legitimate until I investigated further...

### <a href="https://docs.google.com/document/d/1qcuVk0nxRIwV5G5QM67-85SDaLe_3rPxoiWKVDoMEzQ/edit?tab=t.0#heading=h.tin35chbc89x" target="_blank">Incident Report:</a>

https://docs.google.com/document/d/1qcuVk0nxRIwV5G5QM67-85SDaLe_3rPxoiWKVDoMEzQ/edit?tab=t.0#heading=h.tin35chbc89x
#

1. Initially, I was excited, thinking a recruiter had gotten back to me. However, as I read through the email, my instincts kicked in, and something felt off about the job listing. The first thing I noticed was that the email was titled "Fwd: [message]," but there was no sign of a conversation thread, only the sender and me. This raised a red flag—if the email had been forwarded, I should have seen the full chain of conversation. I also realized I did not recall ever speaking with a Vijay Kiran, which prompted me to immediately dig deeper-for fun.

![1 1](https://github.com/user-attachments/assets/296a8064-4d7b-4304-a45f-d23615455680)
![1](https://github.com/user-attachments/assets/5ae09ac3-fb3f-4a88-8641-d217c2a03b4f)
#

2. I started by investigating the raw data to verify the DKIM (DomainKeys Identified Mail), SPF (Sender Policy Framework), and DMARC (Domain-based Message Authentication Reporting and Conformance) and noticed only the DKIM had passed but the SPF and DMARC are labeled as none/unknown. This is suspicious because although the DKIM had passed, it just means that the email had not been altered during transmission and that its digital signature matches the sender's domain. 
- The SPF failing means that the email was not sent through an authenticated mail server. 
- The DKIM verifies both DKIM and SPF as an extra layer of security, it failing means that the email did not align with the sender domain's policies. 
- I checked the originating IP address on VirusTotal, which confirmed that it is malicious, traced back to the US.

![2 1](https://github.com/user-attachments/assets/e2b8ef04-acd4-40e1-960d-6f6c14917952)
![2 2](https://github.com/user-attachments/assets/38cb9ba4-6f22-45a6-8df5-fc5a786a9af6)
#

3. 

![3 1](https://github.com/user-attachments/assets/550d4811-e242-4c54-aa78-7a4d55f87201)
![3 2](https://github.com/user-attachments/assets/1a27e014-a8ea-4324-8538-c0fd2f05d0f3)
#

4.

![4 1](https://github.com/user-attachments/assets/f47e7e6d-4c2d-4085-8eca-3ccaebad37df)
#

5.

![5 1](https://github.com/user-attachments/assets/6f1f43f1-7a7d-4fb0-8483-e775824cdddf)
![5 2](https://github.com/user-attachments/assets/5732e096-7b4e-47fc-9ee7-8bb2c143bc08)
#

6.

![6](https://github.com/user-attachments/assets/a9685efb-ee28-43e2-bf3a-3fdbc5b55ef8)
#

