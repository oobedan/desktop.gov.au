# Changelog

You can find published releases at [https://github.com/govau/desktop.gov.au/releases](https://github.com/govau/desktop.gov.au/releases) where you can more easily compare between versions.

## Next version

* Incorporate Essential Eight July 2021 updates and expanded detail [#116]
* Updated the Windows Defender Application Control guidance [#78]
* Updated and consolidated the Continuous Monitoring Plan to be more blueprint specific [#73]
* Updated minimum Windows Server version requirement for Azure AD Connect [#86]
* Extended the Solution Overview with Zero Trust [#82] and secure systems administration [#80]
* Replacement of security baselines for better compliance with ACSC hardening guidance [#87] [#110]
* Client devices design
  * Overall tidy up, freshen and incorporate latest ACSC Essential Eight guidance [#85]
  * Update justification for fast user switching [#79]
  * Updated Windows 10 and Edge hardening sections to align to the 21H1 Windows 10 Hardening Guide from the ACSC. This included removing guidance on Windows To Go [#93]
  * Genericise references to specific versions of Windows hardening guidance [#94]
  * Expand Office hardening with ACSC Office guidance [#95] 
  * Add browser based web advertisement blocking guidance [#105]
  * Incorporated Apple Business Manager together with Intune to allow for application control [#113]  
  * Other minor changes [#99]
* Office 365 general uplift, including: [#88]
  * More on DKIM/DMARC/SPF
  * More on data loss prevention policy
  * M365 group creation lockdown
  * Clarify retention vs backup
  * Other minor changes [#100]
* Platform and Platform ABAC uplift including: [#92]
  * Add Azure AD Tenant Restrictions section
  * Better alignment with E8 July 2021 changes
  * Updated guidance on M365 group naming policy
  * Incorporate Terms of Use capability
  * Expanded privileged identity management roles
  * Update to product names (eg Azure ATP -> Defender for Identity, Microsoft Defender ATP -> Microsoft Defender for Endpoint) [#110]
* Client devices ABAC [#115]
  * General clean up, readability enhancements and removal of items no longer required 
  * Migration of settings from Configuration Profiles to Endpoint Security
  * Additional custom firewall rules added (ACSC - Windows Firewall Rules policy)
  * New Endpoint Security device control policy (ACSC - Device Control)
  * New Endpoint Security exploit protection policy (ACSC - Exploit Protection)
  * New Endpoint Security Application Guard policy (ACSC - Application Guard)
  * Updated Defender for Endpoint deployment
  * Improvements to iOS hardening profiles
  * Improvement to iOS device enrollment and application delivery
  * Removal of conflicting guidance around Office security and macro setting (Trusted location removed to align with Client Devices design update)
  * Updated Intune configuration to include a method to block web browsers and Outlook for administrators [#81]
  * Add Ease of Use section [#141]
* Office 365 ABAC uplift [#124]
  * 2018.4 PSPF updates
  * Added Global Settings for Safe Links
  * Updated Exchange policies [#140]
* Consolidated duplicate As-Built-As-Configured content for a better user experience [#109]
* Add ability to disable inactive user accounts as per Essential Eight July update [#111]
* Updated detail for PSPF labelling limitations [#114] [#138]
* Updated sensitivity labels [#130] and provide an automated method for deploying sensitivity labels using M365DSC [#117]
* Updated and expanded Identity and Access Management DSC script to include group settings and tenant contacts [#137]
* Incorporated updated ACSC references: Apple iOS 14 Devices (Oct 2021), Essential Eight (Oct 2021), Microsoft Office Hardening (Oct 2021) and Windows Hardening (Oct 2021) [#125] [#139]

Other general website changes:

* Expanded the engagement model into a larger comprehensive framework [#96]
* Added a new "Patterns" section with a remote access pattern using Azure Virtual Desktop [#107] [#128]

## June 2021

For exact details on changes, please follow the linked pull request tickets.

* Forms, Whiteboard and Planner have been added to the blueprint. These products have been IRAP assessed to handle government PROTECTED data [#44]
* Incorporate ISM April 2021 updates (from October 2020) [#43]
* Incorporate iOS 14 hardening (from iOS 12) [#44]
  * The updated guidance now requires the use of a virtual private network (notably via per-app VPN) for data in transit. We have modified our solution overview to identify this early [#52]
* Improve Windows application whitelisting by incorporating Windows Defender Application Control [#34] 
* Improve OLE protections. We believe this will increase the maturity rating for User Application Hardening [#44]
* Update Intune and SCCM references to better reflect current state [#44]
  * `System Center Configuration Manager` updated to `Microsoft Endpoint Configuration Manager`
  * `Intune` to `Microsoft Endpoint Manager - Intune` to reflect the move into the Microsoft Endpoint Manager suite
* In Identity and access management > Azure Active Directory, removed ambiguity around app registration [#48]
* Updated Log Analytics section and configured diagnostic settings for Microsoft Endpoint Manager and Azure Active Directory [#44]
* Our first foray into scripting the configuration and auditing of Identity and Access Management items using Microsoft 365 Desired State Configuration [#59]
* Renamed Office 365 Advanced Threat Protection to Microsoft Defender for Office 365 [#61]
* Renamed Office 365 groups to Microsoft 365 groups [#44]
* Updated Unified Audit log retention to 10 years [#44]
* Updated the Microsoft 365 organisation configuration section [#44]
* Add ABACs for Safe Links, Safe Attachments and Anti-phishing [#61]
* Expand on Teams ABACs (including guest and external access) [#69]
* Supply CMTrace and DefenderATP PowerShell scripts [#69]
* Redo sensitivity labels [#69]
* General clean up [#49]
* Fix timezone OMA-URI [#58]

## February 2021 dot 1

This release incorporates changes to the ISM to October 2020.

* New documents added
  * Continuous Monitoring Plan
  * Cloud Assessment and Authorisation Alignment
* Overview
  * Replaced "whitelist/blacklist" terminology with "allow/deny lists"
* Client Devices
  * Incorporate ACSC Windows 10 hardening guidance 1909
  * iOS minimum password length increased to 14
* Office 365
  * Additional Telstra calling decision point added
  * Removed typo in mail flow images 
* Platform
  * Replaced "whitelist/blacklist" terminology with "allow/deny lists"
* ABAC Platform, Incident response plan
  * Update ITSA address to align with the value from hybrid. Neither ISM or the PSPF require agencies to have an ITSA
* Security Risk Management Plan
  * Included to reflect additional and expanded treatments outlined within the SSP Annex which are relevant to this risk
  * Call out additional controls that have been highlighted as agency responsibility in the SSP Annex
  * Added additional controls
  * Correct wording for better context
* System Security Plan
  * New sections added
    * Shared responsibility matrix
    * Virtualisation hardening
  * Indicate when logs are generated
  * Personnel security section expanded
  * Better clarity
* SSP Annex documents updated

## February 2021

Joining the overviews, all remaining Blueprint documents have been incorporated into the website. These include as built as configured, security and standard operating procedures. All documents are the August 2020 release (currently available).

Added site wide search functionality.

## October 2020

* Website release
* Second iteration of the Blueprint covering hybrid environments
