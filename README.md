# PCAPDecrypt-Encrypt
Decrypt and Encrypt Wireshark PCAP files
When saving or even dumping Packet captures on Wireshark or any other packet sniffer/capture software using the PCAP lib the captured data will most likely be encrypted after playing around with the binaries i manage to output some readable data and convert them back.

If you have Wireshark downloaded we will be using the Tshark.exe file to decrypt & text2pcap.exe to encrypt:


Decrypting:


tshark.exe -r input.pcap -x > output.txt


Encrypting:


text2pcap.exe -F pcap output.txt new.pcap
