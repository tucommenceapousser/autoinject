# AutoInject

Outil automatique pour l'analyse des ports et des services avec Nmap, ainsi que pour les tests d'injection SQL avec SQLmap.

C'est la solution parfaite si vous souhaitez centraliser ces outils dans une seule application, et si vous voulez que vos scans Nmap soient affichés de manière plus visuelle.

Développé par trhacknon.

![autoinject](https://github.com/afsh4ck/autoinject/assets/132138425/330a7d75-1608-484f-93ab-af6f069b9cca)

## Injection SQL

L'injection SQL est une technique utilisée par les pirates informatiques pour exploiter les failles de sécurité dans les applications web qui interagissent avec des bases de données. En injectant du code SQL malveillant dans les champs de saisie des formulaires ou dans les paramètres des URL, les attaquants peuvent manipuler les requêtes SQL de l'application pour obtenir des informations sensibles, modifier ou supprimer des données, voire prendre le contrôle complet du système.

## Fonctionnement du script

Ce script combine les fonctionnalités de deux outils populaires : Nmap et SQLmap. 

- **Nmap** est un scanner de ports open source qui permet de découvrir les hôtes et les services actifs sur un réseau.
- **SQLmap** est un outil automatisé pour détecter et exploiter les failles d'injection SQL dans les applications web.

Ce script automatise le processus d'analyse des ports avec Nmap et de test d'injection SQL avec SQLmap, offrant ainsi une solution pratique pour évaluer la sécurité des applications web.

## Installation

1. Clonez le dépôt :
    ```
    git clone https://github.com/tucommenceapousser/autoinject
    ```

2. Accédez au répertoire cloné :
    ```
    cd autoinject
    ```

3. Installez les dépendances requises :
    ```
    pip install -r requirements.txt
    ```

4. Donnez les permissions d'exécution au fichier autoinject.py :
    ```
    sudo chmod 777 autoinject.py
    ```

5. Lancez l'outil :
    ```
    python3 autoinject.py
    ```

## Options

- **Tor**: Utilisez le réseau Tor pour les requêtes effectuées par SQLmap.
- **Risk**: Déterminez le niveau de risque des tests effectués par SQLmap (1 à 3).
- **Level**: Définissez le niveau de profondeur des tests effectués par SQLmap (1 à 5).
- **Random-Agent**: Choisissez aléatoirement un agent utilisateur pour chaque requête HTTP envoyée par SQLmap.

En utilisant ces options, vous pouvez personnaliser et ajuster le comportement de SQLmap selon vos besoins et les exigences de votre test d'injection SQL.

## Support

Si vous trouvez cet outil utile, vous pouvez me soutenir en m'offrant un café !

<a href="https://www.buymeacoffee.com/trhacknon" rel="nofollow"><img width="250" alt="buymeacoffe" src="https://camo.githubusercontent.com/cd9a722712fec4278ef95ff114b458897a37a52ef8129b6c833efcf8c66e2211/68747470733a2f2f63646e2e6275796d6561636f666665652e636f6d2f627574746f6e732f76322f64656661756c742d6f72616e67652e706e67" data-canonical-src="https://cdn.buymeacoffee.com/buttons/v2/default-orange.png" style="max-width: 100%;"></a>

## Exécutez sur Replit

[![Run on Repl.it](https://repl.it/badge/github/tucommenceapousser/autoinject)](https://repl.it/github/tucommenceapousser/autoinject)
