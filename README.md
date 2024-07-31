Ubicacion de los componentes: PROCEEDINGS_EVENTS/ProceedingsEvents/presentacion/vista/EdicionEvento/EdicionEvento2023/src/app/component

# Cookbook

## Descripción del Cookbook

Un **Cookbook** es una colección de ejemplos y patrones reutilizables en el desarrollo web, proporcionando soluciones estandarizadas para problemas comunes.

## ¿Qué es un Cookbook?

Un **Cookbook** ofrece "recetas" de diseño y desarrollo, con código y mejores prácticas para implementar componentes y estilos web de manera eficiente y consistente.

## Implementación y Contexto del Uso (Footer como Plantilla Cookbook)

El **Footer** es un componente estándar en el **Cookbook** que sirve como una plantilla reutilizable para la sección de pie de página en sitios web.

### Código HTML

```html
<!-- Pie de Página -->
<footer class="bg-dark text-white py-4">
  <div class="container">
    <div class="row">
      <!-- Sección de Navegación -->
      <div class="col-md-3">
        <h5>Navegación</h5>
        <ul class="list-unstyled">
          <li><a href="#home" class="text-white">Inicio</a></li>
          <li><a href="#about" class="text-white">Sobre Nosotros</a></li>
          <li><a href="#services" class="text-white">Servicios</a></li>
          <li><a href="#contact" class="text-white">Contacto</a></li>
        </ul>
      </div>
      <!-- Sección de Contacto -->
      <div class="col-md-3">
        <h5>Contacto</h5>
        <p>Tel: 123-456-7890</p>
        <p>Email: info&#64;mipagina.com</p>
      </div>
      <!-- Sección de Redes Sociales -->
      <div class="col-md-3">
        <h5>Redes Sociales</h5>
        <a href="#facebook" class="text-white me-2"><i class="fab fa-facebook"></i></a>
        <a href="#twitter" class="text-white me-2"><i class="fab fa-twitter"></i></a>
        <a href="#instagram" class="text-white me-2"><i class="fab fa-instagram"></i></a>
      </div>
      <!-- Sección de Suscripción -->
      <div class="col-md-3">
        <h5>Suscríbete</h5>
        <form>
          <div class="input-group">
            <input type="email" class="form-control" placeholder="Tu Email">
            <button class="btn btn-primary" type="button">Suscribirse</button>
          </div>
        </form>
      </div>
    </div>
    <!-- Fila de Derechos Reservados -->
    <div class="row mt-4">
      <div class="col text-center">
        <p>&copy; 2024 Mi Empresa. Todos los derechos reservados.</p>
      </div>
    </div>
  </div>
</footer>
```

### Estilos CSS

```css
/* Estilos para Enlaces del Pie de Página */
footer a {
  text-decoration: none;
  color: #ffffff; /* Blanco */
}

footer a:hover {
  text-decoration: underline;
  color: #dddddd; /* Un tono más claro de blanco */
}

/* Estilos para Texto del Pie de Página */
footer p, footer h5 {
  color: #ffffff; /* Blanco */
}
```

## Explicación de la Implementación

1. **Navegación**: Enlaces a secciones del sitio.
2. **Contacto**: Información de contacto.
3. **Redes Sociales**: Enlaces a redes sociales.
4. **Suscripción**: Formulario para capturar correos electrónicos.
5. **Derechos Reservados**: Aviso legal de copyright.


# Things

## Descripción de Things

**Things** es un enfoque de diseño en el que se utilizan componentes dentro de otros componentes para estructurar y organizar el contenido de manera modular y reutilizable en aplicaciones web.

## ¿Qué es Things?

**Things** se refiere a la práctica de integrar componentes independientes dentro de un contenedor o componente principal para crear una interfaz de usuario más estructurada y manejable. Esto permite una mejor organización y reutilización del código, facilitando el mantenimiento y la escalabilidad de la aplicación.

## Implementación y Contexto del Uso (Uso de un Componente Dentro de un Componente)

En el siguiente codigo, se demuestra el uso de un componente (`app-inscripcion-component`) dentro de un contenedor principal, que organiza dos secciones con contenido y una sección adicional para un componente de inscripción.

### Código HTML

```html
<!-- Contenedor Principal -->
<div class="container my-5">
  <!-- Primera Sección -->
  <div class="row align-items-center mb-5">
    <div class="col-md-6">
      <img src="assets/imagenes/Escuela.png" class="img-fluid" alt="Fondo Escuela">
    </div>
    <div class="col-md-6">
      <h2 class="content-title">Nuestra Escuela</h2>
      <p class="content-description">
        Esta es una breve descripción del primer contenido. Aquí puedes agregar más detalles sobre la imagen a la izquierda.
      </p>
    </div>
  </div>
  
  <!-- Segunda Sección -->
  <div class="row align-items-center mb-5 flex-md-row-reverse">
    <div class="col-md-6">
      <img src="assets/imagenes/Persona.png" class="img-fluid" alt="Persona Random">
    </div>
    <div class="col-md-6">
      <h2 class="content-title">Coordinadores</h2>
      <p class="content-description">
        Esta es una breve descripción del segundo contenido. Aquí puedes agregar más detalles sobre la imagen a la derecha.
      </p>
    </div>
  </div>
  <app-inscripcion-component></app-inscripcion-component>
</div>
```

## Explicación de la Implementación

1. **Contenedor Principal**: Utiliza la clase `container` para un diseño centrado y espacioso.
2. **Sección 1 y 2**: Organiza el contenido en dos secciones utilizando `row` y `col-md-6` para estructurar la información y las imágenes de manera responsiva.
3. **Componente de Inscripción**: Se incluye al final del contenedor principal para integrarlo con el contenido existente, demostrando cómo los componentes pueden ser anidados dentro de otros componentes.


# Descripción de Error/Exception Handling

## ¿Qué es Error/Exception Handling?

**Error/Exception Handling** se refiere a la técnica de manejar y responder a errores y excepciones en el código para evitar que la aplicación falle y para proporcionar una experiencia de usuario más robusta y amigable. En el contexto de formularios y validaciones, esto implica mostrar mensajes de error claros cuando el usuario no cumple con los requisitos de entrada.

## Implementación y Contexto del Uso

En el siguiente codigo, se utiliza **Error/Exception Handling** para validar los campos de un formulario de inscripción y para mostrar mensajes de error cuando el usuario no proporciona información válida o completa.

### Código HTML

```html
<div class="inscripcion-container">
    <h2 class="form-title">Formulario de Inscripción</h2>
    <form (ngSubmit)="onSubmit()" #inscripcionForm="ngForm">
      <div class="form-group" [ngClass]="{ 'has-error': nombre.invalid && (nombre.dirty || nombre.touched) }">
        <label for="nombre">Nombre</label>
        <input type="text" id="nombre" [(ngModel)]="nombre" name="nombre" #nombre="ngModel" required />
        <div *ngIf="nombre.invalid && (nombre.dirty || nombre.touched)" class="error">
          El nombre es requerido.
        </div>
      </div>
      <div class="form-group" [ngClass]="{ 'has-error': apellido.invalid && (apellido.dirty || apellido.touched) }">
        <label for="apellido">Apellido</label>
        <input type="text" id="apellido" [(ngModel)]="apellido" name="apellido" #apellido="ngModel" required />
        <div *ngIf="apellido.invalid && (apellido.dirty || apellido.touched)" class="error">
          El apellido es requerido.
        </div>
      </div>
      <div class="form-group" [ngClass]="{ 'has-error': dni.invalid && (dni.dirty || dni.touched) }">
        <label for="dni">DNI</label>
        <input type="text" id="dni" [(ngModel)]="dni" name="dni" #dni="ngModel" required />
        <div *ngIf="dni.invalid && (dni.dirty || dni.touched)" class="error">
          El DNI es requerido.
        </div>
      </div>
      <div class="form-group" [ngClass]="{ 'has-error': ocupacion.invalid && (ocupacion.dirty || ocupacion.touched) }">
        <label for="ocupacion">Ocupación</label>
        <input type="text" id="ocupacion" [(ngModel)]="ocupacion" name="ocupacion" #ocupacion="ngModel" required />
        <div *ngIf="ocupacion.invalid && (ocupacion.dirty || ocupacion.touched)" class="error">
          La ocupación es requerida.
        </div>
      </div>
      <div class="form-group" [ngClass]="{ 'has-error': correo.invalid && (correo.dirty || correo.touched) }">
        <label for="correo">Correo</label>
        <input type="email" id="correo" [(ngModel)]="correo" name="correo" #correo="ngModel" required />
        <div *ngIf="correo.invalid && (correo.dirty || correo.touched)" class="error">
          El correo es requerido.
        </div>
      </div>
      <div class="form-group" [ngClass]="{ 'has-error': voucher.invalid && (voucher.dirty || voucher.touched) }">
        <label for="voucher">Voucher</label>
        <input type="text" id="voucher" [(ngModel)]="voucher" name="voucher" #voucher="ngModel" required />
        <div *ngIf="voucher.invalid && (voucher.dirty || voucher.touched)" class="error">
          El voucher es requerido.
        </div>
      </div>
      <button type="submit" class="btn btn-primary" [disabled]="inscripcionForm.invalid">Enviar</button>
    </form>
    <div class="separator"></div>
</div>
```

### Explicación de la Implementación

1. **Validación de Campos**: Cada campo del formulario tiene un `ngClass` que agrega la clase `'has-error'` si el campo es inválido y ha sido tocado o modificado. Esto permite aplicar estilos específicos a los campos con errores.

2. **Mensajes de Error**: Se utilizan directivas `*ngIf` para mostrar mensajes de error específicos debajo de cada campo que no cumple con los requisitos de validación. Estos mensajes aparecen solo si el campo es inválido y ha sido tocado o modificado, proporcionando retroalimentación inmediata al usuario.

3. **Estilos**: En el CSS, se definen estilos para la clase `'error'`, que aplica color rojo a los mensajes de error, haciendo que sean fácilmente visibles para el usuario.
