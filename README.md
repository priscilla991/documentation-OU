
# Documentation - Création d'une Unité d'Organisation, d'un Groupe d'Utilisateurs et d'un Utilisateur dans Active Directory

Cette procédure décrit les étapes nécessaires pour créer une **Unité d'Organisation (OU)**, un **Groupe d'utilisateurs** et un **Utilisateur** dans Active Directory sur le domaine **wilders.lan**.

## 1. Créer une Unité d'Organisation (OU) : **Wilders_students**

1. **Ouvrir la console Active Directory Users and Computers**.
   - Depuis le **Gestionnaire de serveur**, clique sur **Outils** > **Utilisateurs et ordinateurs Active Directory**.

2. **Créer une nouvelle Unité d'Organisation (OU)** :
   - Dans la fenêtre **Utilisateurs et ordinateurs Active Directory**, fais un clic droit sur **wilders.lan** (ou l'arborescence principale de ton domaine).
   - Sélectionne **Nouveau** > **Unité d'organisation**.
   - Dans le champ **Nom**, entre **Wilders_students** pour le nom de l'OU.
   - Clique sur **OK** pour valider.

## 2. Créer un Groupe d'utilisateurs : **Students**

1. **Créer un groupe** :
   - Toujours dans la console **Utilisateurs et ordinateurs Active Directory**, clique droit sur **Wilders_students** (l'OU que tu viens de créer).
   - Sélectionne **Nouveau** > **Groupe**.
   - Dans la fenêtre qui s'ouvre, entre **Students** comme nom du groupe.
   - Choisis le type de groupe : **Groupe global** et la portée : **Sécurisé**.
   - Clique sur **OK** pour valider.

## 3. Créer un Utilisateur : **student01**

1. **Créer un nouvel utilisateur** :
   - Dans l'OU **Wilders_students**, fais un clic droit et choisis **Nouveau** > **Utilisateur**.
   - Remplis les champs suivants :
     - **Prénom** : `Student`
     - **Nom** : `01`
     - **Nom d'ouverture de session** : `student01`
     - **Mot de passe** : entre un mot de passe sécurisé (par exemple `Password123!`).
     - Coche la case **L'utilisateur doit changer le mot de passe à la prochaine ouverture de session** (option facultative).
   - Clique sur **Suivant**, puis sur **Terminer** pour créer l'utilisateur.

2. **Ajouter l'utilisateur au groupe** :
   - Fais un clic droit sur l'utilisateur **student01** dans l'OU **Wilders_students**.
   - Sélectionne **Ajouter au groupe**.
   - Dans la fenêtre qui apparaît, tape **Students** (le nom du groupe) et clique sur **OK**.

## 4. Vérification

1. **Vérifier l'utilisateur et le groupe** :
   - Retourne dans la console **Utilisateurs et ordinateurs Active Directory** et vérifie que l'utilisateur **student01** se trouve bien dans l'OU **Wilders_students**.
   - Assure-toi qu'il est bien ajouté au groupe **Students** en vérifiant les **membres** du groupe **Students**.


**Fin de la documentation.**
