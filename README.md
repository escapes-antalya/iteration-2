# MasterCook

¡Impresionante trabajo, equipo! Ya habéis descubierto una parte muy importante: vuestra app se llamará *MasterCook*, y será una app en la cual los usuarios puedan almacenar sus recetas. 

![](recipe.jpeg)

Cada una de las recetas tendrá la siguiente estructura:

```js
{
  name: String, 
  people: Number, //comensales
  time: Number, //tiempo de preparación en minutos
  level: String, //podrá ser "advanced", "easy", "medium"
  image: String,
  ingredients: [String], //array de strings
  creator: ObjectId de User, //¿quién está loguinado en el momento de crearla?
}
```

En el mismo repositorio que habéis empezado, debéis crear las siguientes rutas:

```js
GET /recipes 
GET /recipes/new 
POST /recipes/new
GET /recipes/:recipeId/edit
POST /recipes/:recipeId/edit
GET /recipe/:recipeId/delete
GET /recipe/:recipeId
```
⚠️ Importante: 
- Para crear, editar o eliminar una receta el usuario debe star logueado, tanto para ver la vista como para mandar los cambios a la BDD. Recordad el uso de los `middlewares` para esta parte.
- Para que esta parte se considere hecha debe tener estilos (en móvil)
- BONUS points: que un usuario sin loguear no vea las opciones que no puede llevar a cabo

📍 Cuando acabéis, debéis presentar vuestros avances en el punto de control para recibir las siguientes pistas.
