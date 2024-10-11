# SubnettingLab


Cisco Packet Tracer Subnetting Lab

English Version

Overview
This project demonstrates subnetting a single network (192.168.1.0/24) into two smaller subnets using Cisco Packet Tracer. It includes the configuration of PCs, switches, and a router to ensure all devices can communicate with each other. The network is divided as follows:

Subnet 1 (Left): 192.168.1.0/25
Subnet 2 (Right): 192.168.1.128/25
Topology
The network consists of:

PC1 connected to Switch S1
PC2 connected to Switch S2

Switch S1 and Switch S2 connected to Router R1

Tasks

Subnet the network: Divide 192.168.1.0/24 into two subnets.

Configure Subnet 1 (S1): Use the first half of the addresses (192.168.1.0/25).

Configure Subnet 2 (S2): Use the second half of the addresses (192.168.1.128/25).

Configure PCs: Assign the first IP address of each subnet to PC1 and PC2.

Configure the router: Use the last IP address of each subnet for router interfaces.

Connect the router between switches: Use Gig0/0/0 and Gig0/0/1.

Configure switches: Use the second IP address of each subnet for S1 and S2.

Verify connectivity: Ensure all devices can ping each other.

Step-by-Step Guide

Step 1: Subnet the Network

Divide the original network (192.168.1.0/24) into two /25 subnets:

Subnet 1 (S1): 192.168.1.0/25 (Range: 192.168.1.1 - 192.168.1.126, Broadcast: 192.168.1.127)

Subnet 2 (S2): 192.168.1.128/25 (Range: 192.168.1.129 - 192.168.1.254, Broadcast: 192.168.1.255)

Step 2: Configure PCs

PC1 Configuration:

IP Address: 192.168.1.1
Subnet Mask: 255.255.255.128
Default Gateway: 192.168.1.126
PC2 Configuration:

IP Address: 192.168.1.129
Subnet Mask: 255.255.255.128
Default Gateway: 192.168.1.254
Step 3: Configure the Router
Interface Gig0/0/0:

IP Address: 192.168.1.126
Subnet Mask: 255.255.255.128
No Shutdown
Interface Gig0/0/1:

IP Address: 192.168.1.254
Subnet Mask: 255.255.255.128
No Shutdown
Step 4: Configure the Switches
Switch S1:

IP Address: 192.168.1.2
Subnet Mask: 255.255.255.128
Switch S2:

IP Address: 192.168.1.130
Subnet Mask: 255.255.255.128

Step 5: Connect the Router Between Switches

Connect Gig0/0/0 on Router R1 to Gig1/0/2 on Switch S1.
Connect Gig0/0/1 on Router R1 to Gig1/0/2 on Switch S2.

Step 6: Verify Connectivity

Use the ping command on PC1 to ping PC2.
Verify that all devices can communicate across the network.

Versione Italiana

Panoramica

Questo progetto dimostra la suddivisione di una singola rete (192.168.1.0/24) in due sottoreti più piccole utilizzando Cisco Packet Tracer. Comprende la configurazione di PC, switch e router per garantire che tutti i dispositivi possano comunicare tra loro. La rete è divisa come segue:

Sottorete 1 (S1): 192.168.1.0/25
Sottorete 2 (S2): 192.168.1.128/25
Topologia
La rete è composta da:

PC1 connesso a Switch S1

PC2 connesso a Switch S2

Switch S1 e Switch S2 connessi a Router R1

Compiti

Sotto-segmentare la rete: Dividere 192.168.1.0/24 in due sottoreti.

Configurare la Sottorete 1 (S1): Utilizzare la prima metà degli indirizzi (192.168.1.0/25).

Configurare la Sottorete 2 (S2): Utilizzare la seconda metà degli indirizzi (192.168.1.128/25).

Configurare i PC: Assegnare il primo indirizzo IP di ciascuna sottorete a PC1 e PC2.

Configurare il router: Utilizzare l'ultimo indirizzo IP di ciascuna sottorete per le interfacce del router.

Collegare il router tra gli switch: Utilizzare Gig0/0/0 e Gig0/0/1.

Configurare gli switch: Utilizzare il secondo indirizzo IP di ciascuna sottorete per S1 e S2.

Verificare la connettività: Assicurarsi che tutti i dispositivi possano comunicare tra loro.

Guida Passo-Passo

Passo 1: Sotto-segmentare la Rete

Dividere la rete originale (192.168.1.0/24) in due sottoreti /25:

Sottorete 1 (S1): 192.168.1.0/25 (Intervallo: 192.168.1.1 - 192.168.1.126, Broadcast: 192.168.1.127)

Sottorete 2 (S2): 192.168.1.128/25 (Intervallo: 192.168.1.129 - 192.168.1.254, Broadcast: 192.168.1.255)

Passo 2: Configurare i PC

Configurazione di PC1:

Indirizzo IP: 192.168.1.1
Maschera di Sottorete: 255.255.255.128
Gateway Predefinito: 192.168.1.126
Configurazione di PC2:

Indirizzo IP: 192.168.1.129
Maschera di Sottorete: 255.255.255.128
Gateway Predefinito: 192.168.1.254
Passo 3: Configurare il Router
Interfaccia Gig0/0/0:

Indirizzo IP: 192.168.1.126
Maschera di Sottorete: 255.255.255.128
No Shutdown
Interfaccia Gig0/0/1:

Indirizzo IP: 192.168.1.254
Maschera di Sottorete: 255.255.255.128
No Shutdown
Passo 4: Configurare gli Switch
Switch S1:

Indirizzo IP: 192.168.1.2
Maschera di Sottorete: 255.255.255.128
Switch S2:

Indirizzo IP: 192.168.1.130
Maschera di Sottorete: 255.255.255.128
Passo 5: Collegare il Router Tra gli Switch
Connettere Gig0/0/0 su Router R1 a Gig1/0/2 su Switch S1.
Connettere Gig0/0/1 su Router R1 a Gig1/0/2 su Switch S2.

Passo 6: Verificare la Connettività

Utilizzare il comando ping su PC1 per pingare PC2.
Verificare che tutti i dispositivi possano comunicare sulla rete.
