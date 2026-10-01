# NEXUS — Téléchargements

Client Windows x64 pour échanger en texte, voix, vidéo et partage d’écran.

[Télécharger la dernière version](https://github.com/Zastaxx/nexus-releases/releases/latest)

Ce dépôt public contient les installateurs, leurs signatures Tauri, le manifeste latest.json et les empreintes SHA-256. Le code source est conservé dans un dépôt privé.

La version 0.3.0 propose un chat central, les salons à gauche, les amis à droite, des participants sous les vocaux, des paramètres centralisés et une inscription avec email et confirmation du mot de passe. Les messages sont enregistrés sur le serveur. L’interface conserve l’identité crème, sauge et vert forêt de NEXUS, avec un thème nocturne et des panneaux adaptés aux petites fenêtres.

Installez le fichier NEXUS_*_x64-setup.exe. Le client vérifie les nouvelles versions au démarrage et chaque heure, puis propose leur installation hors appel. Chaque mise à jour est vérifiée avec la clé publique embarquée.

Le serveur NEXUS doit être mis à jour en 0.3.0 avec LiveKit. L’API locale par défaut est http://localhost:3000 ; une API distante HTTPS peut être choisie dans Paramètres → Connexion après déconnexion. Ce dépôt ne déploie pas de serveur public.

Les signatures de mise à jour Tauri sont fournies. Aucun certificat Windows Authenticode d’éditeur n’est configuré.
