# Link Collection

These links were collected while running the MS-102 course.

---

## Links

| Topic | Links(s) | Notes |
| --- | --- | --- |
| Office Deployment Tool | [Docs](https://support.knowbe4.com/hc/en-us/articles/115004326408-Bypass-Safe-Link-and-Safe-Attachments-in-Microsoft-Defender-for-Office-365#:~:text=Click%20Save.-,Safe%20Attachments%20Bypass%20Rule,Click%20Save.),  [M365 Apps admin center](https://config.office.com/officeSettings/), [Download](https://www.microsoft.com/en-us/download/details.aspx?id=49117) | |
| MD for Office 365 | [Bypass Policies](https://support.knowbe4.com/hc/en-us/articles/115004326408-Bypass-Safe-Link-and-Safe-Attachments-in-Microsoft-Defender-for-Office-365#:~:text=Click%20Save.-,Safe%20Attachments%20Bypass%20Rule,Click%20Save.), [Third-party Phishing Simulation](https://learn.microsoft.com/en-us/defender-office-365/advanced-delivery-policy-configure), [Service Description](https://learn.microsoft.com/en-us/office365/servicedescriptions/office-365-advanced-threat-protection-service-description) | |
| Licenses | [M365Maps](https://m365maps.com/), [M365 Enterprise Licenses](https://go.microsoft.com/fwlink/p/?LinkID=2139145&clcid=0xc07&culture=de-at&country=at) | |
| SPO - Sync disable | [Blog](https://blog.dan-toft.dk/2022/12/add-shortcut-onedrive-sync/) | With PowerShell see [Hint 1](#hint-1) |
| M365 Roadmap | [Roadmap](https://www.microsoft.com/en-us/microsoft-365/roadmap) | |

---

## Hints

### Hint 1

```PowerShell
#Connect to SharePoint Online
Connect-SPOService "https://<yourTenant>-admin.sharepoint.com"
 
#Disable "Add Shortcut to OneDrive"
Set-SPOTenant -DisableAddShortCutsToOneDrive $True
```
