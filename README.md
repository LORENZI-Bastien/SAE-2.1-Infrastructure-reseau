# SAÉ 2.1 · Construire un réseau pour une petite structure

> Mise en place d’une infrastructure réseau complète permettant de démarrer des machines sans disque par le réseau (PXE).

| | |
|---|---|
| **Formation** | BUT Réseaux et Télécommunications, Montbéliard |
| **Année** | 1<sup>re</sup> année, semestre 2 |
| **Organisation** | En équipe de 4, jalons répartis entre les membres |
| **Outils et notions** | `Cisco` `DHCP` `Relais DHCP` `PXE` `NFS` `TFTP` `SSH` `VLAN` `Port security` `Packet Tracer` `Linux` |

## Objectif

Concevoir et configurer le réseau d’une petite structure : plan d’adressage, routeur et switch Cisco, serveurs Linux (DHCP, TFTP, NFS, SSH), jusqu’au démarrage par le réseau d’un Raspberry Pi, d’une machine virtuelle et d’un PC.

## Ma part

- **Jalon 5 · Câblage et réseau 3** : câblage du switch et du routeur Cisco en console, configuration du relais DHCP (`ip helper-address`). Leçon retenue : sans `copy run start`, la configuration est perdue au redémarrage.
- **Jalon 8 · Serveur TFTP** : installation de `tftpd-hpa`, correction des droits et des chemins d’accès, sauvegarde de la configuration du routeur vers le serveur (`copy startup-config tftp:`), validée en conditions réelles.
- **Travail collectif** : plan d’adressage en /26, carte mentale, diagramme de Gantt, capture Wireshark de l’attribution d’adresse (filtre `bootp`), rapport et soutenance.

## Jalons du projet

| Jalon | Sujet |
|---|---|
| 1 | [Plan d’adressage IP](jalons/jalon-01-plan-adressage-ip.pdf), [Gantt](jalons/jalon-01-gantt.mvdx), [carte mentale](jalons/jalon-01-carte-mentale.mvdx) |
| 2 | [Configuration du Raspberry Pi pour le démarrage réseau](jalons/jalon-02-raspberry-pi.pdf) |
| 3 | [Simulation DHCP sous Packet Tracer](jalons/jalon-03-simulation-dhcp.pkt) |
| 4 | [Adresses IP statiques](jalons/jalon-04-ip-statiques.txt) |
| 5 | [Câblage et configuration du réseau 3](jalons/jalon-05-cablage-reseau-3.txt) |
| 6 | [Serveur DHCP](jalons/jalon-06-serveur-dhcp.txt) |
| 7 | [Capture Wireshark](jalons/jalon-07-capture-wireshark.pdf) |
| 8 | [Serveur TFTP](jalons/jalon-08-serveur-tftp.txt) |
| 9 | [NFS et démarrage PXE](jalons/jalon-09-nfs-boot-pxe.txt) |
| 10 | [SSH sécurisé](jalons/jalon-10-ssh.txt) |
| 11 | [VLAN et sécurisation du switch](jalons/jalon-11-vlan-securite-switch.txt) |
| 12 | [Jalon 12](jalons/jalon-12.pdf) |

## Contenu du dépôt

```
rapport/       retour d’expérience de l’équipe
presentation/  diaporama de soutenance
jalons/        livrables de chaque jalon
consignes/     sujets et supports fournis par l’IUT
```

---

<sub>Bastien Lorenzi · BUT Réseaux et Télécommunications, parcours cybersécurité · [Portfolio](https://wonderful-chebakia-f83e9d.netlify.app/#projets) · [Profil GitHub](https://github.com/LORENZI-Bastien)</sub>
