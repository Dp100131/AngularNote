# Inicializar

- ng new NOMBRE_APP || Crear proyecto
- ng serve || Inicializar proyecto
- ng serve -o || Abrir en el navegador automáticamente
- ng serve -o --port-3500 || Elegir un ppuerto

## Estructura de un proyecto en Angular

### src

- El corazón de toda la app.

### .browawerslistrc

    - Indica a angular en que versiones debe ser compatible la app, recomendable dejarlo como está.
### .editorconfig

    - pluging editor config (Herramientas para desarrollar en equipo).

### .tsconfig

    - configuración de typeScript en angular.

### Angular.json

    - Configuración de compilación de angular.

### .nvmrc

    - Ayuda por si estás trabajando en diferentes versiones de node.

## Conceptos basicos de typeScript

    - Ver el archivo recap.ts ubicadodo en la carpeta src del repositorio [Curso de Fundamendos de Angular](https://github.com/Dp100131/Curso_de_fundamentos_Angular).

## String Interpolation
    - {{ 1 + 1}}
    - {{ myVar }}
    - {{ myFunction }}
    - Las variables deben ser public para que se puedan utilzar en el html.

## Property [ Binding ]

    - <button [disabled]="btnDisabled">Enviar</button>

## Event Binding

<button (click)="toggleButton()">Toggle button</button>

### Eventos
    - (scroll)
    - (click)
    - Se envía los eventos nativos con $event

### Data [(Biding)]