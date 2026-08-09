# Snort-IDS-Project

## INTRODUCTION

The Snort command is used to run Snort, an open-source Network Intrusion Detection System (NIDS) and Intrusion Prevention System (NIPS). It allows security professionals and network administrators to monitor network traffic in real time, analyze packets, detect suspicious or malicious activities, and generate alerts based on predefined or custom rules.

**The basic syntax of the Snort command is:-** snort [options]

# Deployment Modes:
An IPS (Intrusion prevention System) is detects and malicious traffic in real time. An IDS (Intrusion Detection system) is detected the malicius activity and generates alerts but does not block traffic.
# Snort-Lab
## Building Snort Lab | IDS/IPS | By Abhishek Maurya
Snort is a powerful open-source network intrusion detection and prevention system (IDS/IPS). Important Note : If any problem occur while installation search it on YouTube rather than Google.

# Steps Before Installation
Open Terminal and run some commands in Kali Linux
## sudo apt update
<img width="1273" height="256" alt="Screenshot 2026-08-09 114836" src="https://github.com/user-attachments/assets/2d8ae935-78b0-40d7-8f88-9f926cfc4436" />

# Installation on snort on Kali Linux

## sudo apt install snort -y

<img width="1093" height="416" alt="image" src="https://github.com/user-attachments/assets/849a693b-65cc-4e8f-ae1d-6a074000b7e1" />

# Check snort is install or not by checking version
## snort -V
<img width="1072" height="433" alt="image" src="https://github.com/user-attachments/assets/9db3018c-6a53-43a8-b106-6ec9089f71fe" />

# Writing Rules in Snort
Basic rules Can be written as the following

Enter Command
# sudo nano /etc/snort/rules/local.rules

type your rules

1. alert icmp any any -> any any (msg:"ICMP Traffic Detected"; sid:1000001; rev:1;)
2. alert tcp any any -> any 80 (msg:"HTTP Traffic Detected"; sid:1000002; rev:1;)
3. alert tcp any any -> any 443 (msg:"HTTPS Traffic Detected"; sid:1000003; rev:1;)

<img width="1252" height="745" alt="Screenshot 2026-08-08 172415" src="https://github.com/user-attachments/assets/1f908a3e-3549-42e8-8106-0e5582af26a1" />
Type command for checking the logs


