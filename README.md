## Phishing Email Campaign Investigations

#### This repository will hold all of my write-ups on investigating Phishing emails that contain malicious links or attachments.
    - Incident reports will be linked in their respective .md files.

#### Phishing attacks have been prevalent since the mid 1990's, and their attack vectors have only evolved and improved over time. For example, Vishing (Voice Phishing) and Smishing (SMS Phishing) has gained popularity in recent years, utilizing phone calls, texts, links, or voice messages to trick individuals into sharing sensitive information, often with the integration of AI. Phishing emails rely on social engineering and capitalize on human error to seek sensitive information or some form of monetary gain. Here are the most common signs to look for:
    - Domain: The email may use a different domain than the legitimate business. 
    - Links: The email may include links that don't match the domain. 
    - Attachments: The email may include unsolicited attachments. 
    - Spelling and grammar: The email may contain obvious spelling or grammatical errors. 
    - Sender: The email may be from a first-time sender, an infrequent sender, or a sender marked as "External".
#

#### NOTE: Before these investigations, I created a home lab and downloaded VMware Workstation Pro as my primary virtual machine and Kali Linux as the disk image, so I can access the malicious emails -through the VM- safely.
#
#### Programs we will be using: 
- VMware Workstation Pro: https://www.broadcom.com/
  - You must create an account
  - Click the drop down menu in the upper right corner and select "VMware Cloud Foundation"
  - Search for VMware Workstation Pro
  - Download for personal use on Windows or Linux
- Kali Linux: https://www.kali.org/get-kali/#kali-virtual-machines
  - For Microsoft Windows: After installing, add the Kali Linux downloaded file as an exclusion in Windows Security > Virus & Threat Protection > Manage Settings > Add or Remove Exclusions > Add Kali Linux.
  - Extract all the files, and it can now be used on VMware as your disk image
