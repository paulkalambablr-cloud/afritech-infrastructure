
# AFRITECH
## Conception, déploiement et sécurisation d'une infrastructure informatique multiservices

**Projet pratique de laboratoire – Réseaux, Administration Systèmes et Cybersécurité**

## 1. Présentation du projet

AFRITECH est un laboratoire informatique virtualisé conçu pour mettre en pratique les compétences en architecture réseau, administration des systèmes, gestion des services informatiques et cybersécurité.

L'objectif est de concevoir une infrastructure segmentée, administrable, supervisée et sécurisée, inspirée d'un environnement informatique d'entreprise.

## 2. Objectifs

- Concevoir une architecture réseau segmentée en plusieurs zones.
- Déployer et administrer des serveurs Windows et Linux.
- Centraliser l'identité et l'authentification avec Active Directory.
- Fournir les services DNS et DHCP.
- Contrôler les communications entre les différents réseaux.
- Gérer les équipements et les demandes d'assistance informatique.
- Superviser l'infrastructure et surveiller les événements de sécurité.

## 3. Architecture technique

Le laboratoire repose sur plusieurs zones réseau :

| Zone | Réseau | Fonction |
|---|---|---|
| SERVEURS | 192.168.10.0/24 | Services d'infrastructure |
| UTILISATEURS | 192.168.20.0/24 | Postes utilisateurs |
| ADMIN-IT | 192.168.30.0/24 | Administration informatique |
| INVITÉS | 192.168.40.0/24 | Réseau isolé des invités |
| DMZ | 192.168.50.0/24 | Services exposés |
| SOC-NOC | 192.168.60.0/24 | Supervision et sécurité |

Le routage et le filtrage entre les zones sont assurés par un équipement VyOS configuré comme routeur et pare-feu.

## 4. Services et composants

| Composant | Technologie | Fonction |
|---|---|---|
| Contrôleur de domaine | Windows Server / Active Directory | Gestion centralisée des identités |
| DNS | Windows Server | Résolution de noms |
| DHCP | Windows Server | Attribution automatique des adresses IP |
| Gestion informatique | GLPI | Inventaire et tickets d'assistance |
| Supervision | Zabbix | Surveillance des équipements et services |
| Sécurité | Wazuh | Surveillance et analyse des événements |
| Routage et filtrage | OPNsense | Routage inter-réseaux et contrôle des flux |
| Virtualisation | VMware Workstation / VirtualBox | Hébergement du laboratoire |

## 5. Sécurité réseau

Les principes appliqués dans le laboratoire comprennent :

- Segmentation des réseaux par zones.
- Filtrage des communications selon les besoins.
- Restriction des accès d'administration.
- Contrôle des flux entre les segments.
- Surveillance de l'infrastructure.
- Centralisation et analyse des événements de sécurité.

## 6. Tests et validations

Les vérifications portent notamment sur :

- La résolution DNS.
- L'attribution des adresses IP.
- L'authentification dans le domaine.
- La communication entre les services autorisés.
- Le fonctionnement des règles de filtrage.
- La supervision des équipements avec Zabbix.
- La surveillance de sécurité avec Wazuh.
- Le cycle de traitement des tickets dans GLPI.

## 7. Environnement technique

Windows Server, Ubuntu Server, Active Directory, DNS, DHCP, GLPI, Zabbix, Wazuh, VyOS, VMware Workstation et VirtualBox.

## 8. Nature du projet

AFRITECH est un laboratoire personnel d'apprentissage et de validation technique. Les configurations, schémas, procédures et résultats de tests seront documentés progressivement dans ce dépôt.

---

**AFRITECH – Apprendre, construire, sécuriser et documenter.**
