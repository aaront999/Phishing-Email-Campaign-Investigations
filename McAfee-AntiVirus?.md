# Phishing Email: McAfee Anti-Virus

#### On October 17th, 2024, I received a suspicious email from a sender attempting to impersonate the computer security company McAfee. The email displayed several phishing characteristics, such as an unfamiliar sender domain and stressing urgency for the user to react and take action.

### <a href="https://docs.google.com/document/d/1lsfPdQwsRPyWe74U6kB_ca3As02XeR4o7CFkpN_4q6Y/edit?tab=t.0#heading=h.tin35chbc89x" target="_blank">Incident Report:</a>

https://docs.google.com/document/d/1lsfPdQwsRPyWe74U6kB_ca3As02XeR4o7CFkpN_4q6Y/edit?tab=t.0#heading=h.tin35chbc89x
#

#### Before I started my investigation, I made sure to check that my Virtual Machine is on a 'host-only' mode so that in the event there's a malicious payload from the link, it will be isolated. Doing this will prevent it from accessing my host network and further minimizing risk. 

![1 01](https://github.com/user-attachments/assets/45503985-2dec-4add-a726-affc3a383d0e)
#

1. I began by investigating the malicious email and immediately noticed that the header displays a strong sense of urgency, which is a common tactic used by attackers to prompt immediate action. The sender’s email address appears unusual and inconsistent with typical support addresses used by legitimate companies. Additionally, the greeting is directed to my email address rather than using my actual name, suggesting a lack of personalization that is typical in phishing attempts.

![1 02](https://github.com/user-attachments/assets/aa6c9385-28a9-4352-9de5-8ff8e82bfb5f)
![1 03](https://github.com/user-attachments/assets/ab7d3397-7a5c-4149-882b-317065c66698)
![1 04](https://github.com/user-attachments/assets/265e2848-9ddd-4a62-a778-14900229f34b)
#

2. To gather additional evidence, I examined the email's source code, where I identified three suspicious, lengthy domains embedded within the content. These domains included a mix of numbers, dashes, and acronyms, suggesting they could function as redirects to external sites. The structure of these URLs is typical of phishing attempts, where attackers use complex, randomized domains to evade detection.

![1 05](https://github.com/user-attachments/assets/c8d942f4-ae3c-4c39-a8ab-290e939b4f3d)
#

3. Furthermore, I examined the raw data to find more information, identifying both the attacker's IP address and email address. I checked the email's DKIM (DomainKeys Identified Mail), SPF (Sender Policy Framework), and DMARC (Domain-based Message Authentication Reporting and Conformance) and noticed that they are all labeled as unknown. Together, DKIM, SPF, and DMARC function like a background check on email senders, to make sure they really are who they say they are. The absence of these verifications is another major red flag. I also decoded the base64 code from the raw data, using CyberChef but could not find any data of relevance. 

![1 06](https://github.com/user-attachments/assets/1a29c029-bf43-4684-81cb-debb1a878f75)

 - I also investigated the sender's IP address, which VirusTotal has flagged as malicious, originating from Turkey. This confirmation adds another layer of validation that the email is part of a broader malicious campaign.

![1 07](https://github.com/user-attachments/assets/9b21cf28-e7f8-4302-abbd-4b0c5e861f20)
#

4. With conclusive evidence that this email is malicious, I proceeded to examine the link in a controlled environment to observe any potential actions it triggers for my own learning. Before clicking, I've taken a snapshot of my virtual machine to create a safe restore point, allowing me to revert to its original state if needed.

![2 01](https://github.com/user-attachments/assets/ae36d571-e1a5-47d5-9184-3d00b24490f8)
![2 02](https://github.com/user-attachments/assets/312fd20e-c211-4739-85e0-d6d9389b262e)
#

5. Once I click the initial malicious link, I am redirected twice and find more malicious linked domains in the source codes.

![2 03](https://github.com/user-attachments/assets/d1522332-c27b-41e6-ad1b-4476ce4c7003)
![3 01](https://github.com/user-attachments/assets/bbe27f19-9d03-46c7-b2ac-d0543e814e39)
![3 02](https://github.com/user-attachments/assets/91532841-3da6-4f32-8f71-2c2dcb8de24c)
#

6. Eventually, it takes us to a checkout screen that request for the user's private information and credit card details.

![4 01](https://github.com/user-attachments/assets/fc2a0e2a-63b9-4aad-b246-58873458c00d)
![4 02](https://github.com/user-attachments/assets/803c3f40-6a6e-4320-9025-82800b92b4f2)
#

7. After I entered all my information and social security number, I closed out of the window, quarantined the malicious email, and reverted my VM back to its original state.

![4 03](https://github.com/user-attachments/assets/2ffe4cf0-4b81-4768-af08-e1c6ff1bbedf)
#

# <a href="https://docs.google.com/document/d/1lsfPdQwsRPyWe74U6kB_ca3As02XeR4o7CFkpN_4q6Y/edit?tab=t.0#heading=h.tin35chbc89x" target="_blank">Incident Report</a>
