# Phishing Email: Deal Watchdogs - Amazon Black Friday Deals

#### - On November 6th, 2024, I received a suspicious email from a company called 'Deal Watchdogs.' The email exhibited several phishing characteristics, including an unfamiliar sender domain, a poorly designed layout, blurry fonts, and addressing me by my email instead of my actual name.


### <a href="https://docs.google.com/document/d/1brqaiAT-QYt1p6rPJLJyaEAWnq4QfOq5Ow9qErMYgv4/edit?tab=t.0#heading=h.jc6e3jt049tw" target="_blank">Incident Report:</a>

https://docs.google.com/document/d/1brqaiAT-QYt1p6rPJLJyaEAWnq4QfOq5Ow9qErMYgv4/edit?tab=t.0#heading=h.jc6e3jt049tw
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

2.1. When I investigate further into the raw data, I noticed 2 strange things. The first being that there are LinkedIn headers such as LinkedIn-Class, LinkedIn-Template, or LinkedIn-ID to look like a LinkedIn alert or notification but the email is claiming to contain Amazon deals. The two do not correlate at all. The second suspicious item(s) are the 6 lengthy URL redirect links to an unknown domain that does not represent 'Deal Watchdogs' or LinkedIn. The structure of these headers and URLs is typical of phishing attempts, where attackers spoof a well known/popular site to present itself as legitimate and use complex, randomized domains to evade detection.  

![Screenshot 2024-11-12 113154](https://github.com/user-attachments/assets/896439ee-ddad-4110-9919-3ac8e0399c8f)
#

3. Furthermore, I investigate the sender's IP Address on VirusTotal and confirm that it is flagged as malicious, originating from Ireland. This confirmation adds another layer of validation that the email is part of a broader malicious campaign.

![deal watchdogs ip addr](https://github.com/user-attachments/assets/07f9c0dc-d174-4515-b488-a017a5e1e061)
#

4.  With conclusive evidence that this email is malicious, I proceeded to examine the link in a controlled environment to observe any potential actions it triggers for my own learning. Before clicking, I've taken a snapshot of my virtual machine to create a safe restore point, allowing me to revert to its original state if needed.

![Screenshot 2024-11-12 114702](https://github.com/user-attachments/assets/e03a6535-8e5f-466a-a286-24bad15e20f7)
#

5.  After I click into the malicious link, I am redirected THREE times to different articles written by "bloggers" reviewing the product I clicked into but I can't seem to click on the author's name to see what else they have reviewed. Which is strange because wouldn't a blogger have more than just 1 blog or review? I then tried to click onto the 2939 reviews by other "purchasers" but could not click into that either. Overall, I was impressed by the length these phishing attackers went to to make these websites look legitimate because attackers will do this at an attempt to throw off browser based security measures and by having different domains- it makes it harder for pattern recognition algorithms to mark these sites as malicious. 

![Screenshot 2024-11-12 115121](https://github.com/user-attachments/assets/cff786e9-249a-4f4a-af87-4ac2fa5f0161)
![Screenshot 2024-11-12 115517](https://github.com/user-attachments/assets/dc2e26c4-21ce-4586-a557-e247a61f3bcc)
![Screenshot 2024-11-12 115606](https://github.com/user-attachments/assets/52f55d3f-b947-422a-b16c-e5071c347219)
#

6. Ultimately, I realized when clicking into several different products, the links would redirect me multiple times to different articles expressing how great the product is, given an obscene discount ranging from 50-80% off, and then finally to a spoofed website to "buy" the product but never actually sending me directly to Amazon to buy the product! By doing this, the attackers are bypassing detection from email filters and anti-virus softwares by avoiding direct links to the malicious content. 
 
![Screenshot 2024-11-12 131538](https://github.com/user-attachments/assets/19a066ad-a1d7-434d-8e19-7ec0e6a47d1a)
![Screenshot 2024-11-12 131721](https://github.com/user-attachments/assets/a4e1db51-6308-4670-b859-f8a09879fcfd)
#

7. To conclude my investigation, I bought all 10 products, closed out all the Window's tabs, quarantined the malicious email, and reverted my VM back to its original state.

![Screenshot 2024-11-12 131940](https://github.com/user-attachments/assets/6846f4af-d259-4f88-bc96-8b30135f14e8)
#

# <a href="https://docs.google.com/document/d/1brqaiAT-QYt1p6rPJLJyaEAWnq4QfOq5Ow9qErMYgv4/edit?tab=t.0#heading=h.jc6e3jt049tw" target="_blank">Incident Report</a>
