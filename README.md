# my_mkdocs_project_3

Aquest és un projecte de test usant [Mkdocs](https://www.mkdocs.org/)     

El projecte està accessible a: https://abrobia.github.io/my_mkdocs_project_3  

## Instal·lació Mkdocs

Instal·lem Mkdocs al nostre ordinador.

```
$ pip install mkdocs
```  

## Creació inicial del projecte

Creem una carpeta on incloure els arxius del projecte. En aquest cas el projecte s'anomena "my_mkdocs_project_3".

```
$ mkdocs new my_mkdocs_project_3
$ cd my_mkdocs_project_3
```  

## Inicialització del servidor virtual

Iniciem el servidor Mkdocs a partir de la següent comanda:

```
$ mkdocs serve
```

I obrim http://127.0.0.1:8000 per veure el nostre projecte local des del navegador.    

## Configuració del projecte

Creem les pàgines .md de contingut

Escollim un [theme](https://www.mkdocs.org/user-guide/choosing-your-theme/)  

## Publicació de la web amb GitHub pages

Creem un repo buit a GitHub per hostetjar el nostre projecte. Es recomana que el nom del repositori sigui igual al nom de projecte al nostre ordinador. 
Aquí és on pujarem el nostre projecte emmagatzemat a l'ordinador fent servir Git.  

Mitjançant el terminal, ens situem dins de la carpeta local ("my_mkdocs_project_3") que conté els arxius que pujarem i a continuació executem:

```
$ python -m mkdocs build
```

Inicialitzem el repositori local i fem el nostre primer commit amb les següents ordres:

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

Si tot ha anat bé, la consola mostrarà el següent missatge:

_Your documentation should shortly be available at:_ https://abrobia.github.io/my_mkdocs_project_3/  

## Actualització del projecte

Si es volen fer canvis en el projecte:

* Creem una nova branch i la clonem des del nostre ordinador (usem SourceTree)
* Fem els canvis que vulguem des de l'editor (usem Visual Studio Code)
* Pujem els canvis a partir de les següents ordres:   
```
$ git add commit "NOM_DEL_COMMIT"
$ git push -u origin update
$ mkdocs gh-deploy
```  
De nou, si tot ha anat bé, la consola mostrarà el següent missatge:

_Your documentation should shortly be available at:_ https://abrobia.github.io/my_mkdocs_project_3/  


