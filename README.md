# Assesment I

Como parte del proceso educativo impartido en el progrma TOP Fullstack de Make It Real, hemos destinado durante el transcurso del mismo, una evaluacion que nos ayude a verificar y validar las habilidades adquiridas de los estudiantes.

La evaluacion consta de dos partes; la primera es la creacion de un proyecto en react que consta de varios pasos y la segunda son preguntas tecnicas que requiren de una sustentacion escrita.

### Objectivo
- Validar las habilidades tecnicas de los estudiantes adquiridas durante estas semanas.
- Verificar que los temas destinados a ser dictados en clase previos al `Assesment I` se cumplieran.


### Materiales de apoyo
- [Guia de React - Make It Real](https://guias.makeitreal.camp/react)
- [Documentacion oficial de React](https://reactjs.org/docs/getting-started.html)


## 1. Proyecto

Construir una aplicacion web la cual constará de tres paginas principalmente, la aplicación debe tener un menú para permitir al usuario navegar.

- Home
- Product Detail
- About

#### Requeriemientos

- Usar flexbox CSS.
- El proyecto debe tener configurado ESLint y el Prettier y que tus archivos no tengan problemas con estos.
- El codigo del proyecto debe estar en un repositorio publico de tu autoria.
- Bonus: Implementar tu CSS con BEM o módulos de CSS.

### Home Page
Esta pagina tendra la responsabilidad de listar una serie de productos que debes obtener consumiento la api de [Fake Store API](https://fakestoreapi.com/).

Para mostrar estos productos debes crear un componente llamada `ProductCard` el cual tendra como propiedades `id`, `title`, `image` las cuales tienen que estar renderizadas. Este componente tiene la particularidad de permitir ir al detalle del producto en otra pagina (`http://localhost:3000/detalle/:id`) en la cual se debe renderizar toda la informacion del productoen detallede forma visualmente agradable.

```json
{
  "id": 1,
  "title": "Fjallraven - Foldsack No. 1 Backpack, Fits 15 Laptops",
  "price": 109.95,
  "description": "Your perfect pack for everyday use and walks in the forest. Stash your laptop (up to 15 inches) in the padded sleeve, your everyday",
  "category": "men's clothing",
  "image": "https://fakestoreapi.com/img/81fPKd-2AYL._AC_SL1500_.jpg",
  "rating": {
    "rate": 3.9,
    "count": 120
  }
}
```

Ademas el componente `ProductCard` solo debe permitir ir a la pagina de detalle siempre y cuando un tiempo random configurado de forma aleatoria no se haya vencido. El tiempo restante debe mostrarse en pantalla como una cuenta regresiva para actualizarse cada segundo.

**Ejemplos**:

- `ProductCard-1`: Tiene un tiempo maximo para ir al detalle de **1 min**, cuando el tiempo finalice este `Card` no debe permitir realizar una navegacion.
- `ProductCard-2`: Tiene un tiempo maximo para ir al detalle de **3 min**, cuando el tiempo finalice este `Card` no debe permitir realizar una navegacion.
- `ProductCard-3`: Tiene un tiempo maximo para ir al detalle de **1 min**, cuando el tiempo finalice este `Card` no debe permitir realizar una navegacion.

Este es un ejemplo aproximado de lo que debes hacer:

<img src="./assets/countdown.gif">

### Product detail Page
Renderizar la informacion del producto y permitir navegar a la pagina de inicio o la del perfil.

### About Page
Debes mostrar en esta pantalla tu informacion personal:

- Nombre
- Descripcion
- Imagen
- Lista de 3 cosas que hayas aprendido en este programa
- Correo
- Link a tu github


## 2. Preguntas
- Cuáles son las ceremonias más importantes de un Sprint y cuál es la idea de cada una?
- Qué son los Wireframes? Nombra al menos una herramienta que podamos utilizar.
- Explicar la diferencia entre var, let y const. Y dar un ejemplo en qué caso se utilizaría.
- Organizar una serie de elementos con Flebox (mostrar el resultado esperado).
- ¿Cuales son los tres comandos que se pueden utilizar para crear una nueva rama llamada `rama-1`?
- Explicar la diferencia entre git merge y git rebase.
- ¿Cuál es la diferencia entre Pull Request (PR) y el comando `git pull`?
- ¿Qué es el Virtual DOM?
- Darles un CodeSandbox y en la respuesta que digan cómo lo arreglarían.


