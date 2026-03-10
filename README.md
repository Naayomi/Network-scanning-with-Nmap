# Network-scanning-with-Nmap
This project demonstrates practical network enumeration using Nmap in a virtual lab environment with Kali Linux and Metasploitable. It includes host discovery, port scanning, service detection, and OS identification.

This project is part of my cybersecurity learning journey. It demonstrates practical use of Nmap to perform network scanning and reconnaissance in a controlled lab environment.

Using Kali Linux and Metasploitable, I conducted multiple scans to identify open ports, running services, and the operating system of the target machine.

## Tools Used
- Kali Linux
- Nmap
- Metasploitable 2
- VirtualBox

- ## Project Objectives

The main objectives of this lab were:

- Discover hosts on the network
- Identify open ports on the target machine
- Detect services running on open ports
- Identify the operating system of the target
- Understand basic network reconnaissance techniques

- ## Lab Setup

The project was conducted in a virtual lab environment using VirtualBox.

- Kali Linux was used as the attacking machine
- Metasploitable 2 was used as the vulnerable target machine
- Both machines were connected on the same virtual network

## Scanning Process

### Step 1: Identify Target IP Address

The IP address of the Metasploitable machine was identified using:

ifconfig


### Step 2: Test Connectivity

The target machine was tested using the ping command.

ping <target-ip>
![ping_test](https://github.com/user-attachments/assets/0555962b-07b0-4471-8c56-f8e1de496847)


### Step 3: Basic Port Scan

A basic Nmap scan was performed to identify open ports.

nmap <target-ip>
![Nmap_scan](https://github.com/user-attachments/assets/b4c23d9f-4e80-4c27-afc7-3d7e843b8440)

### Step 4: Service Detection Scan

Service detection was performed using:

nmap -sV <target-ip>
![Serviceversion_detectionscan](https://github.com/user-attachments/assets/2e72a993-3c03-4451-9174-cae824d4a25d)

### Step 5: Operating System (OS) Detection

The operating system of the target machine was detected using:

sudo nmap -O <target-ip>
![OS detection scan](https://github.com/user-attachments/assets/545b4168-f54a-42f1-ad87-fa3bac70419a)

### Step 6: Saving Scan Results

All Nmap scans were saved to a text file to document the findings and provide proof of work. Saving scans is important for reporting and analysis in cybersecurity projects.

nmap -sV <target-ip> -oN scan-results.txt
![[scan-results.txt](https://github.com/user-attachments/files/25869478/scan-results.txt)
scan-result]
(https://github.com/user-attachments/assets/1c014d86-0051-4150-b132-921c9f01fe4b)





