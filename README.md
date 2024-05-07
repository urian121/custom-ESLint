# Mi Custom ESLint

##### Agregar cualquiera de estas dos opciones en la parte final del archivo '.eslintrc' que está al nivel del proyecto, con esta configuración perzonalizada nos permitirá desactivar la regla "react/prop-types" para todos los archivos con extensión .js y .jsx en el proyecto.

##### La regla "react/prop-types" es una regla proporcionada por ESLint que verifica si los componentes de React tienen definidos los tipos de sus props mediante PropTypes. Al desactivar esta regla con "off", estás indicando que no deseas que ESLint te advierta sobre la ausencia de definiciones de PropTypes en tus componentes de React

##### Opción 1

    overrides: [
        {
          files: ["*.js", "*.jsx"],
            rules: {
            "react/prop-types": "off",
            },
        },
    ],

##### Opción 2

    "eslint.validate": [
      "javascript",
      "javascriptreact",
      { "language": "javascript", "autoFix": true },
      { "language": "javascriptreact", "autoFix": true }
    ],
