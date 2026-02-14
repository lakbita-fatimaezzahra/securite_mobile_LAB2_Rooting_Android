# securite_mobile_LAB2_Rooting_Android

 #Étape 1 : Rooter l'AVD
 
<img width="1223" height="320" alt="image" src="https://github.com/user-attachments/assets/c5819347-08ee-4e6a-9921-fc23c9b48eb9" />

   Vérifications :
   
<img width="1700" height="417" alt="image" src="https://github.com/user-attachments/assets/2ff55a60-a4ec-4bcf-b08d-ad00e01c3671" />

<img width="828" height="624" alt="image" src="https://github.com/user-attachments/assets/276c6245-44c6-4ebc-8155-2f6432910f58" />

  Journalisation :
  
<img width="1461" height="125" alt="image" src="https://github.com/user-attachments/assets/9f5d4c79-d7d5-4037-888f-9442521ff0a5" />

<img width="1409" height="664" alt="image" src="https://github.com/user-attachments/assets/d01c58ce-aded-40dd-9e38-4e29c082775b" />


Étape 2 : Fiche périmètre 

#Fiche périmètre

Application / Version : Android Emulator Pixel 6 – Android 16 (API 36)

Support : AVD (Android Virtual Device – environnement de laboratoire)

Objectif : Comprendre rooting et impacts sur le système et les mécanismes d’intégrité

Données : Fictives (aucune donnée réelle ou personnelle)

Réseau : Test (réseau isolé, aucune connexion internet réelle)


Étape 3 : Démarrer un AVD propre

<img width="719" height="984" alt="image" src="https://github.com/user-attachments/assets/f2452541-5730-4073-aaad-a2eb988c6df3" />

<img width="1784" height="758" alt="image" src="https://github.com/user-attachments/assets/795ca972-6b62-4278-a9a5-598945b3ac4c" />

Étape 4 : Installer et lancer l'app de test

Installer et lancer l'app de test

<img width="1504" height="126" alt="image" src="https://github.com/user-attachments/assets/337fd166-64e5-489a-ab41-aea3871f65dc" />

Vérifier que l'application s'ouvre et qu'un scénario simple est réalisable. Noter la version de l'application dans le rapport.

<img width="513" height="122" alt="image" src="https://github.com/user-attachments/assets/53c65a2c-47d6-4638-a6cc-7fe103f82b29" />

clique button *next*

<img width="527" height="809" alt="image" src="https://github.com/user-attachments/assets/3e0ebdd3-751e-471c-90e7-0258d79fce85" />
 
clique button *previous*

<img width="348" height="767" alt="image" src="https://github.com/user-attachments/assets/e5e9017f-0f3b-455c-bf51-c87f5dd92c5e" />

Étape 5 : Définir 3 scénarios simples


Étape 6 : Lire Android Security 

Android utilise plusieurs couches de sécurité : chaque application est isolée dans un sandbox, empêchant l’accès aux données des autres apps. Le modèle de permissions contrôle l’accès aux ressources sensibles comme le micro, la caméra ou les fichiers. L’intégrité du système protège contre les modifications non autorisées. Le sandboxing, c’est comme mettre chaque appli dans sa propre salle de classe fermée. Les permissions, c’est demander l’autorisation au professeur avant d’utiliser un équipement. L’intégrité système, c’est verrouiller le bâtiment entier pour sécuriser sa structure.


Étape 7 : Verified Boot (idée générale + check AVD)

Objectif principal : Garantir que le système qui démarre est celui prévu par le fabricant, sans modifications malveillantes.

Concept simplifié : Verified Boot est comme un système d’alarme qui vérifie si quelqu’un a changé les serrures ou portes de votre maison. Si oui, il alerte ou refuse de démarrer.

Chain of trust (2 lignes) : Chaque composant vérifie l’authenticité du suivant avant de lui faire confiance. Comme une chaîne de gardiens où chacun vérifie l’identité du suivant.

Pourquoi c’est critique : Si le démarrage est compromis, toutes les protections suivantes peuvent être contournées, comme une forteresse dont la porte principale serait ouverte.

Commande pour vérifier sur AVD :
<img width="958" height="210" alt="image" src="https://github.com/user-attachments/assets/f10310fd-0af7-436d-81b0-15b4c7bbe207" />

Étape 8 : AVB (Android Verified Boot)

Android Verified Boot (AVB) ajoute une vérification d’intégrité moderne à chaque démarrage, garantissant que les composants système n’ont pas été modifiés.
Il protège également contre le rollback, empêchant le retour à une version plus ancienne vulnérable du système.
Ainsi, AVB renforce la sécurité globale et la confiance dans le démarrage du dispositif.

Étape 9 : Définir le rooting 

Le rooting permet d’obtenir des privilèges super-utilisateur sur Android, donnant un contrôle complet sur le système.
Cela modifie les protections et la confiance du système, ce qui peut compromettre la sécurité si mal utilisé.
Utile en laboratoire pour observer certains comportements, il reste risqué, et nécessite isolement, traçabilité et possibilité de remise à zéro.
Le rooting, c’est comme avoir un passe-partout pour toutes les portes d’un bâtiment : très pratique pour le personnel de maintenance, mais dangereux si le passe tombe entre de mauvaises mains.

Étape 10 : Intérêt en laboratoire (non opérationnel)

En labo, un environnement privilégié peut aider à : voir des données normalement invisibles, observer comment l’application fonctionne à bas niveau, et tester la sécurité du stockage.
Exemple : Avec les droits root, on peut vérifier si une application chiffre correctement ses données sensibles.
 #À faire uniquement en labo autorisé.
Le rooting peut être interdit par le fabricant ou la loi, donc toujours avoir l’autorisation avant de tester.






