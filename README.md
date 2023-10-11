Instuction to run the Assignment:
For HTTP Server Emulation:

In the /basic directory, run the following commands:
- make clean
- make run
- run "xterm h1" & "xterm  h2" in the Mininet prompt.
- Two separate shells open, named H1 & H2
- run "bash h2-arp.sh" & "python server.py" on the H2 shell
- run "bash h1-arp.sh" & "python client.py" on the H1 shell
- Enter IP: "10.0.1.2" when prompted. Note: " " are needed
- Enter the commands on the client shell when prompted
- For PUT: "PUT /assignment2/key/val HTTP/1.1"
- For GET: "GET /assignment2?request=key HTTP/1.1"
- For DELETE: "DELETE /assignment2/key HTTP/1.1"

For WebCache Development:
- make clean
- make run
- run "xterm h1" & "xterm  h2" & "xterm h3" in the Mininet prompt.
- Three separate shells open, named H1 & H2 & H3
- run "bash h3-arp.sh" & "python server.py" on the H3 shell
- run "bash h2-arp.sh" & "python cache.py" on the H2 shell
- run "bash h1-arp.sh" & "python client.py" on the H1 shell
- Enter "PUT" or "GET" when prompted
- If "PUT" is chosen, enter key & value when prompted
- If "GET" is chosen, enter key when prompted


Location of pcap File:
For HTTP Server Emulation:
- The "basic" directory contains "mypcaps" Folder.
- This folder contains pcap file for pcap traces at H1 for all three types of requests

For Web Cache Development:
- The "star" directory contains "mypcaps" Folder.
- This Folder contains 2 Folders "incache" , "notincache"
- "incache" contains 3 pcap files of case where given key is already in the cache 
- H1 : Client - s1-eth1.pcap
  H2 : Cache  - s1-eth2.pcap
  H3 : Server - s1-eth3.pcap

- "notincache" contains 3 pcap files of case where given key is not in the cache 
- H1 : Client - s1-eth1.pcap
  H2 : Cache  - s1-eth2.pcap
  H3 : Server - s1-eth3.pcap


Location of Reports:
For HTTP Server Emulation:
- The "basic" directory contains 'Report' Folder. This folder contains 'Report-1.pdf' file

For Web Cache Development:
- The "star" directory contains 'Report' Folder. This folder contains 'Report-2.pdf' file

- All the inbuilt files are present in their respective locations


