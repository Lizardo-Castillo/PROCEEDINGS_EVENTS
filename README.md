# Principios SOLID en el Diseño de Componentes de Página Web

En este proyecto, se han aplicado los principios SOLID para diseñar una interfaz web modular y mantenible. A continuación se detalla cómo se implementan estos principios:

## **Single Responsibility Principle (SRP)**

Cada componente de la página tiene una única responsabilidad específica:

- **Footer:** Muestra los datos de derechos de autor.
- **Header:** Contiene el logotipo y los botones con la barra de búsqueda.
- **Hero:** Presenta un video y una breve descripción.
- **Main Content:** Alberga el contenido principal de la página.

Estos componentes están organizados en el directorio `PROCEEDINGS_EVENTS/ProceedingsEvents/presentacion/vista/EdicionEvento/EdicionEvento2023/src/app/component`, garantizando que cada uno maneje una parte distinta de la página.

## **Open/Closed Principle (OCP)**

La separación en componentes asegura que el sistema esté abierto para la extensión pero cerrado para la modificación. Puedes añadir nuevas funcionalidades o contenido sin necesidad de alterar el código existente de otros componentes.

## **Interface Segregation Principle (ISP)**

Los componentes están diseñados de manera que cada uno tiene una interfaz específica para su función particular. Esto evita que los componentes dependan de interfaces innecesarias o de métodos que no utilizan.

---

Estos principios ayudan a mantener el código limpio, flexible y fácil de mantener. Para más detalles sobre la implementación, revisa la estructura de los componentes en el directorio mencionado.
