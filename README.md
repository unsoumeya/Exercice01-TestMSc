# Exercice01-TestMSc
# Test d’admission MSc Cyber – Exercice 01

## Objectif
Mettre en place un mini-lab réseau sous Cisco Packet Tracer intégrant :
- segmentation par VLAN
- routage inter-VLAN
- serveur DHCP
- accès Wi-Fi

## Topologie
Le réseau est composé de :
- 1 routeur Cisco 1941
- 3 switchs (un par bureau)
- 3 points d’accès Wi-Fi
- PC fixes, PC portables et téléphones IP

## Plan VLAN
- VLAN 1 : VoIP – 192.168.0.0/24
- VLAN 10 : Wi-Fi – 192.168.10.0/24
- VLAN 20 : PC fixes – 192.168.20.0/24
- VLAN 30 : Administration – 192.168.30.0/24

## Configuration
- Création des VLANs sur les switchs
- Affectation des ports selon l’énoncé
- Mise en place des trunks (ports 1 et 9)
- Configuration du routeur (router-on-a-stick)
- Configuration du DHCP sur le routeur

## Tests et validation
- Attribution d’adresses IP par DHCP sur les PC fixes
- Tests de connectivité (ping) entre les VLANs
- Vérification des trunks et du routage inter-VLAN


