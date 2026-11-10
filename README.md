# Poste client Windows et accès à un NAS TrueNAS

Installation d'un poste client Windows 10 Entreprise et intégration à un réseau local avec accès aux partages d'un serveur de stockage TrueNAS.

Mini-projet de formation : la configuration a d'abord été validée en environnement virtuel avant l'installation physique chez le client.

## Environnement

| Élément | Détail |
| --- | --- |
| Poste client | Windows 10 Entreprise (version d'évaluation), en machine virtuelle |
| Serveur de stockage | TrueNAS, accessible via `truenas.local` et `192.168.1.17` |
| Réseau | Accès par pont sur les deux machines |
| Virtualisation | VirtualBox |

## Démarche

### 1. Préparation du poste client

Installation de Windows 10 Entreprise sur une machine virtuelle, puis configuration du réseau en mode pont pour placer le poste sur le même segment que le NAS.

### 2. Connexion au NAS

- Vérification de la configuration réseau du NAS
- Connexion par nom de domaine local (`truenas.local`) puis par adresse IP, pour valider la résolution de noms
- Accès aux dossiers partagés depuis l'explorateur de fichiers Windows
- Test de lecture et d'écriture dans un dossier utilisateur dédié

### 3. Validation

Captures d'écran de l'accès aux partages depuis l'explorateur Windows et de l'interface d'administration de TrueNAS.

## Compétences mises en œuvre

Installation et configuration d'un poste Windows · partages réseau SMB · résolution de noms sur réseau local · administration de base d'un NAS TrueNAS · validation en environnement virtuel avant déploiement

## Note

Les machines virtuelles ne sont pas distribuées ici : les exports dépassent la limite de taille de GitHub. Le dépôt documente la démarche et la configuration.
