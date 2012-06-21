suricata-patchs
===============

Proposed suricata patch:

- suricata-1.2.1-archive.patch<br><br>
  This patch add an extra mode to the pcap-log mode to archive files.<br>
  With this added modality when pcap file are under dump by suricata they are written in archive_temp_dir: /directory/path <br>
  When then the file are closed are then moved to archive_dest_dir: /directory/path <br>
  To enable this kind of dump mode you need in pcap-log yaml section to set the following options: <br>

    mode = archive<br>
    archive_temp_dir = /path/where/dump/file/until/they/are/closed<br>
    archive_dest_dir = /path/where/dump/file/AFTER/thet/are/closed<br>
    
  
- suricata-1.x.-archive.patch<br>
  Under development . 