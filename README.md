# HANDY MIRROR - Règles

![Logo](https://github.com/alain-guillon-it/HandyMirror-Documents/blob/main/logo/HM.jpg)

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
-   [ ] -   [] Consommation de plusieurs services (API)

## Les technologies à utiliser pour HandyMirror (Fil rouge)

![Logo](https://github.com/alain-guillon-it/HandyMirror-Documents/blob/main/screenshots/Technologies_used.png)

-   Micro Services éventuels ( technologies libre )

## Important

```diff
- Chaque membre de l'équipe doit impérativement suivre les étapes ci-dessous afin de mener à bien ce projet dans des conditions optimal.
```

1. Chaque membre de l'équipe devra cloner la branche **develop** du repository sur lequel vous êtes amenez à travailler.
2. A partir de là, vous devrez créer des branches spécifiques qui seront amener à être supprimer avec le temps avec quelques règles de nommage à respecter avec un exemple:
    - **feature/createLoginForm** _La branche qui te permettra de créer une nouvelle fonctionnalité_
    - **patch/createLoginForm** _Cette branche te servira au cas où si tu as un bug non critique à corriger rapidement_
    - **hotfix/createLoginForm** _Cette branche te servira au cas où si tu as un bug critique à corriger urgemment_
    - **test/createLoginForm** _Cette branche te servira pour tester la compatibilité avec la branche develop_
3. **Respecter la syntaxe pour les commits** pour une meilleure gestion du projet, voir un exemple juste après.
4. Une fois que toutes les étapes sont respectés, alors il te faut créer une **PR** (_Pull Request_) et si le commit précédent a bien été respecter alors il n'y aura rien à modifier sur le commit de la pull request.
5. Il faudra attendre une review de deux collaborateur afin de valider où non celle-ci.
6. Une fois validé, le product owner se concertera avec les scrums master afin de merger la pull_request vers la branche **main**

## Normalisation des commits

Cette section est super importante pour garder des commits sains et propres.
**Attention, aucun commit ne seras écrit avec des majuscules, tout seras en minuscule à l'exception du nom d'une classe**
**On va se forcer à garder des README en Français, mais l'intégralité du code ainsi que des commits seront en ANGLAIS**

```sh
# Ajout d'une nouvelle feature (exemple)
git commit -m "feature: login form" -m "create a login form for the e-commerce"

# Correction d'une feature critique avec un bug
git commit -m "hotfix: login form" -m "fix a submit button"

# Correction d'un problème mineur
git commit -m "patch: login form" -m "path text for name label"

# Test de plusieurs changements à venir
git commit -m "test: login form" -m "test of feature before merge to develop branch"
```
