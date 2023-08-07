# WiFi Network Attack: Intrusion, Reconnaissance, Monitoring


## Project Overview
In this project I will be demonstrating a Network Attack with my home wifi; the intruder will find my network, gain access, scan my local devices, and start monitoring my outbound traffic. 





##
### 1. Setup 
For this project I will be using Parrot OS combined with a network adapter and the tools below.

- airodump-ng
- aireplay-ng
- hashcat
- nmap
- ettercap
- wireshark



### 2. Reconnaissance
- Set the adapter in monitor mode and use airodump-ng to monitor networks within range, target a network, and get their BSSID MAC adress, channel,
- Use airo dumpt to associate clients with a network, get client MAC address, and set dumpfile to start collecting their network traffic/comms
  #
![Screenshot at 2023-08-06 20-30-47](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/e17b7555-1a54-4ece-a6d9-218227101903)
![Screenshot at 2023-08-06 20-30-56](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/3a1aa235-9b82-4d54-9d67-a2a4d013bf8b)
![Screenshot at 2023-08-06 20-36-00](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/571d04b8-617b-4aba-9980-3a6cd97381b3)




  #
### 3. De-authentication Attack
- use aireplay-ng to target a client, and send deauthentication packets to knock them off the network
   #
![Screenshot at 2023-08-06 20-39-04](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/c096197f-e9dc-4f56-99d3-0c9215443ac6)
![Screenshot at 2023-08-06 20-39-18](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/a9a61cb3-fba2-4ce8-9ef8-ab4e2b7a294c)





  #
### 4. Capture EAPOL Handshake
- capture EAPOL handshake and write it to a file that can be cracked
   #
![Screenshot at 2023-08-06 20-39-33](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/d3c72981-9fc9-4643-9d6f-eb0ffcfbeced)
![Screenshot at 2023-08-06 20-40-54](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/244ed00c-4b31-4343-852f-65d8837ce652)



  #
### 5. Hashcat Password Attack
- convert file and use hashcat to crack with rules and dictionary
  #
![Screenshot at 2023-08-06 20-48-22](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/38a2ef0e-06e4-4991-a91d-8165d022a880)
![Screenshot at 2023-08-06 20-48-47](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/52ed0480-2e03-46d8-a0f6-b1545ca8f4d1)



  #
### 6. Reconnaissance
- join network and run ifconfig and nmap for recon
- choose target
- run vulnerability scanner
   #
![Screenshot at 2023-08-06 20-57-53](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/b7c8905a-3d65-41d8-ac47-24f49c8b4f75)



  #
### 7. Arp Poisoning, MiTM
- use ettercap to arp poison
  #
![Screenshot at 2023-08-06 20-58-56](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/5bc771b4-90cf-4622-9ca5-9406abf3c1d6)



  #
### 8. Packet Capture
-use wireshark for detailed traffic monitoring and analysis
- use online tool to see hosts
  #
![Screenshot at 2023-08-06 21-02-03](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/5ba604b9-a0ff-4e1d-9b0a-ac763ec7666f)
![Screenshot at 2023-08-06 21-07-13](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/34c811cd-cb39-4c5e-aa20-065a1ff96fd7)
![Capture](https://github.com/blwhit/Network-Intrusion-and-Sniffing/assets/141170960/81fb0c30-248c-46f9-8516-276779ebf796)
  #





