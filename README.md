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

<h3> Part 1 </h3>

<p align="left">
The command apt update && apt full-upgrade -y was executed on the Kali VM to automatically update and upgrade all installed applications to their latest versions. This ensures that the system is up to date with the most recent patches and security improvements. <br/><br/>
  <img src="Screenshot 2025-04-30 164137.png" height="80%" width="80%" alt="Step 1"/>
  <br/>
</p>

<p align="left">
The successful execution of the command is confirmed, indicating that all updates and upgrades have been applied successfully. <br/><br/>
  <img src="Screenshot 2025-04-30 164151.png" height="80%" width="80%" alt="Step 2"/>
  <br/>
</p>

<p align="left">
The Lynis scan on the Kali VM revealed no vulnerabilities, indicating that the system is secure and properly configured. <br/><br/>
  <img src="Screenshot 2025-04-30 164158.png" height="80%" width="80%" alt="Step 3"/>
  <br/>
</p>

<h3> Part 2 </h3>

<p align="left">
The 'Recovery Console: Automatic Administrative Logon' prompt has been disabled to enhance system security and prevent unauthorized access during the recovery process. <br/><br/>
  <img src="Screenshot 2025-04-30 164203.png" height="80%" width="80%" alt="Step 4"/>
  <br/>
</p>

<p align="left">
The ‘Roles and Features’ Wizard shows the selection of ‘Bitlocker Drive Encryption’ for installation, ensuring the system's drive is encrypted for enhanced data protection. <br/><br/>
  <img src="Screenshot 2025-04-30 164208.png" height="80%" width="80%" alt="Step 5"/>
  <br/>
</p>

<p align="left">
Bitlocker has been successfully installed, and the option to enable it for full disk encryption is now available, providing an added layer of security for the system’s data. <br/><br/>
  <img src="Screenshot 2025-04-30 164213.png" height="80%" width="80%" alt="Step 6"/>
  <br/>
</p>

<p align="left">
The password creation process for Bitlocker is displayed, ensuring secure access to the encrypted drive and enhancing overall data protection. <br/><br/>
  <img src="Screenshot 2025-04-30 164219.png" height="80%" width="80%" alt="Step 7"/>
  <br/>
</p>

<p align="left">
The process of encrypting the VM's disk is shown, securing all data on the disk through Bitlocker encryption to protect sensitive information. <br/><br/>
  <img src="Screenshot 2025-04-30 164224.png" height="80%" width="80%" alt="Step 8"/>
  <br/>
</p>

<p align="left">
The C drive is shown to be successfully encrypted by Bitlocker, ensuring that all data on the drive is protected from unauthorized access. <br/><br/>
  <img src="Screenshot 2025-04-30 164229.png" height="80%" width="80%" alt="Step 9"/>
  <br/>
</p>

<p align="left">
Windows Firewall is enabled for all three profiles, ensuring comprehensive network protection by controlling inbound and outbound traffic across different network environments. <br/><br/>
  <img src="Screenshot 2025-04-30 164234.png" height="80%" width="80%" alt="Step 10"/>
  <br/>
</p>

<p align="left">
All incoming traffic is blocked, enhancing security by preventing unauthorized access to the system from external sources. <br/><br/>
  <img src="Screenshot 2025-04-30 164239.png" height="80%" width="80%" alt="Step 11"/>
  <br/>
</p>

<p align="left">
The listening command on all ports is displayed, providing visibility into the open ports and active network connections on the system. <br/><br/>
  <img src="Screenshot 2025-04-30 164244.png" height="80%" width="80%" alt="Step 12"/>
  <br/>
</p>

<p align="left">
The new inbound rules for specific local ports are configured, effectively restricting access to all other ports and enhancing security by limiting network traffic to authorized connections only. <br/><br/>
  <img src="Screenshot 2025-04-30 164250.png" height="80%" width="80%" alt="Step 13"/>
  <br/>
</p>

<p align="left">
The 'NetBIOS over TCP/IP' feature has been successfully disabled to reduce the attack surface and prevent unnecessary network protocols from being exposed. <br/><br/>
  <img src="Screenshot 2025-04-30 164254.png" height="80%" width="80%" alt="Step 14"/>
  <br/>
</p>

<p align="left">
This confirms that the 'NetBIOS over TCP/IP' feature was successfully disabled, ensuring enhanced network security by preventing the use of legacy protocols. <br/><br/>
  <img src="Screenshot 2025-04-30 164259.png" height="80%" width="80%" alt="Step 15"/>
  <br/>
</p>

<p align="left">
This demonstrates the verification of Windows Defender settings, ensuring that the system's antivirus protection is properly configured and operational. <br/><br/>
  <img src="Screenshot 2025-04-30 164304.png" height="80%" width="80%" alt="Step 16"/>
  <br/>
</p>

<p align="left">
This indicates that the system is free of any detected threats, ensuring that the virtual machine remains secure and protected. <br/><br/>
  <img src="Screenshot 2025-04-30 164310.png" height="80%" width="80%" alt="Step 17"/>
  <br/>
</p>

<p align="left">
This confirms that the security setting "Do not store LAN Manager hash value on next password change" has been enabled, enhancing password security by preventing the storage of outdated and less secure hash values. <br/><br/>
  <img src="Screenshot 2025-04-30 164315.png" height="80%" width="80%" alt="Step 18"/>
  <br/>
</p>

<p align="left">
This demonstrates that the "Lan Manager" authentication protocol has been successfully upgraded to "NTLMv2" and that "LM" and "NTLM" protocols have been disabled, thereby strengthening security by enforcing more secure authentication methods. <br/><br/>
  <img src="Screenshot 2025-04-30 164321.png" height="80%" width="80%" alt="Step 19"/>
  <br/>
</p>

<p align="left">
This indicates that the "File and Print Sharing" feature has been removed from the network settings, reducing potential attack vectors by disabling unnecessary services. <br/><br/>
  <img src="Screenshot 2025-04-30 164325.png" height="80%" width="80%" alt="Step 20"/>
  <br/>
</p>

<p align="left">
This demonstrates the disabling of an unnecessary service, specifically the 'Print Spooler,' which is not required for the system’s operations and helps minimize the potential attack surface by removing unused services. <br/><br/>
  <img src="Screenshot 2025-04-30 164330.png" height="80%" width="80%" alt="Step 21"/>
  <br/>
</p>

<p align="left">
This shows the removal of the 'XPS Viewer,' a feature that is not necessary for the system, further enhancing the security posture by eliminating unused software. <br/><br/>
  <img src="Screenshot 2025-04-30 164335.png" height="80%" width="80%" alt="Step 22"/>
  <br/>
</p>

<p align="left">
This demonstrates the successful removal of an unnecessary feature, contributing to the optimization and security of the system by eliminating non-essential components. <br/><br/>
  <img src="Screenshot 2025-04-30 164339.png" height="80%" width="80%" alt="Step 23"/>
  <br/>
</p>

<p align="left">
This indicates the successful download of ClamWIN, a free and open-source antivirus tool, to enhance the system's security measures. <br/><br/>
  <img src="Screenshot 2025-04-30 164344.png" height="80%" width="80%" alt="Step 24"/>
  <br/>
</p>

<p align="left">
This  <br/><br/>
  <img src="Screenshot 2025-04-30 164.png" height="80%" width="80%" alt="Step 24"/>
  <br/>
</p>

<p align="left">
This  <br/><br/>
  <img src="Screenshot 2025-04-30 164.png" height="80%" width="80%" alt="Step 24"/>
  <br/>
</p>

<p align="left">
This  <br/><br/>
  <img src="Screenshot 2025-04-30 164.png" height="80%" width="80%" alt="Step 24"/>
  <br/>
</p>

<h2>Write Up</h2>

<p><u> Performing Backups and Restoring Data </u></p>
<p>ClamWin is a free and open-source antivirus program designed primarily for Microsoft Windows. It uses the ClamAV engine and provides users with basic malware protection against a wide array of threats (KilObit, 2022). ClamWin has a more user-friendly interface, which helps users plan their scans and specify what they want. While it may offer a cost-effective solution for organizations, it does come with limitations. The absence of advanced features such as real-time protection, web filtering, and email scanning can leave vulnerabilities undetected, especially if they rely solely on ClamWin. Furthermore, the software's effectiveness largely depends on users proactively engaging with it, which can lead to gaps in security if not monitored closely. The biggest con, however, is that scanning large file systems will consume significant time and affect user productivity. </p>
<p>To effectively formulate and deploy business information systems solutions, an analysis is crucial. This process begins with identifying all personnel utilizing the system to gather diverse perspectives on needs. Conducting interviews, surveys, and workshops helps capture both functional and non-functional requirements, ensuring the system aligns with user expectations and business objectives. The information is compiled into a detailed requirements document, which serves as a reference throughout the development process. Additionally, performing a study assesses the technical and financial viability of the proposed solution, ensuring the organization's infrastructure can support it. By rigorously applying requirements analysis, organizations can deploy information systems that not only enhance operational efficiency but also bolster security measures, thereby mitigating risks effectively. Overall, creating a plan that will meet all employees' needs is crucial as it will ensure that everyone's jobs can be completed as needed.
 </p>

<p><u> References </u></p>
<p> kilObit. (2022, December 9). Open Source Free Antivirus - ClamAV. Bing. https://www.bing.com/videos/riverview/relatedvideo?q=clamav+1029+windows+kilobit&mid=2303C7C6F3C0EE4A43D22303C7C6F3C0EE4A43D2&ajaxhist=0 </p>
