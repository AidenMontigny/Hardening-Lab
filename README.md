<h1> Hardening Lab </h1>

<h2>Description</h2>
The Hardening Lab project focuses on securing a Kali Linux VM and a Windows environment through various hardening techniques. The project demonstrates the process of updating, configuring, and securing systems against potential vulnerabilities. Key steps include running system updates using ‘apt update’ and ‘apt full-upgrade’, performing a Lynis security scan, and implementing Bitlocker drive encryption on Windows to ensure data confidentiality. The project also involves configuring Windows Firewall to restrict incoming traffic, disabling unnecessary services such as NetBIOS and Print Spooler, and enforcing strong password policies by disabling LAN Manager hashes. Additional security measures include the installation of ClamWin Antivirus for malware protection and the removal of unused features. This exercise highlights the importance of system hardening in enhancing security and preventing potential attacks.
<br />

<h2>Languages and Utilities Used</h2>

- <b> Bash (Linux Shell) </b>
- <b> PowerShell </b>
- <b> Lynis </b>
- <b> BitLocker </b>
- <b> Windows Firewall </b>
- <b> ClamWin Antivirus </b>
- <b> NetBIOS </b>
- <b> Print Spooler </b>
- <b> Windows Defender </b>
- <b> XPS Viewer </b>

<h2>Environments Used </h2>

- <b> Kali Linux </b>
- <b> Windows 10 </b>

<h2>Project walk-through:</h2>
<p align="left">
TEXT. <br/><br/>
  <img src="Screenshot 2025-04-19 144313.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>


<h2>Write Up</h2>

<p><u> Performing Backups and Restoring Data </u></p>
<p>ClamWin is a free and open-source antivirus program designed primarily for Microsoft Windows. It uses the ClamAV engine and provides users with basic malware protection against a wide array of threats (KilObit, 2022). ClamWin has a more user-friendly interface, which helps users plan their scans and specify what they want. While it may offer a cost-effective solution for organizations, it does come with limitations. The absence of advanced features such as real-time protection, web filtering, and email scanning can leave vulnerabilities undetected, especially if they rely solely on ClamWin. Furthermore, the software's effectiveness largely depends on users proactively engaging with it, which can lead to gaps in security if not monitored closely. The biggest con, however, is that scanning large file systems will consume significant time and affect user productivity. </p>
<p>To effectively formulate and deploy business information systems solutions, an analysis is crucial. This process begins with identifying all personnel utilizing the system to gather diverse perspectives on needs. Conducting interviews, surveys, and workshops helps capture both functional and non-functional requirements, ensuring the system aligns with user expectations and business objectives. The information is compiled into a detailed requirements document, which serves as a reference throughout the development process. Additionally, performing a study assesses the technical and financial viability of the proposed solution, ensuring the organization's infrastructure can support it. By rigorously applying requirements analysis, organizations can deploy information systems that not only enhance operational efficiency but also bolster security measures, thereby mitigating risks effectively. Overall, creating a plan that will meet all employees' needs is crucial as it will ensure that everyone's jobs can be completed as needed.
 </p>

<p><u> References </u></p>
<p> kilObit. (2022, December 9). Open Source Free Antivirus - ClamAV. Bing. https://www.bing.com/videos/riverview/relatedvideo?q=clamav+1029+windows+kilobit&mid=2303C7C6F3C0EE4A43D22303C7C6F3C0EE4A43D2&ajaxhist=0 </p>
