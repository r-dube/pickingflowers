# Infiltrating the Tibetan Diaspora
After the Chinese invasion of Tibet in the 1950s, may Tibetans left Tibet for a life of exile in India and other countries. 
Ever since, fearing that the Tibetans would someday muster enough of an organization to demand their country back, China has infiltrated Tibetan organizations. 
Since the 2000s this infiltration has extended online.
An analysis of China's efforts shows that China's infiltration of Tibetan organizations, both online and in-person, is well resourced, persistent and agile.
In contrast, and for obvious reasons, Tibetan counter measures are incomplete and unable to fend-off the Chinese.

## Cyber attacks against Tibetans
That China monitors communications into and out of Tibet is well known.
After all, all current communication into Tibet transits through infrastructure contolled by the Chinese.
However, multiple studies from non-profits and commercial information security companies show China's stiffling presence in the online lives of Tibetan organizations and activists outside of China.

### Tibetan communication transcripts
\[TCL0\] documents China's logging and monitoring of Skype messages in and and out China and territories currently under Chinese control such as Tibet.
These logs were likely used to arrest a Tibetan woman (circa 2008) who worked in Dharmasala (India), and was returning to her village in Tibet.
The woman was confronted by Chinese officials at Tibet's Nepal border with transcripts of her communication during the time that she away in Dharmasala.
The Chinese officials claimed that that the transcripts demonstrated that the woman was politically active - sufficient for an arrest in Chinese controlled Tibet \[TCL1\], \[O8\], \[O9\].

Given China's extensive infiltration of Tibetans, it is possible that the transcipts referred to above came from a direct compromise of the woman's computer or cell phone (as we will see below \[O9\]).
Recorded incidents of electronic compromise of Tibetan nationals outside of Tibet by China go atleast as far back as 2007 \[SANS1\].

### Social engineering and email attachments with malware
Chinese social engineering techniques have evolved alongside newsworthy developments in the Tibetan diaspora.
In 2007, the Chinese attackers relied on creating cognitive disonance.
The attackers created email messages and matching document attachments attributed to well known Tibetan personalities.
However, the messages and documents contradicted the reader's priot belief about the well known personalites' views.
The result, in many cases, was that the reader clicked on the attachment out of curiosity, allowing the attacker into their computer \[SANS1\].

In 2012, the Chinese attackers used genuine posts and articles on protest self-immolations among Tibetans in Tibet as the vehicle to deliver malware to Tibetan readers \[TCL2\].
In the same year, the attackers used genuine articles on the European Parliament's concerns of human rights in Tibet to deliver malware to a targetted list of Tibetan activists \[TCL3\].
Later in 2012, the Chinese attackers used authentic privately-held messages of some Tibetans as the lure to send malware to other Tibetans \[TCL4\].

These social engineering attacks demonstrate that by 2012, the Chinese had deeply penetrated communications between prominent Tibetans living outside Tibet.
These attacks also demonstrate that the attackers were paying close attention to news articles and forum messages relevant to the Tibetan diaspora.
The depth of penetration and up-to-date information on issues of interest to Tibetans enabled the Chinese attackers to construct credible lures to ensnare additional Tibetans over multiple years \[AV1\], \[AV2\],  \[AV3\], \[AV4\], \[K1\], \[TCL7\], \[TCL8\], \[TCL9\].

China continues to use social engineering and attachments containing malware to infilitrate Tibetans \[C1\], \[TSL2\], \[PAN1\], \[TSL1\].

### Cloud credential phishing and drive-by-downloads 
Eventually word of malicious attachments in emails spread among the Tibetan community.
Instead passing documents around, Tibetan groups started storing documents in the public cloud (for example on Google Drive).
The Chinese attackers noticed the change in Tibetans' behavior and shifted to using cloud credential phishing (putting up a fake login page and asking the user to enter their credentials) and drive-by-downloads (compromising web-sites frequented by Tibetans and download malware to the users' computer when they visit these web-sites) \[K3\], \[TCL10\], \[TCL11\].

In one such attack, the Chinese attackers compromised the website of the Tibetian government in exile (called the Central Tibetan Authority or CTA).
Chinese speaking visitors to the website had a backdoor dropped onto their computer.
Once the backdoor is successfully installed, the attackers have access to the computer \[K3\].

In another case, a Tibetan activist received an email purporting to be from a division of the CTA.
The message include several links to attachments that the sender claimed were approved by the Tibetan paliament.
Clicking on the link opened a fake Google login page.
Once credentials were entered, a decoy file (that was otherwise genuine) is shown to trick the user into believing that nothing bad has happened.
Meanwhile, the credentials entered by the user are shipped back to the Chinese command-and-control server \[TCL11\].

These new (for the Tibetan community) attacks continue to be used in parallel with older generation email attachment based attacks.

### Cell phone malware
Smart cell (mobile) phones are now ubiquitous.
Similar to the general population, the Tibetan diaspora has also adopted cell phone for their communication needs.
Noticing the change in their targets' communication habits, Chinese attackers hcreated and used cell phone speficic malware to maintain their infilitration of the Tibetan community \[TCL6\], \[TCL12\], \[K2\].

In one 2018 incident, a Tibetan activist received a WhatsApp message from a Chinese attacker claiming to be an Amnesty Internal employee.
The attacker engaged the activist in a conversation regarding a recent protest self-immolation incident in Tibet.
Subsequently, the attacker sent the activist obfuscated links that if clicked would download malware onto the activist's cell phone \[TCL12\].

Chinese attackers are known to target Tibetans with both Applie IOS and Android malware \[TCL12\].

### Exfiltration and maintaining persistence

### Continuous development of malware and attacks 

### Using the same infrastructure against other groups

## Gathering human intelleigence on Tibetans

### In Sweden

### In the U.S.

## Conclusion

## References and notes

### University of Toronto
\[TCL0\]: BREACHING TRUST: An analysis of surveillance and security practices on China’s TOM-Skype platform. Information Warfare Monitor. October 1, 2008.

\[TCL1\]: Tracking GhostNet: Investigating a Cyber Espionage Network. Information Warfare Monitor. March 29, 2009.

\[TCL1a]: Shadows in the Cloud: Investigating Cyber Espionage 2.0. Information Warfare Monitor. April 6, 2010.

\[TCL2\]: Information Operations and Tibetan Rights in the Wake of Self-Immolations. The Citizen Lab. March 9, 2012,

\[TCL3\]: Spoofing the European Parliament. The Citizen Lab. June 20, 2012.

\[TCL4\]: Recent Observations in Tibet-Related Information Operations: Advanced Social
Engineering for the Distribution of LURK Malware. The Citizen Lab. July 26, 2012

\[TCL5\]: APT1’s GLASSES—Watching a Human Rights Organization. The Citizen Lab. February 25, 2013.

\[TCL6\]: Permission to Spy: An Analysis of Android Malware Targeting Tibetans. The Citizen Lab. April 18, 2013.

\[TCL7\]: Surtr: Malware Family Targeting the Tibetan Community. The Citizen Lab. August 2, 2013.

\[TCL8]: Communities @ Risk: Targeted Digital Threats Against Civil Society. The Citizen Lab. November 11, 2014.

\[TCL9\]: Targeted Threat Index: Characterizing and Quantifying Politically-Motivated Targeted Malware. 23rd USENIX Security Symposium. August 2014

\[TCL10\]: Shifting Tactics: Tracking changes in years-long espionage campaign against Tibetans. The Citizen Lab. March 10, 2016

\[TCL11\]: Spying on a Budget: Inside a Phishing Operation with Targets in the Tibetan Community. The Citizen Lab. January 30, 2018.

\[TCL12\]: Missing Link: Tibetan Groups Targeted with 1-Click Mobile Exploits. The Citizen Lab. September 24, 2019.

### AT&T / Alien Vault
\[AV1\]: Targeted Attacks Against Tibetan Organizations. Alien Vault. March 13, 2012.

\[AV2\]: AlienVault Tibet Related Research Now Used to Target Tibetan NonGovernmental Organizations. Alient Vault. March 19, 2012.

\[AV3\]: CVE-2012-0158, Tibet, Targeted Attacks and so on. Alien Vault. April 18,
2012.

\[AV4\]: Latest Adobe PDF Exploit Used to Target Uyghur and Tibetan Activists. Alient Vault. March 14, 2013.

### Kaspersky
\[K1\]: A Gift for Dalai Lama’s Birthday. Kaspersky Lab Securelist. July 4, 2012.

\[K2\]: Android Trojan Found in Targeted Attack. Kaspersky Lab Securelist. March 26, 2013.

\[K3\]: Central Tibetan Administration Website Compromised. Kaspersky Lab Securelist. August 12, 2013.

### FireEye / Mandiant
\[FEYE1\]: New Targeted Attack on Taiwanese Government & Tibetan Activists Open up
a Can of Warms - GrayPigeon, Hangame & Shiqiang Gang. FireEye. April 18, 2013

### Palo Alto Networks
\[PAN1\]: Scarlet Mimic: Years-Long Espionage Campaign Targets Minority Activists. Palo Alto Networks Unit 42. January 24, 2016.

### SANS
\[SANS1\]: Overview of cyber attacks against Tibetan communities. The SANS Institute. March 24, 2008.

### Blackberry / Cylance
\[BB1\]: Puttering into the Future. Blackberry Threat Vector Blog. January 12, 2016.

### Volexity
\[V1\]: Storm Cloud Unleashed: Tibetan Focus of Highly Targeted Fake Flash Campaign. Volexity Threat Research. March 31, 2020.

### Trend Micro
\[TM1\]: Trends in Targeted Attacks. Trend Micro. 2011.

### Cisco 
\[C1\]:ExileRAT shares C2 with LuckyCat, targets Tibet. Cisco Talos. February 4, 2019.

### The Security Ledger
\[TSL1\]: Targeted Attacks Follow Tibetans To The Cloud. The Security Ledger. March 10, 2016.

\[TSL2\]: ExileRAT Malware Targets Tibetan Exile Government. The Security Ledger. February 6, 2019.

### ZDnet
\[ZD1\]: Chinese cyberspies targeted Tibetans with a malicious Firefox add-on. ZDnet. February 25, 2021.

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