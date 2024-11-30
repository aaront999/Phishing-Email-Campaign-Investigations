# Phishing Email: Intelligence Analyst @@@ AP Solutions

#### - On November 29th, 2024, I received a suspicious job listing from a recruiter by the name of "Vijay Kiran" representing "AP Solutions." The email seemed very legitimate until I investigated further...

### <a href="https://docs.google.com/document/d/1qcuVk0nxRIwV5G5QM67-85SDaLe_3rPxoiWKVDoMEzQ/edit?tab=t.0#heading=h.tin35chbc89x" target="_blank">Incident Report:</a>

https://docs.google.com/document/d/1qcuVk0nxRIwV5G5QM67-85SDaLe_3rPxoiWKVDoMEzQ/edit?tab=t.0#heading=h.tin35chbc89x
#

1. Initially, I was excited, thinking a recruiter had gotten back to me for a role I applied to. However, as I read through the email, my instincts kicked in, and something felt off about the job listing. The first thing I noticed was that the email was titled "Fwd: [message]," but there was no sign of a conversation thread, only the sender and me. This raised a red flag—if the email had been forwarded, I should have seen the full chain of conversation. I also realized I did not recall ever speaking with a Vijay Kiran, which prompted me to immediately dig deeper-for fun.

![1 1](https://github.com/user-attachments/assets/296a8064-4d7b-4304-a45f-d23615455680)
![1](https://github.com/user-attachments/assets/5ae09ac3-fb3f-4a88-8641-d217c2a03b4f)
#

2. I started by investigating the raw data to verify the DKIM (DomainKeys Identified Mail), SPF (Sender Policy Framework), and DMARC (Domain-based Message Authentication Reporting and Conformance) and noticed only the DKIM had passed but the SPF and DMARC are labeled as none/unknown. This is suspicious because although the DKIM had passed, it just means that the email had not been altered during transmission and that its digital signature matches the sender's domain. 
- The SPF failing means that the email was not sent through an authenticated mail server. 
- The DMARC verifies both DKIM and SPF as an extra layer of security, it failing means that the email did not align with the sender domain's policies. 
- I checked the originating IP address on VirusTotal, which confirmed that it is malicious, traced back to the US.

![2 1](https://github.com/user-attachments/assets/e2b8ef04-acd4-40e1-960d-6f6c14917952)
![2 2](https://github.com/user-attachments/assets/38cb9ba4-6f22-45a6-8df5-fc5a786a9af6)
#

3. I wasn't satisfied with the evidence I gathered so far, so I looked into AP Solutions to look for more information on the company but could not find any straight forward legitimate site to read into, which raised another red flag for me.

![3 1](https://github.com/user-attachments/assets/550d4811-e242-4c54-aa78-7a4d55f87201)
![3 2](https://github.com/user-attachments/assets/1a27e014-a8ea-4324-8538-c0fd2f05d0f3)
#

4. I cross-referenced the address Mr. Kiran claimed for the business. It turns out that the address is actually an office building that hosts virtual office suites, which can be commonly used by legitimate businesses. However, the suite in question is still listed as available for rent, raising doubts about the legitimacy of the business. 

![4 1](https://github.com/user-attachments/assets/f47e7e6d-4c2d-4085-8eca-3ccaebad37df)
#

5. I conducted a WHOIS lookup on the domain used by Mr. Kiran’s email and discovered that it was registered on March 12, 2023, making it a relatively new domain. Then I looked further by searching the domain on Talos Intelligence and was not able to find any related ip addresses associated, which draws up another concern.
- Additionally, the domain is registered in Reykjavik, Iceland, which raises more suspicion about its authenticity. 

![5 1](https://github.com/user-attachments/assets/6f1f43f1-7a7d-4fb0-8483-e775824cdddf)
![5 2](https://github.com/user-attachments/assets/5732e096-7b4e-47fc-9ee7-8bb2c143bc08)
#

6. As a final step, I wanted to verify whether Viray Kiran was a real person representing AP Solutions. 
- Upon further investigation, I found someone with the same name and job title, but this individual actually represents a legitimate company: AP Federal!! This led me to believe that the attacker was attempting to impersonate the real Vijay Kiran. 
- With this discovery, along with the other evidence gathered, I can confidently conclude that this email is part of a broader phishing campaign, designed to build trust and ultimately steal personal information if I were to engage with the attackers and submit any sensitive data.

![7](https://github.com/user-attachments/assets/57f7219b-b753-4a6b-b6cf-072c14bed991)
#

# <a href="https://docs.google.com/document/d/1qcuVk0nxRIwV5G5QM67-85SDaLe_3rPxoiWKVDoMEzQ/edit?tab=t.0#heading=h.tin35chbc89x" target="_blank">Incident Report</a>
