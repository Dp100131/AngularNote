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

dir -> app.module.ts -> Se incluye el paquete
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
```
    import { FormsModule } from '@angular/forms';


    @NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule,
    FormsModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

## *ngIf
```
<p *ngIf="person.name == 'daniel' ">
```
se puede complicar la lógica dentro de las "" tanto como se requiera.
```
<h1>*ngIf</h1>
<input type="text" [(ngModel)]="person.name">
<p *ngIf="person.name == 'daniel'; else elseBlock">
  Acertó.
</p>
<ng-template #elseBlock>
  <p>Bloque else</p>
</ng-template>

```