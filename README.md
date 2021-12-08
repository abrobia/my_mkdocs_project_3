# my_mkdocs_project_3

_Aquest és un projecte de test usant Mkdocs:_ https://abrobia.github.io/my_mkdocs_project_3  

## Instalació Mkdocs

Instal·lem Mkdocs a la nostra màquina

```
$ pip install mkdocs
```  

## Creació inicial del projecte

Creem una carpeta on incloure els arxius del projecte. En aquest cas el projecte s'anomena "my_mkdocs_project_3"

```
$ mkdocs new my_mkdocs_project_3
$ cd my_mkdocs_project_3
```

## Inicialització del servidor virtual

```
$ mkdocs serve
```

I obrim http://127.0.0.1:8000 per veure el nostre projecte local des del navegador  

## Configuració del projecte

Creem les pàgines .md de contingut

Escollim un theme: material    

## Publicació de la web amb GitHub pages

Creem un repo buit a GitHub per hostetjar al nostre projecte. Es recomana que el nom del repositori sigui igual al nom de projecte al nostre ordinador. Aquí és on pujarem el nostre projecte emmagatzemat a l'ordinador fent servir Git.  

Mitjançant el terminal, ens situem dins de la carpeta del projecte local ("my_mkdocs_project_3") que conté els arxius que pujarem i a continuació executem:

```
$ python -m mkdocs build
```

Inicialitzem el nostre repositori local i fem el nostre primer commit amb les següents ordres:

```
$ git init

$ site/ > .gitignore

$ git add .

$ git commit -m "first commit"

$ git branch -M main

$ git remote add origin https://github.com/abrobia/my_mkdocs_project_3.git

$ git push -u origin main

$ mkdocs gh-deploy

```

_Your documentation should shortly be available at:_ https://abrobia.github.io/my_mkdocs_project_3/

