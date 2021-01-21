# bootstrap4-theming-test
 Provant el theming de Bootstrap4 amb SCSS

## Com fer-ho
### 1. Instal·lar bootstrap
A la carpeta del projecte, instal·lar Bs amb:

    > npm install bootstrap

### 2. Seguir les instruccions [aqui](https://getbootstrap.com/docs/4.4/getting-started/theming/)
- Crear la carpeta `scss` i el fitxer `custom.scss` a dins.
- Importar a `custom.scss` els fitxers de scss de Bootstrap (no els de css, que estan a dins de dist/ i són els que empram quan utilitzam Bootstrap de la forma acostumada)
- Compilar el fitxer `.scss` amb *Koala* o l'extensió _Live Sass Compiler_ de VSC 

Un cop fet això, ja puc modificar qualsevol classe de Bootstrap i fer _overrride_ a sobre.

## Don't forget the links to the 3 JS libraries of Bootstrap!
https://getbootstrap.com/docs/4.4/getting-started/introduction/#js

## More about Bootstrap Customization
https://uxplanet.org/how-to-customize-bootstrap-b8078a011203

## gitignore
En treballar amb Theming, no inclourem els fitxers de la carpeta `node_modules` en el repo. Per això, inclourem aquesta linia en el fitxer `.gitigonre`:

    /node_modules
