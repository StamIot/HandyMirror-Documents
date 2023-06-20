# HANDY MIRROR - Règles

![Logo](https://github.com/StamIot/HandyMirror-Documents/blob/feature/updateStructure/logo/HM.jpg)

## Fourniture physique pour mener à bien le projet IOT

-   [x] Vitre ou plexiglas sans tain
-   [x] Un écran LCD (HDMI 2.0)
-   [x] Utiliser le Raspberry PI Model 4
-   [x] Communiquer avec un serveur distant sous (Linux - Raspbian)

## Outils afin de réaliser à bien le projet IOT

-   [x] Visual Studio Code, JetBrains (PhpStorm), GitHub CodeSpaces.
    -   [x] **Alain** : Visual Studio Code
    -   [x] **Zeinab** : JetBrains (PhpStorm) | Visual Studio Code
    -   [x] **Sophie** : Visual Studio Code
    -   [x] **Tarek** : Visual Studio Code
-   [ ] Consommation de plusieurs services (API)

## Les technologies à utiliser pour HandyMirror (Fil rouge)

![Logo](https://github.com/stamiot/HandyMirror-Documents/blob/main/screenshots/Technologies_used.png)

-   [ ] Micro Services éventuels ( technologies libre )

## Important

```diff
- Chaque membre de l'équipe doit impérativement suivre les étapes ci-dessous
- afin de mener à bien ce projet dans des conditions optimal.
```

### 1 - Cloner le repository

```sh
# Tu devras cloner la branche develop du repository sur lequel tu es amenez à travailler.
git clone https://URL_DE_LA_BRANCHE_QUE_TU_AS_COPIE
```

### 2 - Se rendre dans le repository fraîchement récupérer

```sh
# Une fois le clone effectuer tu devras te déplacer dans le répertoire de travaille.
cd NOM_DU_PROJET
```

### 3 - Créer sa branche selon quelques règles

> Tu devras des branches spécifiques qui seront amener à être supprimer avec le temps que si elle ne nécessite plus d'intervention des membres du projet.

ci-dessous se trouve les règles suivi d'un exemple.

#### 3.1 - Règles de nommage des branches

-   **feature/createLoginForm**
    -   _La branche qui te permettra de créer une nouvelle fonctionnalité_
-   **patch/createLoginForm**
    -   _Cette branche te servira au cas où si tu as un bug non critique à corriger rapidement_
-   **hotfix/createLoginForm**
    -   _Cette branche te servira au cas où si tu as un bug critique à corriger urgemment_
-   **test/createLoginForm**
    -   _Cette branche te servira pour tester la compatibilité avec la branche develop_

#### 3.2 - Exemple sur l'utilisation des branches

```sh
# Ajout d'une nouvelle feature (exemple)
git checkout -b feature/loginForm

# Correction de la feature login form qui comporte un bug critique
git checkout -b hotfix/loginForm

# Correction d'un problème mineur sur la feature login form
git checkout -b patch.loginForm

# Test d'une futur migration vers la branche develop
git checkout -b test/loginForm
```

### 4 - Respecter la syntaxe des commits

> **Tu dois prendre en considération qu'il y a une syntaxe a respecter pour les commits**.
> c'est volontaire pour une meilleure gestion du projet.
> On gagnera du temps dur une pull request

```diff
- Attention

- Aucun commit ne seras écrit avec des majuscules, tout seras en minuscule
- à l'exception du nom d'une classe
- On va se forcer à garder nos README en Français,
- mais l'intégralité du code ainsi que des commits seront eux en ANGLAIS
```

#### 4.1 - Exemple d'un commit

```sh
# Ajout d'une nouvelle feature (exemple)
git commit -m "feature: login form" -m "create a login form for the e-commerce"

# Correction de la feature login form qui comporte un bug critique
git commit -m "hotfix: login form" -m "fix a submit button"

# Correction d'un problème mineur sur la feature login form
git commit -m "patch: login form" -m "path text for name label"

# Test d'une futur migration vers la branche develop
git commit -m "test: login form" -m "test of feature before merge to develop branch"
```

#### 4.2 - Explication des deux -m

```sh
# Voici ce que signifie précisément les deux -m
git commit -m "Titre du commit" -m "Contenu du commit"
```

```diff
+ Information utile
+ si tu as bien respecter le commit précédent, alors,
+ tu n'auras rien à modifier sur ton commit de ta futur pull request.
```

### 5 - Création de la pull request

Une fois que tout te semble OK, tu peux te rendre sur le projet, il te faudra cliquer sur l'onglet **pull request** où tu verras que tu as une pull request à faire.
Une fois que celle-ci sera faîte, alors il ne te restera plus qu'à la soumettre.
En effet l'étape 4 aura été directement implémenter via l'étape grâce à l'étape 3.

Quelques subtilités:

-   [x] pense à ajouter les 2 personnes qui feront la review
-   [x] Ajoute des tags qui sont censé correspondre à ce que tu fais
-   [x] Attribue toi le projet
-   [x] Enfin soumet la pull request et patiente pour la review de code.

### 6 - Attendre une review

_En attendant va travailler sur une autre étape du projet_

Sache qu'il te faudra attendre une review de deux collaborateur afin de valider où non celle-ci.
Une fois validé, le product owner se concertera avec les scrums master afin de merger la pull request vers la branche **main**
