# AngularTourOfHeroes

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.2.3.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

# Notas personales.

Estudio de Angular con angular Cli

1. Angular Cli : Es un generador de código para angular, nos permite crear workspace, componentes, entre otros
    1. ng generate component heroes  “Con el comando anterior creamos un componente con el nombre heroes en angular cli”

 2. Interpolation binding  : Es el nombre que recibe la propiedad de hacer referencia desde el html  a elementos que están en el component mediante  doble llave {{nombre_propiedad}}

3. Pipes: son utilizados para formatear los String que se van a mostrar al front, ejemplo {{hero.name | uppercase}} uppercases es un pipe, ” date, exponentialStrength”
4.  Two-way binding = Se conoce como la propiedad de permitir el flujo de información entre el componente y la pantalla automáticamente
    1. Ejemplo :   <input [(ngModel)]="hero.name" placeholder="name”/>, la propiedad [(ngModel)] es la que  que indica como es el flujo de información Two way binding  entre el componente y la pantalla, en este ejemplo especifico para el campo hero.name.
5.  decorators, utilizados para la metada de la aplicación, ejemplo : @Component, buscar mas sobre estos
6.  Todo componente debe estar declarado en un modulo
7.  Directivas : las directivas en angular son elementos en el HTML que permiten añadir, manipular o eliminar elementos del DOM, ejemplo : ngIf, ngShow, ngFor, ngModel
8. El decorator @Input() se utiliza para marcar una propiedad como parámetro, es decir que dicha propiedad viene desde un componente padre.
9.  property binding  es el nombre que recibe la propiedad de mandar parámetros de un componente a otro ejemplo :  <app-hero-detail [hero]="selectedHero"></app-hero-detail>  el componente héroe-retail debe tener una propiedad hero, que es de tipo Hero y que está marcado con el decorator @input()
10. El decorator @Injectable se utiliza para indicar que una clase se puede inyectar en un componente, utilizado especialmente para los servicios de acceso a data.
11.  Observable es utilizado para remplazar las Promise o los callBack, son utilizados en los servicios para esperar respuesta del back, en los componentes cuando se usa un método de un servicio que retorna un Observable entonces dicho componente se debe suscribir al Observable para esperar la respuesta del mismo, de esta forma se manejan las llamadas asincrónicas 
