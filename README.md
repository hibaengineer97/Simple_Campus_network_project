# Simple_Campus_network_project / Projet réseau simple d'un campus (Cisco Packet Tracer)

[English](#english) | [Français](#français)

## English

Multi-building campus network with VLANs, DHCP relay (`ip helper-address`) and inter-VLAN routing.

### Content
- `packet-tracer/`: project file (.pkt)
- `configs/`: router and switch configurations
- `docs/LIVRABLE_miniprojet1.pdf`: full report (in French)
- `screenshots/`: topology and tests

### Summary
- 10 VLANs, one per department
- DHCP on the Main Router (VLANs 10 to 80) and the Branch Router (VLANs 9 and 100)
- Inter-VLAN routing on the 3650 multilayer switches
- Serial links between routers and static routes

### Adressing
| Department | VLAN | Subnet | Gateway |
|---|---|---|---|
| Admin | 10 | 192.168.1.0/24 | 192.168.1.1 |
| HR | 20 | 192.168.2.0/24 | 192.168.2.1 |
| Business | 30 | 192.168.3.0/24 | 192.168.3.1 |
| Finance | 40 | 192.168.4.0/24 | 192.168.4.1 |
| Engineering | 50 | 192.168.5.0/24 | 192.168.5.1 |
| Art & Design | 60 | 192.168.6.0/24 | 192.168.6.1 |
| Student Lab | 70 | 192.168.7.0/24 | 192.168.7.1 |
| IT | 80 | 192.168.8.0/24 | 192.168.8.1 |
| Staff | 9 | 192.168.9.0/24 | 192.168.9.1 |
| Student Lab (Health & Science) | 100 | 192.168.10.0/24 | 192.168.10.1 |

| Link | Network |
|---|---|
| Main Router to Branch Router | 10.10.10.0/30 |
| Main Router to Cloud Router | 10.10.10.4/30 |
| Cloud Router to Email Server | 20.0.0.0/30 |
| Main Router to Building A | 172.16.2.0/30 |
| Branch Router to Building B | 172.16.1.0/30 |


### Open the project
Open `packet-tracer/PROJETYANECODE1ST.pkt` with Cisco Packet Tracer.

### Author
hiba_Jean

Project built during a cybersecurity and networking training program in YaneCodeACademy



## Français

Réseau de campus multi-bâtiments avec VLANs, DHCP via relais (`ip helper-address`) et routage inter-VLAN.

### Contenu
- `packet-tracer/` : fichier du projet (.pkt)
- `configs/` : configurations des routeurs et des switchs
- `docs/LIVRABLE_miniprojet1.pdf` : rapport complet (en français)
- `screenshots/` : topologie et tests

### Résumé
- 10 VLANs, un par département
- DHCP sur le Main Router (VLANs 10 à 80) et le Branch Router (VLANs 9 et 100)
- Routage inter-VLAN sur les switchs multicouches 3650
- Liaisons série entre les routeurs et routes statiques

### Ouvrir le projet
Ouvrir `packet-tracer/PROJETYANECODE1ST.pkt` avec Cisco Packet Tracer.

### Auteur
hiba_Jean

Projet réalisé lors d'une formation en cybersécurité et réseaux à YaneCodeAcademy



