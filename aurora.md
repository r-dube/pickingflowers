# Large scale intrusion into U.S. corporations
In 2009, Chinese government hackers already had a large-scale cyber-espionage operation underway in multiple countries with targets such as the Tibetan government in exile \[W1\]. 
However, penetrating U.S. intelligence operations was likely proving harder.
As an alternative, the Chinese hackers penetrated multiple private (non-state) U.S. corporations to aid their espionage and counter-espionage efforts.
Along the way, they also stole intellectual property from these corporations. 
These near-simultaneous intrusions into U.S. corporations came to be known as Operation Aurora \[W2\].

## Chinese counter-espionage via Google
Chinese spies in the U.S. sometimes use Gmail.
U.S. intelligence services track these Chinese spies and, in some cases, have gotten court orders to access the spies' information at Google.

Google had built an internal portal to service court-ordered requests for information on the (alleged) spy accounts.
The Chinese government wanted to know which Gmail accounts were under surveillance - so that the government could figure out which of its spies had been discovered \[CNN1\].

Obviously, such information could be gotten by breaking into the U.S. intelligence services.
However, at the time, it was easier to break into a company such as Google to obtain this information.

The Chinese attackers orchestrated their break into Google by first identifying and then breaking into the accounts of Chinese nationals who communicated with Google China's employees.
That is, the attackers first broke into the lightly defended accounts of Google China's employees' friends and family \[FT1\], \[NP1\].

The attackers had prepared a Windows exploit that used an as yet unknown vulnerability (zero-day) in Microsoft's Internet Explorer \[WI3\].
This exploit would download spyware onto a user's computer if the user clicked a malicious link using Internet Explorer.
The Chinese attackers used the compromised friends and family accounts to send the malicious link inside phishing messages to Google China's employees.

Employees who clicked on the malicious links using their work computers had their computers compromised with malware that gave the attackers remote access.
The attackers used these computers to access the rest of Google's network.
In particular, the Chinese attackers accessed the Google internal portal to identify the Chinese spies on U.S. intelligence agencies' radar \[CNN1\], \[DR1\].

## Surveilling Chinese dissidents and human rights activists
Many Chinese dissidents and minority ethnic group human rights activists use Google services such as Gmail.
To access some of these services from China, one must first use a virtual private network (VPN) to get around Chinese censorship and surveillance.
The accounts of these dissidents and activists could also be accessed using Google's internal portal.

As part of Operation Aurora, the Chinese attackers accessed the accounts of several dissidents and activists.
One of these dissidents was Ai Weiwei - a well-known artist living in China - who maintained two Gmail accounts \[W3\], \[FT2\].

The information gathered from Ai's account was subsequently used to harass him with tax violations.
In November 2010, Ai was placed under house arrest. 
Then in 2011, Ai was jailed, and his passport seized. 
Worn down by the Chinese government, Ai left China in 2015 - a result that the Chinese government wanted as it would be far more difficult for Ai to challenge the government from outside China \[W3\].

## Stealing source code
At the time of the Aurora attacks, most companies that developed software configured their source control management (SCM) systems for ease of use.
Typically, there was no extra security protecting the SCM system, and often source code was transmitted un-encrypted between the developers' computer and the SCM system.
Google was one of these companies \[ML1\], \[ML2\], \[DS1\].

The Chinese attackers stole Google's source code.
However, Google has not disclosed how much source code was stolen and the affected products \[WI1\], \[WI2\].

The attackers could use the source code in at least three ways.
First, they could examine the source code to aid future attacks on Google or Google's users.
Second, they could inject their own code into Google's to create a vulnerability in Google's services that would not otherwise exist.
Third, they could share the source code with Google's Chinese competitors, such as Baidu.
Note that Baidu has collaborated with the Chinese government on attacks on companies such as Github.
Further, the Chinese government is also known to routinely share trade secrets and foreign intellectual property with Chinese corporations \[CNA1\], \[NP1\], \[DS1\].

## Infiltrating Adobe
Adobe was also infiltrated by the Chinese attackers at roughly the same time as Google and using similar techniques - the attackers compromised friends and family of Adobe employees, sent them a malicious link that, when clicked, installed malware on the employees' computers.
The malware gave the attackers remote access to the compromised machines \[WI3\].

Similar to Google, the attackers obtained access to Adobe's source code. 

## Stealing source code from other U.S. corporations
Besides Google and Adobe, the Chinese attackers infiltrated 32 other U.S. corporations and stole source code.
Not all the corporations that have been breached have been identified.
However, we know that the breached corporations include Intel, Juniper Networks, Akamai, Rackspace, Northrop Grumman, Dow Chemical and Morgan Stanley \[WP1\], \[NP1\], \[W2\], \[RB1\], \[DR3\].

In some cases, the zero-day in Internet Explorer was used to compromise a user's computer. 
In other cases, another zero-day in Adobe's pdf reader was used in the attack - employees were sent a malicious pdf attachment that once opened would download the remote access malware onto the computer \[CA1\].

It appears that in all the breached corporations, the SCM system was accessed and source code stolen.

## Connections to China
After jumping through several intermediary hops in multiple countries, security researchers traced Operation Aurora to two colleges in China: Shanghai Jiao Tong University and Lanxiang Vocational School.
It is possible that the college networks were being used by the Chinese hackers to hide their exact locations inside China.
Further, encryption algorithms used in a portion of the malware were found to have been developed in China and almost exclusively used in China.
Finally, the Google attack was tracked in real-time by Google's IT staff and commercial security companies.
Attack activity was most prolific during work hours in China \[NP1\], \[DR3\], \[TG1\].

In 2012, three years after Operation Aurora, the Chinese attackers were conducting similar infiltrations at other corporations worldwide \[DR1\].

## References and notes
\[W1\]: Ghostnet. Wikipedia. (Retrieved) September 15, 2021.

\[W2\]: Operation Aurora. Wikipedia. (Retrieved) October 11, 2021.

\[W3\]: Ai Weiwei. Wikipedia. (Retrieved) October 11, 2021.

\[ML1\]: Operation Aurora, Part 1: Season 3, Episode 55. Malicious Life. September 12, 2019.

\[ML2\]: Operation Aurora, Part 2: Season 3, Episode 56. Malicious Life. September 26, 2019.

\[FT1\]: Hackers target friends of Google workers. Joseph Menn. The Financial Times. January 25, 2010.

\[FT2\]: The Chinese dissident's "unknown visitors." Jamil Anderlini. The Financial Times. January 14, 2010.

\[TG1\]: Google attacks "traced to Chinese schools." Bobbie Johnson and Tania Branigan. The Guardian. February 19, 2010.

\[WI1\]: Google Hackers Targeted Source Code of More Than 30 Companies. Kim Zetter. Wired. January 13, 2010.

\[WI2\]: Google Hack Attack Was Ultra Sophisticated, New Details Show. Kim Zetter. Wired. January 14, 2010.

\[WI3\]: Hack of Google, Adobe Conducted Through Zero-Day IE Flaw. Kim Zetter. Wired. January 14, 2010.

\[CA1\]: In-depth Analysis of Hydraq. Zarestel Ferrer and Methusela Cebrian Ferrer. CA Internet Security Intelligence. 2010.

\[DR1\]: Google Aurora Attackers Still On Loose, Symantec Says. Mathew Schwartz. Dark Reading. September 7, 2012.

\[DR2\]: Google Aurora Hack Was Chinese Counterespionage Operation. Mathew Schwartz. Dark Reading. May 21, 2013.

\[DR3\]: 9 Years After: From Operation Aurora to Zero Trust. Andy Ellis. Dark Reading. February 20, 2019.

\[CNN1\]: U.S. enables Chinese hacking of Google. Bruce Schneier. CNN. January 23, 2010.

\[WP1\]: Google China cyberattack part of vast espionage campaign, experts say. Ariana Cha and Ellen Nakashima. The Washington Post. January 14, 2010.

\[RB1\]: Rackspace Response to Cyber Attacks. Fran Stephenson. The Official Rackspace Blog. January 13, 2010.

\[DS1\]: The Perfect Weapon. David Sanger. Broadway Books. 2019.

\[NP1\]: This Is How They Tell Me The World Ends. Nicole Perlroth. Bloomsbury. 2021.

\[CNA1\]: How China Acquires Foreign Technology. CNA. November 11, 2020.