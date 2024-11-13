# Phishing Email: Deal Watchdogs - Amazon Black Friday Deals

#### - On November 6th, 2024, I received a suspicious email from a company called 'Deal Watchdogs.' The email exhibited several phishing characteristics, including an unfamiliar sender domain, a poorly designed layout, blurry fonts, and addressing me by my email instead of my actual name.


#
#
#
## >*Currently work-in-progress on documentating this investigation*
#
#
#

#### - Before I started my investigation, I made sure to check that my Virtual Machine is on a 'host-only' mode so that in the event there's a malicious payload from the link, it will be isolated. Doing this will prevent it from accessing my host network and further minimizing risk. 

![1 01](https://github.com/user-attachments/assets/45503985-2dec-4add-a726-affc3a383d0e)
#

1. I began by taking a look at the initial email header and found nothing unusual yet; however, when I clicked into the email, something spoke out to me as fishy. Other than the email being addressed to my email address and not my name, the first thing is that the sender doesn't look like a legitmate email a company would use if they're company name is 'Deal Watchdogs'. The next suspicious indicator is that the email contains 3 different font colors and sized awkardly from medium, to large, and to small. The last thing that spoke out to me is that the last 3 clickable links are very blurry, which I tend to find in a lot of phishing emails.

![Screenshot 2024-11-12 110838](https://github.com/user-attachments/assets/0750ac69-8842-4db0-bc3f-eb9c07062b21)
![Screenshot 2024-11-12 111930](https://github.com/user-attachments/assets/2a2d5028-3ad5-4875-82c3-9588e7c622e9)
![Screenshot 2024-11-12 112026](https://github.com/user-attachments/assets/340aef42-fbab-4126-b8d5-b4889accf920)
#

2. Next, I examined the raw data to find more information, identifying both the attacker's IP address and email address. I checked the email's DKIM (DomainKeys Identified Mail), SPF (Sender Policy Framework), and DMARC (Domain-based Message Authentication Reporting and Conformance) and noticed that they are all labeled as unknown. Together, DKIM, SPF, and DMARC function like a background check on email senders, to make sure they really are who they say they are. The absence of these verifications is another red flag.

![Screenshot 2024-11-12 113053](https://github.com/user-attachments/assets/55382600-a5b7-490e-b4dc-a1ae44b98d91)
#

2.1. When I investigate further into the raw data, I noticed 2 strange things. The first being that there are LinkedIn headers such as LinkedIn-Class, LinkedIn-Template, or LinkedIn-ID to look like a LinkedIn alert or notification but the email is claiming to contain Amazon deals. The two do not correlate at all. The second suspicious item(s) are the 6 lengthy URL re-direct links to an unknown domain that does not represent 'Deal Watchdogs' or LinkedIn. The structure of these headers and URLs is typical of phishing attempts, where attackers spoof a well known/popular site to present itself as legitimate and use complex, randomized domains to evade detection.  

![Screenshot 2024-11-12 113154](https://github.com/user-attachments/assets/896439ee-ddad-4110-9919-3ac8e0399c8f)
#

3. I investigate the sender's IP Address on VirusTotal and confirm that is is flagged as malicious, originating from Ireland. This confirmation adds another layer of validation that the email is part of a broader malicious campaign.

![deal watchdogs ip addr](https://github.com/user-attachments/assets/6a36b22b-2510-4d3f-ac01-99fb57287693)
#

4.

![Screenshot 2024-11-12 114702](https://github.com/user-attachments/assets/e03a6535-8e5f-466a-a286-24bad15e20f7)
![Screenshot 2024-11-12 115121](https://github.com/user-attachments/assets/cff786e9-249a-4f4a-af87-4ac2fa5f0161)
![Screenshot 2024-11-12 115212](https://github.com/user-attachments/assets/e51be5ab-bc73-4a25-b3e4-6dcaaada0b80)
![Screenshot 2024-11-12 115231](https://github.com/user-attachments/assets/c14fd12a-e091-4451-b557-6986fa87ec38)


![Screenshot 2024-11-12 115517](https://github.com/user-attachments/assets/dc2e26c4-21ce-4586-a557-e247a61f3bcc)
![Screenshot 2024-11-12 115606](https://github.com/user-attachments/assets/52f55d3f-b947-422a-b16c-e5071c347219)
![Screenshot 2024-11-12 115911](https://github.com/user-attachments/assets/33e6996d-407e-4d5f-acea-5ec0d71e1dd3)


![Screenshot 2024-11-12 131538](https://github.com/user-attachments/assets/19a066ad-a1d7-434d-8e19-7ec0e6a47d1a)
![Screenshot 2024-11-12 131721](https://github.com/user-attachments/assets/a4e1db51-6308-4670-b859-f8a09879fcfd)


![Screenshot 2024-11-12 131940](https://github.com/user-attachments/assets/6846f4af-d259-4f88-bc96-8b30135f14e8)



