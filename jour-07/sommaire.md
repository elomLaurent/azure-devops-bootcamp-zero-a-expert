# Cours Pratique : Serveur Bastion avec accès Internet pour VM privée via NAT Gateway

## Sommaire

1. [Objectifs et architecture](#1-objectifs-et-architecture)
2. [Prérequis](#2-prérequis)
3. [Création du groupe de ressources](#3-création-du-groupe-de-ressources)
4. [Création du réseau virtuel (VNet) et des sous-réseaux](#4-création-du-réseau-virtuel-vnet-et-des-sous-réseaux)
5. [Création et configuration du groupe de sécurité réseau (NSG) unique](#5-création-et-configuration-du-groupe-de-sécurité-réseau-nsg-unique)
6. [Création des machines virtuelles](#6-création-des-machines-virtuelles)
   - 6.1 VM publique (bastion)
   - 6.2 VM privée
7. [Installation de Nginx sur la VM publique](#7-installation-de-nginx-sur-la-vm-publique)
8. [Connexion à la VM privée via la VM publique (transfert de clé SSH)](#8-connexion-à-la-vm-privée-via-la-vm-publique-transfert-de-clé-ssh)
9. [Problème d’accès Internet sur la VM privée](#9-problème-daccès-internet-sur-la-vm-privée)
10. [Mise en place d’une NAT Gateway pour le subnet privé](#10-mise-en-place-dune-nat-gateway-pour-le-subnet-privé)
11. [Vérification de l’accès Internet sur la VM privée](#11-vérification-de-laccès-internet-sur-la-vm-privée)
12. [Nettoyage des ressources](#12-nettoyage-des-ressources)
13. [Conclusion et bonnes pratiques](#13-conclusion-et-bonnes-pratiques)
