# Salt Typhoon - Verified Facts

## F001 - Activity and targeting
Source: S02 - FBI
Relevance: Direct
Fact: Salt Typhoon compromised multiple US telecommunications companies.
Fact: The activity resulted in theft of call data logs, some private communications, and information subject to court-ordered US law enforcement requests.

## F002 - Organizational link
Source: S03 - US Treasury
Relevance: Direct
Fact: The US Treasury designated Sichuan Juxinhe Network Technology Co., LTD. for its direct involvement with the Salt Typhoon cyber group.

## F003 - Industry naming overlap
Source: S04 - Joint Advisory
Relevance: Associated / attribution caveat
Fact: The advisory lists Salt Typhoon, OPERATOR PANDA, RedMike, UNC5807, and GhostEmperor as names related to overlapping cyber activity.
Caveat: The advisory warns that industry group names do not necessarily correspond one-to-one with government attribution.

## F004 - Cmd1 SFTP client
Source: S04 - Joint Advisory
Relevance: Direct
Fact: The advisory includes a YARA rule named SALT_TYPHOON_CMD1_SFTP_CLIENT.
Fact: The rule contains strings related to packet capture, FTP export, SSH command shells, and SFTP download functions.

## F005 - New2 SFTP client
Source: S04 - Joint Advisory
Relevance: Direct
Fact: The advisory includes a YARA rule named SALT_TYPHOON_NEW2_SFTP_CLIENT.
Fact: The rule contains strings related to command execution, logging, encryption configuration, and network sniffing.

## F006 - General Chinese state-sponsored activity
Source: S04 - Joint Advisory
Relevance: Context only
Fact: The advisory describes compromises of telecommunications, government, transportation, lodging, and military networks.
Caveat: These general observations must not automatically be attributed to Salt Typhoon individually.

## F007 - Initial access and persistence observations
Source: S08 - Cisco Talos
Relevance: Direct, based on Talos investigations
Fact: Talos determined that initial access to Cisco devices in the incidents it investigated was obtained through legitimate victim login credentials.
Fact: Talos observed persistence across devices from multiple vendors, including one instance lasting more than three years.
Caveat: These observations describe Talos-investigated incidents and should not be generalized to every Salt Typhoon operation.

## F008 - Credential collection
Source: S08 - Cisco Talos
Relevance: Direct
Fact: Talos observed collection of network credentials and secrets from SNMP, TACACS, and RADIUS traffic.
Caveat: The report describes the likely purpose of some activity as obtaining additional credentials; preserve the report's qualification.

## F009 - Configuration exfiltration and reconnaissance
Source: S08 - Cisco Talos
Relevance: Direct
Fact: Talos observed network device configurations being transferred using TFTP or FTP.
Fact: These configurations could expose authentication material and network information useful for reconnaissance and lateral movement.

## F010 - JumbledPath
Source: S08 - Cisco Talos
Relevance: Direct
Fact: Talos documented a custom utility named JumbledPath used for remote packet capture through a jump host.
Fact: The report describes attempts to clear logs and impair logging during this activity.

## F011 - RedMike activity and vulnerability exploitation
Source: S09 - Recorded Future / Insikt Group
Relevance: Associated / attribution caveat
Fact: Recorded Future reported that RedMike attempted to exploit more than 1,000 Cisco devices.
Fact: The report describes an exploitation sequence involving CVE-2023-20198 for initial access and CVE-2023-20273 to obtain root access.
Caveat: Recorded Future assesses RedMike as associated with Salt Typhoon; this is an analytical attribution, not proof that the names identify exactly the same entity.

## F012 - Observed compromised devices and GRE tunnels
Source: S09 - Recorded Future / Insikt Group
Relevance: Associated / attribution caveat
Fact: Recorded Future observed seven compromised Cisco devices communicating with RedMike infrastructure.
Fact: The report describes GRE tunnels between compromised Cisco devices and infrastructure, used for persistence and data exfiltration.
Caveat: Distinguish more than 1,000 devices targeted from the seven compromised devices observed by Recorded Future. Preserve the report's RedMike attribution qualification.
