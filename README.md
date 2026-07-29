![logo](Ressources/Logo.png)

## 📖 Présentation du projet
Nginx Proxy Manager (NPM) est une interface graphique open-source conçue pour simplifier la gestion des reverse proxys basés sur Nginx et des certificats SSL.  
Ce projet consiste en le déploiement de ce reverse proxy dans un conteneur LXC sous Proxmox VE.   


## 🎯 Objectifs
- **Sécuriser** l'accès au différents services (Home Assistant, Vaultwarden, Proxmox, et autres) avec des certificats SSL Let's Encrypt.   
- **Simplifier** les accès via un nom de domaine plutôt que par adresse IP.
- **Centraliser** sous un domaine personnalisé (ici `*.azortix-local.duckdns.org`) divers services.
 


## Type d'infrastructure
- **Version de Proxmox utilisée** : 9.1.4
- **Conteneur :** Nginx Proxy Manager (Image officielle via Docker ou script de déploiement LXC).
- **Image Docker** : jc21/nginx-proxy-manager  
- **DNS :** DuckDNS.  
- **Adresse IP** : 192.168.1.90
- **Port** : 81


## 🛠️ Ce que j'ai appris
- **Virtualisation & Conteneurs :** Déploiement et configuration d'un conteneur LXC sous Proxmox (allocation de ressources, réseau).  
- **DNS :** Gestion des enregistrements DNS avec DuckDNS.   
- **Sécurité Web :** Mise en place de certificats SSL Wildcard (`*.domaine`), utilisation de Let's Encrypt.  
- **Nginx :** Compréhension du rôle d'un reverse proxy pour router le trafic HTTPS vers des services HTTP/HTTPS internes. 

## 🔄 Améliorations futures
- Prendre un nom de domaine plus simple
- Permettre l'accès aux services depuis internet de manière sécurisée
