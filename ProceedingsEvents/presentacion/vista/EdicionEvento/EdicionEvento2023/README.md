
# Proyecto de Desarrollo Web

## Prácticas de Codificación Legible

### 1. Nombres Descriptivos

**Práctica**: Usa nombres descriptivos para variables, funciones y archivos para que el código sea más comprensible.

**Fragmento de Código**:

```html
<!-- Barra de Navegación -->
<nav class="navbar navbar-expand-lg navbar-dark bg-dark px-2">
  <!-- Logotipo a la Izquierda -->
  <a class="navbar-brand" href="#">
    <img src="assets/imagenes/logo-blanco.png" alt="Logotipo" height="50">
  </a>
  <!-- Enlaces de Navegación Centrados -->
  <div class="collapse navbar-collapse justify-content-center">
    <ul class="navbar-nav">
      <li class="nav-item">
        <a class="nav-link" href="#">Inicio</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Eventos</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Sobre Nosotros</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Edición</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Documentos</a>
      </li>
    </ul>
  </div>
  <!-- Barra de Búsqueda a la Derecha -->
  <div class="navbar-collapse justify-content-end">
    <form class="form-inline my-2 my-lg-0">
      <input class="form-control mr-sm-2" type="search" placeholder="Buscar" aria-label="Buscar">
      <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Buscar</button>
    </form>
  </div>
</nav>
```

### 2. Comentarios Claros

**Práctica**: Añade comentarios claros en el código para explicar el propósito y funcionamiento de las secciones clave.

**Fragmento de Código**:

```css
/* Estilos para la Sección Principal */
.hero-section {
  height: 60vh; /* Ajusta la altura según tus necesidades */
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
}

/* Estilos para el Video de Fondo */
.hero-video {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 100%;
  height: 100%;
  object-fit: cover;
  transform: translate(-50%, -50%);
  z-index: 1;
  filter: brightness(50%); /* Oscurece el video */
}
```