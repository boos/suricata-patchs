suricata-patchs
===============

Proposed suricata patch:

- suricata-1.2.1-archive.patch 
  This patch add an extra mode to the pcap-log mode to archive files.
  With this added modality when the file are under dump by suricata will be written in archive_temp_dir: /directory/path .
  When then the file are closed are then moved to archive_dest_dir: /directory/path . 
  To enable this kind of dump mode you need in pcap-log yaml section to set the following options: 

    mode = archive
    archive_temp_dir = /path/where/dump/file/until/they/are/closed
    archive_dest_dir = /path/where/dump/file/AFTER/thet/are/closed
    # other normal pcap options follows .. 
  
- suricata-1.x.-archive.patch
  Under development . 