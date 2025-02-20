## Objective


The SOC Automation Lab project aimed to establish a controlled environment for simulating and detecting cyber attacks. The primary focus was to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test telemetry to mimic real-world attack scenarios. This hands-on experience was designed to deepen understanding of network security, attack patterns, and defensive strategies.

### Skills Learned


- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used


- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools to create realistic network traffic and attack scenarios.

## Steps

*Ref 1: Network Diagram displaying the flow of data*   <img width="960" alt="Screenshot 2025-01-17 223144" src="https://github.com/user-attachments/assets/e7a3732d-c27e-4887-b560-8664b08db5aa" />

*Ref 2: Windows 10 Machine Setup*  <img src="https://github.com/user-attachments/assets/17d67402-9f80-4a60-8250-575d312d2ff8" />

*Ref 3: Install Sysmon for our Windows 10 Machine* <img src="https://github.com/user-attachments/assets/57acda57-b84f-4272-a3a8-bad15a297c46" /> 

*Ref 3: Configure a Firewall for our Wazuh Server and theHive hosted on Digital Ocean Cloud                                              
We will only allow traffic from our public IP* <img width="960" alt="Screenshot 2025-01-20 184259" src="https://github.com/user-attachments/assets/81af3025-7c2b-4cfc-b63a-35062c3780d6" />

*Ref 5: Install the Wazuh Server* <img alt="Screenshot 2025-01-20 193713" src="https://github.com/user-attachments/assets/cc48f07c-ed2c-4da1-adc1-21f0d873780f" />

*Ref 6/7: Configure Cassandra Database for theHive and then start the service* 
<img width="960" alt="Screenshot 2025-01-21 204216" src="https://github.com/user-attachments/assets/1a971bd5-1e90-400a-8292-3a7f1995e61d" />
<img alt="Screenshot 2025-01-21 204751" src="https://github.com/user-attachments/assets/7fca46c8-ac45-4882-b2ce-1473aa447be4" />

*Ref 8: Start and Enable ElasticSearch* <img alt="Screenshot 2025-01-21 210158" src="https://github.com/user-attachments/assets/c33b59f0-cd8a-45d4-975c-e4fc4bdb1a1f" />

*Ref 8: Start and Enable theHive* <img alt="Screenshot 2025-01-21 222347" src="https://github.com/user-attachments/assets/14f09ded-d3aa-4eac-b732-a3ea28997e44" />

*Ref 9: Install our Wazuh Agent* <img alt="Screenshot 2025-01-22 000803" src="https://github.com/user-attachments/assets/cf00b19f-4ba4-44f2-bdfb-8789f1297ae5" />

*Ref 10: Filter the Wazuh Agent for Sysmon Events* <img alt="VirtualBox_demo_23_01_2025_00_07_01" src="https://github.com/user-attachments/assets/f6222748-58b7-49a1-803e-e5739d64928b" />

*Ref 11: FDownload and Install Mimikatz* ![VirtualBox_demo_23_01_2025_01_00_13](https://github.com/user-attachments/assets/cea4fd3a-7457-46f0-bce0-91231a9c5e46)
*Ref 12: Edit our configuration log to forward all alerts to Wazuh* ![Screenshot 2025-01-23 011215](https://github.com/user-attachments/assets/96499da2-7fe7-4672-9f3a-d4f6fed04083)

*Ref 13: Create a Custom Rule in Wazuh to detect Mimikatz credential dumping*![VirtualBox_demo_23_01_2025_02_21_51](https://github.com/user-attachments/assets/003e827d-92d3-44d7-901d-19bb28dd32a9)

*Ref 14: Add an integration tag to our Wazuh config files to allow Shuffle connection
![Screenshot 2025-02-19 232328](https://github.com/user-attachments/assets/905e90cf-2ee9-49f4-ab98-20ace99e4842)

*Ref 15: Use regex to parse our SHA256 hash from Wazuh ![Screenshot 2025-02-20 005823](https://github.com/user-attachments/assets/1e7be111-3ed0-48f4-a0db-adf09421d6d6)
![Screenshot 2025-02-19 234514](https://github.com/user-attachments/assets/5769c9c8-1bdc-4fe5-8357-c5060c22b147)

 
