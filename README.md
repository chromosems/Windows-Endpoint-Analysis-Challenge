# Windows-Endpoint-Analysis-Challenge
## Instructions:
You've been assigned to remotely investigate a compromised Windows workstation as part of a live incident response scenario. The affected system has been imaged and all necessary forensic artifacts have been gathered. Your objective now is to investigate the scope of the compromise and identify any persistence mechanisms installed by the attacker.

## Tools Used
- Task manager
- Registry editor
- Process Explorer
- TcpView
- Command prompt

## Skilled learnt
- Threat detection and analysis
- Incident Response and Mitigation
- Security tool Mastery
- Malware Analysis

Use your endpoint analysis skills to conduct the investigation and answer the questions below
## What port is the challenge.exe malware listening on?
Using both TCPview and netstat -anob the listening port is 50050
- <img width="481" height="300" alt="image" src="https://github.com/user-attachments/assets/18ab7834-504a-4a7d-ab73-a312e0006189" />
- <img width="635" height="165" alt="image" src="https://github.com/user-attachments/assets/6589bb43-5527-48ec-a256-6387fedba09e" />
## What is the Process ID (PID) of the malware? This answer cannot be verified, but it's required for the next question(s)
- <img width="440" height="232" alt="image" src="https://github.com/user-attachments/assets/4b8d873d-8719-410c-ac41-e287a83230a2" />
## List all of the loaded DLL modules for the listener's associated process. What are the names of the two DLLs that start with the letter m?
To list DLL associated with the malware file, use the PID for to point to the file and /M to list DLL
- <img width="515" height="85" alt="image" src="https://github.com/user-attachments/assets/b52f4ad1-dc35-426d-be22-fd8069c96b8b" />
##  What is the name of the malware's parent process?
- <img width="459" height="520" alt="image" src="https://github.com/user-attachments/assets/b9827431-b019-4bf8-ba61-c1a6a22e78e8" />
## List all the shared resources on the local system. What is the name of the share that the attacker created?
 use netshare to list all file shares then analyze unfamiliar share names
 - <img width="444" height="121" alt="image" src="https://github.com/user-attachments/assets/6896d36a-8b4f-431b-9f26-96fa245158af" />
## The attacker created a Run entry to establish persistence on the system. What is the full path of the registry key?
- <img width="722" height="55" alt="image" src="https://github.com/user-attachments/assets/ef9d2ee0-d338-4296-a843-483be4dd8b5e" />

## What is the name of the backdoor service installed by the attacker?
- <img width="778" height="245" alt="image" src="https://github.com/user-attachments/assets/259bb911-3f5f-4d73-b24c-804cade1586d" />
## 
What is the name of the scheduled task created by the attacker?

- <img width="762" height="170" alt="image" src="https://github.com/user-attachments/assets/b1e54d6b-aaa1-4cca-9709-356d3b07e45f" />

## At what time is the scheduled task set to run?
- <img width="409" height="280" alt="image" src="https://github.com/user-attachments/assets/7fd3987f-dd24-4add-a26c-bf500894e6dd" />
##
What is the START_TYPE configuration of the service?
- <img width="317" height="282" alt="image" src="https://github.com/user-attachments/assets/2fcf57f2-a1bb-44fb-bebb-a9926b878c12" />

