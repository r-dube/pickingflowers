# Infiltrating the Tibetan Diaspora
After the Chinese invasion of Tibet in the 1950s, many Tibetans left Tibet for a life of exile in India and other countries. 
Ever since, fearing that the Tibetans would someday muster enough of an organization to demand their country back, China has infiltrated Tibetan organizations. 
Since the 2000s, this infiltration has extended online.
An analysis of China's efforts shows that China's infiltration of Tibetan organizations, both online and in-person, is well resourced, persistent, and agile.
In contrast, and for obvious reasons, Tibetan countermeasures are incomplete and unable to fend off the Chinese.

## Cyber attacks against Tibetans
That China monitors communications into and out of Tibet is well known.
After all, all current communication into Tibet transits through infrastructure controlled by the Chinese.
However, multiple studies from non-profits and commercial information security companies show China's stifling presence in the online lives of Tibetan organizations and activists outside of China.

### Tibetan communication transcripts
\[TCL0\] documents China's logging and monitoring of Skype messages in and out of China and territories currently under Chinese control, such as Tibet.
This infrastructure was likely used to arrest a Tibetan woman (circa 2008) who worked in Dharmasala (India) and was returning to her Tibet village.
The woman was confronted by Chinese officials at Tibet's Nepal border with transcripts of her communication while she was away in Dharmasala.
The Chinese officials claimed that that the transcripts demonstrated that the woman was politically active - sufficient for an arrest in Chinese-controlled Tibet \[TCL1\], \[O8\], \[O9\].

Given China's extensive infiltration of Tibetans, it is possible that the transcripts came from a direct compromise of the woman's computer or cell phone (as we will see below \[O9\]).
Recorded incidents of electronic compromise of Tibetan nationals outside of Tibet by China go at least as far back as 2007 \[SANS1\].

### Social engineering and email attachments with malware
Chinese attackers use their knowledge of Tibetan's activities to construct lures for Tibetans.
These lures are used to install malware (spyware) on Tibetan users' computers and cell phones and to harass them.

In 2007, the Chinese attackers created cognitive dissonance to get Tibetan to click on malware-laced attachments.
The attackers constructed email messages and matching document attachments attributed to well-known Tibetan personalities.
However, the messages and documents contradicted the reader's prior belief about the well-known personality's views.
The result was that the reader clicked on the attachment out of curiosity, allowing the attacker into their computer \[SANS1\].

In 2012, Chinese attackers booby-trapped genuine posts and articles on self-immolations among Tibetans as the vehicle to deliver malware to Tibetan readers \[TCL2\].
In the same year, the attackers also booby-trapped articles on the European parliament's concern for human rights in Tibet to deliver malware to a targetted list of Tibetan activists \[TCL3\].
Later in 2012, Chinese attackers used authentic privately-held messages of some Tibetans as the lure to send malware to other Tibetans \[TCL4\].
In all these cases, the attackers' goal was to get a Tibetan of interest to click on a doctored document that silently dropped malware on the users' computer.

These social engineering attacks demonstrate that by 2012, the Chinese had deeply penetrated communications between prominent Tibetans living outside Tibet.
These attacks also demonstrate that the attackers were paying close attention to news articles and forum messages relevant to the Tibetan diaspora.
The depth of penetration and up-to-date information on issues of interest to Tibetans enabled the Chinese attackers to construct credible lures to ensnare additional Tibetans \[AV1\], \[AV2\],  \[AV3\], \[AV4\], \[K1\], \[TCL7\], \[TCL8\], \[TCL9\].

The Chinese attackers continues to use social engineering and attachments containing malware to infilitrate Tibetans \[C1\], \[TSL2\], \[PAN1\], \[TSL1\].

### Cloud credential phishing and drive-by-downloads 
Eventually, word of malicious attachments in emails spread among the Tibetan community.
Instead of passing documents around, Tibetan groups started storing documents in the public cloud (for example, on Google Drive).
The Chinese attackers noticed the change in Tibetans' behavior. They shifted to using cloud credential phishing (for example, by putting up a fake login page and asking the user to enter their credentials) and drive-by-downloads (for example, by compromising websites frequented by Tibetans and downloading malware to the users' computer during the visit) \[K3\], \[TCL10\], \[TCL11\].

In one such attack, the Chinese attackers compromised the website of the Tibetan government in exile (called the Central Tibetan Authority or CTA).
Chinese-speaking visitors to the website had a backdoor dropped onto their computer.
Once the backdoor was successfully installed, the attackers accessed the computer \[K3\].

In another case, a Tibetan activist received an email purporting to be from a division of the CTA.
The message included several links to attachments that the sender claimed were approved by the Tibetan parliament.
Clicking on the link opened a fake Google login page.
Once credentials were entered, a decoy file (otherwise genuine) was shown to trick the user into believing that nothing terrible had happened.
Meanwhile, the credentials entered by the user were shipped back to a Chinese command-and-control server \[TCL11\].

These new (for the Tibetan community) attacks continue to be used in parallel with older generation email attachment-based attacks.

### Cell phone malware
Smart cell (mobile) phones are now ubiquitous.
Similar to the general population, the Tibetan diaspora has also adopted cell phones for their communication needs.
Noticing the change in their targets' communication habits, Chinese attackers created and used cell phone-specific malware to maintain their infiltration of the Tibetan community \[TCL6\], \[TCL12\], \[K2\].

In one 2018 incident, a Tibetan activist received a WhatsApp message from a Chinese attacker claiming to be an Amnesty Internal employee.
The attacker engaged the activist in a conversation regarding a recent protest self-immolation incident in Tibet.
Subsequently, the attacker sent the activist obfuscated links that, if clicked, would download malware onto the activist's cell phone \[TCL12\].

Chinese attackers target Tibetans with both Apple iOS and Android malware \[TCL12\].

### Cloud credential phishing with OAuth
Cloud credential phishing attempts (say for Gmail login ids and passwords) can be effectively thwarted using two-factor authentication.
Unfortunately, two-factor authentication has only modest penetration in the Tibetan community (similar to the general population).
However, some Tibetan activists do use it.

Chinese attackers get around the use of a second factor for authentication by tricking users into giving malicious cloud applications permissions to access their Gmail account or other data stored in the cloud.
In one documented case, a Chinese attacker attempted to get a Tibetan activist to click on a link sent to a Tibetan activist via WhatsApp. 
Had the link been clicked and the prompts on the subsequent screens followed, a malicious cloud-based application would have been given OAuth permissions (effectively delegated access) to the activist's Gmail account \[TCL12\].

### Exfiltration and maintaining persistence
The various intrusions described above aim to exfiltrate data from the device/computer (emails, documents, contact lists) and maintain persistence on the breached device/computer to enable future exfiltration.

In the cases where malware is installed on a computer or cell-phone, the malware typically connects back to a command-and-control server under the control of the Chinese attackers. 
Periodically, the command-and-control server instructs the malware to send back new data.
Persistence is typically maintained by starting up the malware every time the computer is rebooted.
Such persistence is more challenging for the attacker to engineer for cell phones (particularly those running iOS).
Even so, once the malware is deployed on the phone, it typically has access to historical information such as call logs and email threads that serve the attackers' purpose, even if the malware disappears at the next phone reboot.

In the cases where credentials to a cloud resource are phished, the attacker maintains access without being discovered as long as the user does not change the account password (in the case of stolen IDs/passwords) or remove delegated access (in the case of third-party applications).
Suppose the user does change the password or remove delegated access to a malicious third-party application. In that case, the attackers have to compromise the user repeatedly (assuming that they remain interested in the user).

### Malware development and reuse 
Malware developed by Chinese attackers shows clear signs of continuous development: the malware improves in sophistication and its ability to evade security tools over time \[TCL5\].

The malware is also reused. 
Evidence shows that malware deployed against Tibetans is also used against the Uighur community and in corporate espionage carried out by the Chinese military \[TCL5\], \[TCL12\].

Finally, the Chinese attackers have malware families for multiple platforms: Microsoft Windows, Apple MacOS, Apple iOS, Android and cloud services such as Gmail \[FEYE1\], \[BB1\], \[V1\], \[TM1\], \[ZD1\], \[PP1\], \[PP12\], \[TCL12\].

Taken together, the depth and breadth of the endeavor point to a well-resourced organization tasked with a time invariant goal of infiltrating Tibetan (and other) organizations and maintaining that infiltration.

## Gathering human intelligence on Tibetans
China supplements its electronic surveillance of the Tibetan community with human intelligence.
Such intelligence is gathered by using lures (such as money) or blackmail (the well-being of the extended family in Tibet) to turn some Tibetans into spies against their community.

### In Sweden
One such Tibetan was Dorjee Gyantsan, who spied for China between 2015 and 2017.
Dorjee, who lived in Sweden, was paid $6,000 by a Chinese intelligence officer in Poland to provide the Chinese government with information about the families, housing situations, and travel plans of members of the Tibetan community in exile in Sweden.
Subsequently, the Chinese government used the information to harass relatives of the exiles still living in Chinese-controlled Tibet \[O4\], \[O5\], \[O6\].

Dorjee was caught, prosecuted, sentenced to prison in Sweden, and on his release, deported from Sweden \[O7\].

### In the U.S.
Baimadajie Angwang was another Tibetan who spied for China.
Baimadajie was a New York City policeman of Tibetan origin.
He was also a former member of the U.S. Marine Corp \[O1\], \[O2\].

In 2018, Baimadajie was recruited by Chinese officials working out of the Chinese consulate in New York.
Subsequently, he met with his New York consulate-based handlers multiple times.
He was arrested in 2020, and his criminal case is pending in the courts as of this writing.

The type of information that Baimadajie gathered for the Chinese government is not known yet.
Baimadajie was likely blackmailed to spy against other Tibetans \[O3\].


## Conclusion
From the analysis above, it is clear that the Chinese attackers have succeeded in deeply infiltrating the Tibetan diaspora and maintaining that infiltration.
Simultaneously, the Chinese government augments what it learns about Tibetans by electronic means with human intelligence gathered using money as a lure or blackmail.

The Tibetan diaspora is severely under-resourced and does not have the human capital (their numbers outside of India and Tibet are small) or the financial means to prevent the Chinese government from eavesdropping or disrupting their communications.
The gap in capability between the Chinese offense and Tibetan defense is depressingly large.

## References and notes

### University of Toronto
\[TCL0\]: BREACHING TRUST: An analysis of surveillance and security practices on China's TOM-Skype platform. Information Warfare Monitor. October 1, 2008.

\[TCL1\]: Tracking GhostNet: Investigating a Cyber Espionage Network. Information Warfare Monitor. March 29, 2009.

\[TCL1a]: Shadows in the Cloud: Investigating Cyber Espionage 2.0. Information Warfare Monitor. April 6, 2010.

\[TCL2\]: Information Operations and Tibetan Rights in the Wake of Self-Immolations. The Citizen Lab. March 9, 2012,

\[TCL3\]: Spoofing the European Parliament. The Citizen Lab. June 20, 2012.

\[TCL4\]: Recent Observations in Tibet-related Information Operations: Advanced Social
Engineering for the Distribution of LURK Malware. The Citizen Lab. July 26, 2012

\[TCL5\]: APT1's GLASSES—Watching a Human Rights Organization. The Citizen Lab. February 25, 2013.

\[TCL6\]: Permission to Spy: An Analysis of Android Malware Targeting Tibetans. The Citizen Lab. April 18, 2013.

\[TCL7\]: Surtr: Malware Family Targeting the Tibetan Community. The Citizen Lab. August 2, 2013.

\[TCL8]: Communities @ Risk: Targeted Digital Threats Against Civil Society. The Citizen Lab. November 11, 2014.

\[TCL9\]: Targeted Threat Index: Characterizing and Quantifying Politically-Motivated Targeted Malware. 23rd USENIX Security Symposium. August 2014

\[TCL10\]: Shifting Tactics: Tracking changes in years-long espionage campaign against Tibetans. The Citizen Lab. March 10, 2016

\[TCL11\]: Spying on a Budget: Inside a Phishing Operation with Targets in the Tibetan Community. The Citizen Lab. January 30, 2018.

\[TCL12\]: Missing Link: Tibetan Groups Targeted with 1-Click Mobile Exploits. The Citizen Lab. September 24, 2019.

### AT&T / Alien Vault
\[AV1\]: Targeted Attacks Against Tibetan Organizations. Alien Vault. March 13, 2012.

\[AV2\]: AlienVault Tibet Related Research Now Used to Target Tibetan NonGovernmental Organizations. Alien Vault. March 19, 2012.

\[AV3\]: CVE-2012-0158, Tibet, Targeted Attacks, and so on. Alien Vault. April 18,
2012.

\[AV4\]: Latest Adobe PDF Exploit Used to Target Uyghur and Tibetan Activists. Alien Vault. March 14, 2013.

### Kaspersky
\[K1\]: A Gift for Dalai Lama's Birthday. Kaspersky Lab Securelist. July 4, 2012.

\[K2\]: Android Trojan Found in Targeted Attack. Kaspersky Lab Securelist. March 26, 2013.

\[K3\]: Central Tibetan Administration Website Compromised. Kaspersky Lab Securelist. August 12, 2013.

### FireEye / Mandiant
\[FEYE1\]: New Targeted Attack on Taiwanese Government & Tibetan Activists Open up
a Can of Warms - GrayPigeon, Hangame & Shiqiang Gang. FireEye. April 18, 2013

### Palo Alto Networks
\[PAN1\]: Scarlet Mimic: Years-Long Espionage Campaign Targets Minority Activists. Palo Alto Networks Unit 42. January 24, 2016.

### SANS
\[SANS1\]: Overview of cyberattacks against Tibetan communities. The SANS Institute. March 24, 2008.

### Blackberry / Cylance
\[BB1\]: Puttering into the Future. Blackberry Threat Vector Blog. January 12, 2016.

### Volexity
\[V1\]: Storm Cloud Unleashed: Tibetan Focus of Highly Targeted Fake Flash Campaign. Volexity Threat Research. March 31, 2020.

### Trend Micro
\[TM1\]: Trends in Targeted Attacks. Trend Micro. 2011.

### Cisco 
\[C1\]: ExileRAT shares C2 with LuckyCat, targets Tibet. Cisco Talos. February 4, 2019.

### The Security Ledger
\[TSL1\]: Targeted Attacks Follow Tibetans To The Cloud. The Security Ledger. March 10, 2016.

\[TSL2\]: ExileRAT Malware Targets Tibetan Exile Government. The Security Ledger. February 6, 2019.

### ZDNet
\[ZD1\]: Chinese cyberspies targeted Tibetans with a malicious Firefox add-on. ZDNet. February 25, 2021.

### Proofpoint
\[PP1\]: Chinese APT TA413 Resumes Targeting of Tibet Following COVID-19 Themed Economic Espionage Campaign Delivering Sepulcher Malware Targeting Europe. Proofpoint. September 1, 2020.

\[PP2\]: TA413 Leverages New FriarFox Browser Extension to Target the Gmail Accounts of Global Tibetan Organizations. Proofpoint. February 25, 2021.

### Other
\[O1\]: How did an NYPD officer from Tibet end up accused of spying for China? Amanda Holpuch. The Guardian. September 29, 2020.

\[O2\]: Judge Halts Release of NYPD Officer Accused of Spying for China. NBC New York. October 2, 2020.

\[O3\]: Counter-espionage regulations force Tibetans to spy on Tibetans. International Campaign for Tibet. March 15, 2021.

\[O4\]: Sweden Charges Tibetan Resident With Spying on Exile Community For China. Radio Free Asia. April 12, 2018.

\[O5\]: Tibetan Charged in Sweden Denies Spying For China. Radio Free Asia. April 18, 2018.

\[O6\]: Tibetan Man Convicted in Sweden of Spying For China. Radio Free Asia. June 15, 2018.

\[O7\]: Sweden to deport Chinese agent arrested for spying on Tibetans. Phayul. October 28, 2020.

\[O8\]: Meet the Canadians who busted GhostNet. The Globe and Mail. March 30, 2009.

\[O9\]: Ghostnet. Wikipedia. (Retrieved) September 15, 2021.