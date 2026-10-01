# NEXUS — Téléchargements

Client Windows x64 pour se retrouver en voix, vidéo et partage d’écran.

[Télécharger la dernière version](https://github.com/Zastaxx/nexus-releases/releases/latest)

Ce dépôt public contient uniquement les installateurs, leurs signatures de mise à jour, le manifeste latest.json et les empreintes SHA-256. Le code source est conservé dans un dépôt privé.

Installez le fichier NEXUS_*_x64-setup.exe. Le client vérifie les nouvelles versions au démarrage et toutes les heures, puis propose leur installation. Chaque mise à jour est vérifiée avec la clé publique embarquée dans l’application.

La version 0.2.0 nécessite un serveur NEXUS et LiveKit ; la configuration fournie cible localhost. Ce dépôt ne fournit pas de serveur public.

Les mises à jour portent une signature Tauri. Aucun certificat Windows Authenticode d’éditeur n’est configuré pour cette version.
