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
