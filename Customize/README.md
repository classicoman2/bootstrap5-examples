# bootstrap4-theming-test
 Provant el [theming de Bootstrap 4](https://getbootstrap.com/docs/4.4/getting-started/theming/) amb SCSS

## Com fer-ho
### 1. Instal·lar bootstrap
A la carpeta del projecte, instal·lar Bs amb:
```bash
npm install --save-dev bootstrap
```

### 2. Instal·lar sass
```bash
npm i --save-dev sass
```

### 3. Configurar custom.scss
- Crear la carpeta `scss` i el crear fitxer `custom.scss` a dins
- Importar a `custom.scss` els fitxers de scss de Bootstrap (no els de css) tal i com s'explica a l'apartat _Theming_ de _GetBootstrap_

### 4. Compilar el SCSS
Compilar una vegada,
```bash
npm run sass
```

Compilar en mode _watch_,
```bash
npm run sass-watch
```

### 5. Modificar variables i mapes per defecte

Escrivim a dalt de tot de `custom.scss` les classes que volem canviar (colors, mides, etc.)

Exemples, 
```css
/* 1. Modificar variables (variable overrrides) */
$primary: magenta;
$body-bg: #000;

/* 2. Maps (afegir un color a primary, secondary, danger.......) */
$theme-colors: (
  "elmeucolor": #900
);
```

Trobaràs la llista completa de variables dins la carpeta Bootstrap, a `scss/variables.scss`



## Llibreries js

Podem linkar les llibreries de js que necessita Bootstrap des dels CDN o bé en local, i podem prescindir d'alguna elles si el nostre codi no la necessita.

https://getbootstrap.com/docs/4.4/getting-started/introduction/#js

## More about Bootstrap Customization
https://uxplanet.org/how-to-customize-bootstrap-b8078a011203

## gitignore
En treballar amb Theming a Github, no inclourem els fitxers de la carpeta `node_modules` en el repo. Per això, inclourem la linia `node_modules` en el `.gitignore`
