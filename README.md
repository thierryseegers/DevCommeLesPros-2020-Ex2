# ProgImpAv-2020-Ex2
Modèle de départ pour exercices d'introduction au makefile, à une structure de projet et aux bibliothèques logicielles.


## Instructions de départ

Ces intructions présupposent que vous avez déjà suivi les instructions de l'[exercice précédent](https://github.com/thierryseegers/ProgImpAv-2020-Ex1) pour la création de compte et l'installation des programmes et eextensions nécéssaires.

1. Créez votre dépôt sur github.com en utilisant ce dépôt-ci (https://github.com/thierryseegers/ProgImpAv-2020-Ex2) comme modèle.
    - Suivez ces instructions: https://help.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template.
    - Choisissez l'option `Private` à l'étape 5.
1. Ajoutez le professeur comme collaborateur à votre dépôt.
    - Suivez ces instructions: https://help.github.com/en/github/setting-up-and-managing-your-github-user-account/inviting-collaborators-to-a-personal-repository
        - Nom d'utilisateur à ajouter: `thierryseegers`.
1. Clonez votre dépôt vers votre espace de travail local.
    - Suivez ces instructions: https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository
    - Attention à ne pas cloner https://github.com/thierryseegers/ProgImpAv-2020-Ex2 mais bien votre dépôt nouvellement créé.
1. Lancez Visual Studio Code.
    - À l'invite de commandes:
        - `> cd [nom de votre dépôt]`
        - `> code .`
1. Compilez une première fois le programme.
    - Menu: `View` > `Command Palette` > `Tasks: Run Build Task`
1. Vous devriez observer dans l'onglet `TERMINAL` le résultat suivant:
    - Sous Linux: 
        - `collect2: error: ld returned 1 exit status`
    - Sous MacOS: 
        - `clang: error: linker command failed with exit code 1`


## Objectif principal

1. Réparez le fichier `makefile` pour faire en sorte que la bibliothèque `libchiffrage.a` contienne tous les fichiers objets nécéssaires (fussent-ils eux-même incomplets) et que le programme `test` puisse être correctment lié et lancé.
1. Implémentez correctement toutes les fonctions de chiffrages (à l'exception de `chiffre_Vigenere_flux_binaire` et `dechiffre_Vigenere_flux_binaire`) pour que le programme `test` retourne `0`.

Il vous est permis: 
- De modifier le fichier `makefile`.
- De modifier les fichiers `lib/ROT13.c`, `lib/Cesar.c` et `lib/Vigenere.c` afin d'implémenter les fonctions qu'ils contiennent.

Il ne vous est pas permis:
- De modifier le fichier `test/main.c`.
- De modifier les fichiers d'entête `lib/ROT13.h`, `lib/Cesar.h`, `lib/Vigenere.h` et `lib/chiffrage.h`.

