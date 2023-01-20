# MasterCook

¡Impresionante trabajo, equipo Antalya! Ya habéis descubierto una parte muy importante: vuestra app se llamará *MasterCook*, y será una app en la cual los usuarios puedan hacer ciertas acciones con recetas. 

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
Con esta información, debéis:
- Crear el modelo Recipe
- Crear un archivo con un array de 10 recetas
- Hacer un seed de la base de datos

Como habéis visto, en el modelo hay una relación. Sin embargo, en el archivo del seed no tenemos acceso a los objetos *request*, *response* y *next* para acceder a req.session.currentUser, así que, en el apartado "creator", podéis copiar y pegar `_id` de usuarios que hayáis creado previamente mediante el `signup`. 

Los `_id` los podéis copiar y pegar de la base de datos mediante Mongo Compass. Así, en el array, cada receta tendrá un campo así:

```js
{
  ...,
  creator: '63c6f21b0629c422f95e0a7f'
}
```

Estas recetas iniciales pueden tener todos el mismo creador o podéis coger _ids de diferentes usuarios, pero todos tienen que ser usuarios reales que existan en la base de datos.

> 📍 Cuando acabéis, debéis presentar vuestros avances en el punto de control para recibir las siguientes pistas.

