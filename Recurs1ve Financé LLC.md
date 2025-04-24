# Phishing Email: 3 positions open at Recursive Financé LLC.

#### - On April 22nd, 2025, I was contacted by an HR Manager named “William Rosen,” claiming to represent a company called “Recursive Finance LLC.” At first glance, the email looked impressively legitimate — polished, professional, the kind you'd expect from a real financial firm. But something felt off... and once I started digging, the red flags came fast.

### <a href="https://docs.google.com/document/d/1tNiKY1832EJ5cECSSFa0h5fOxyQQV9gjawZd9fqd5E0/edit?usp=sharing" target="_blank">Incident Report:</a>

https://docs.google.com/document/d/1tNiKY1832EJ5cECSSFa0h5fOxyQQV9gjawZd9fqd5E0/edit?usp=sharing
#


1. I started by examining the email header and content. At first glance, it looked extremely legitimate—well-formatted, professional language, and structured like a real recruiting email. But a few things raised red flags:

  - Unrealistic Pay Range: The listed hourly rate ranged from $47 to $110/hour across three roles. That’s $97,760 to $228,800 annually, which immediately sounded too good to be true—especially for roles like Customer Service Representative.

  - Subtle Formatting Errors: There were two minor spacing issues in the body. While small, they stood out in an otherwise clean email—something often missed in scam templates.

  - Generic Multi-Role Offer: I was offered a choice between Financial Analyst, IT Specialist, and Customer Service—without ever applying. Legitimate recruiters rarely offer multiple roles without a prior application or interview.

These factors combined—especially the overly generous pay and the generic job options—led me to dig deeper into the headers and domain info, confirming this was likely a phishing attempt.

<img width="918" alt="Screen Shot 2025-04-23 at 2 34 35 PM" src="https://github.com/user-attachments/assets/ec954fbe-c0d0-41ae-bc97-1b754bff9540" />
<img width="914" alt="Screen Shot 2025-04-23 at 2 34 58 PM" src="https://github.com/user-attachments/assets/862c5316-f908-4622-bca6-fa400260e9a2" />
<img width="912" alt="Screen Shot 2025-04-23 at 2 35 17 PM" src="https://github.com/user-attachments/assets/52423d67-929b-4521-89ee-bf4afa98a7fa" />
<img width="912" alt="Screen Shot 2025-04-23 at 2 35 34 PM" src="https://github.com/user-attachments/assets/d05ceef7-69fa-4d3b-93f0-81c9cc332a1b" />
<img width="906" alt="Screen Shot 2025-04-24 at 8 38 55 AM" src="https://github.com/user-attachments/assets/83440873-97c9-4955-b566-267380577834" />

#

2. While analyzing the raw header of a suspicious email, I noticed that it passed DKIM, SPF, and DMARC—which usually indicates authenticity. However, digging deeper revealed inconsistencies:

  - Originating IP Address traced back to France, but the domain was registered in Iceland, and very recently—in 2025. A domain that new raises immediate suspicion unless it’s a clearly verifiable new company.

  - The choice of Iceland for domain registration could suggest the attacker is leveraging a region with lax enforcement or anonymity-friendly policies.

This mismatch between the IP and domain geography suggests a few possibilities:

  - The attacker may be using a VPN, proxy, or relay server to spoof location.

This kind of behavior aligns with evasive phishing tactics designed to bypass basic geo-based filters and header validation checks.

<img width="922" alt="Screen Shot 2025-04-23 at 2 39 32 PM" src="https://github.com/user-attachments/assets/6a9e8187-a927-4a78-b667-b60927254eb8" />
<img width="1162" alt="Screen Shot 2025-04-23 at 2 41 33 PM" src="https://github.com/user-attachments/assets/3e518db1-9e5e-4a7c-972f-ae882e7f3758" />
<img width="1430" alt="Screen Shot 2025-04-23 at 2 42 06 PM" src="https://github.com/user-attachments/assets/895a91bf-c550-4d72-b768-5ad920d7bd1e" />
<img width="974" alt="Screen Shot 2025-04-23 at 2 42 19 PM" src="https://github.com/user-attachments/assets/6f5d4154-76b4-41a8-9e2d-a9e5f3fd559e" />
<img width="975" alt="Screen Shot 2025-04-23 at 2 42 35 PM" src="https://github.com/user-attachments/assets/c40baef5-e713-4b4c-9544-43e180e42092" />

#

3. After confirming this was a phishing attempt designed to extract sensitive personal information, I decided to dig deeper into the identity of the supposed sender, “William Rosen,” and the legitimacy of the company, Recursive Finance.

A series of Google searches turned up no trace of Recursive Finance—no official website, business listing, or social media presence. Even LinkedIn had no relevant matches. The closest I found was a “Will Rosenbaum,” an assistant professor, not an HR manager.

<img width="1024" alt="Screen Shot 2025-04-23 at 2 43 54 PM" src="https://github.com/user-attachments/assets/2c45ffdc-5b8b-4b48-8c59-83f3f56e3fbd" />
<img width="1050" alt="Screen Shot 2025-04-23 at 2 44 31 PM" src="https://github.com/user-attachments/assets/c21621bf-f620-4eb1-84b3-e3b4b435ee84" />
<img width="1050" alt="Screen Shot 2025-04-23 at 2 44 53 PM" src="https://github.com/user-attachments/assets/f2fc6236-0cf0-491e-af9f-89a6cd31e4d1" />

#

4. I also cross-referenced the address listed in the email. Instead of a commercial business location, it mapped to a residential home, which would be highly unusual for any legitimate financial firm.

These red flags further confirmed that the email was part of a well-disguised phishing campaign, using fake corporate identities and social engineering tactics to appear trustworthy.

<img width="909" alt="Screen Shot 2025-04-23 at 2 35 53 PM" src="https://github.com/user-attachments/assets/d7c09807-5520-42d4-8913-7b1f964ebfaf" />
<img width="1027" alt="Screen Shot 2025-04-23 at 2 45 19 PM" src="https://github.com/user-attachments/assets/bcc958f6-4644-4322-81fb-b34a90e9b175" />


