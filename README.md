# Jajivetotal

## Récupérer les API keys dans PassiveTotal

* Se connecter sur PassiveTotal
* Account Settings
* Cliquer sur show a cote de User dans la catégorie API

## Renseigner les API Keys

Dans le fichier jajivetotal.py :

```
credentials = {
  "USERNAME": ['email1', 
  			   'email2', 
  			   'email3'],

  "API_KEY": ['email1_key',
              'email2_key', 
              'email3_key'],
}
```
Remplacer par un ou plusieurs compte.

## Utilisation

```
python jajivetotal.py DOMAINE_DE_DEPART
```

## Explications

En partant d un domaine, Jajivetotal va recuperer le mail aillant enregistre ce domaine pour ensuite faire une recherche par rapport a ce mail. Une fois tout les domaines du mail recuperer, Jajivetotal va recuperer les sous-domaines.

Par la suite, un fichier CSV et XLSX seront generes avec une colonne Domaine et une colonne IP. Les domaines aillant la meme IP seront rassemble
