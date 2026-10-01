# NEXUS — téléchargements Windows

**[Télécharger NEXUS 0.4.1](https://github.com/Zastaxx/nexus-releases/releases/download/v0.4.1/NEXUS_0.4.1_x64-setup.exe)** · [Notes de version](https://github.com/Zastaxx/nexus-releases/releases/tag/v0.4.1)

NEXUS permet de se retrouver en voix, vidéo et partage d’écran. Son identité visuelle mêle crème, sauge et vert forêt, avec un thème sombre. Les salons sont à gauche, le chat ou le stream au centre et les amis à droite.

La version 0.4.1 apporte une liste de salons entièrement revue : texte et vocal distincts, catégories obligatoires, glisser-déposer avec aperçu et repères de position, menus et navigation au clavier. Le microphone est ouvert à l’entrée. Les états micro/casque coupés sont affichés en rouge près des pseudos. Les commandes d’appel sont regroupées en bas à gauche. Le lecteur de stream propose agrandissement, plein écran, son individuel et quitter/reprendre.

Le partage Windows utilise un sélecteur NEXUS personnalisé : écran, fenêtre ou application, avec ou sans son, qualité et FPS. La capture image passe par Windows Graphics Capture et le son par WASAPI. Le mode application partage sa fenêtre principale et les fenêtres secondaires prises en charge ; le son de processus demande une version Windows compatible. Les FPS sont une limite dépendante du matériel.

Les paramètres proposent la détection automatique des périphériques et un aperçu webcam ; les changements de caméra et microphone s’appliquent pendant l’appel.

La connexion est obligatoire, avec option « Se souvenir de moi ». Les préférences se sauvegardent automatiquement sur le compte. La suppression d’un compte demande son mot de passe et une confirmation écrite.

## Installer et mettre à jour

L’installateur x64 cible l’utilisateur courant et propose le français ou l’anglais. Les mises à jour Tauri sont signées et vérifiées avec la clé publique du client. Leur recherche est automatique ; l’installation se fait hors appel. Aucun certificat Windows Authenticode d’éditeur n’est configuré.

Le client demande un serveur NEXUS compatible et LiveKit. L’API locale par défaut est `http://localhost:3000`. Avant connexion, **Configurer le serveur** permet de choisir une API distante HTTPS. Le serveur doit aussi être mis à jour pour utiliser les nouvelles fonctions.

Ce dépôt contient les installateurs, signatures et manifestes de mise à jour. Le code source est conservé dans un dépôt privé distinct.

La mise à jour serveur 0.4.1 réinitialise volontairement les anciens salons, catégories et messages en **SALONS → Bienvenue / Salon 1** (textuels). Comptes, sessions et préférences sont conservés. Chaque salon doit appartenir à une catégorie ; supprimer une catégorie occupée exige une catégorie de destination.

Le dépôt de code privé inclut aussi un guide et des scripts pour installer soi-même le serveur sur un VPS Debian/Ubuntu : Docker, PostgreSQL, API Rust, LiveKit, coturn, HTTPS/WSS Caddy et supervision/logs PM2. Le client se connecte à l’adresse HTTPS de ce serveur.
