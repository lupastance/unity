# 🧪 Las tuberias

Ya tenemos a nuestro 🐦 Prota listo para volar, con su gravedad y su **collider** establecido dentro del propio **GameObject**. Lo que tenemos que hacer ahora es crear el **GameObject** para las tuberías y hacer que vayan apareciendo y avanzado por la pantalla.

## La tuberia como ***GameObject***

De la misma manera que hemos hecho con *Bird Läwson* tendremos que crear un **GameObject** nuevo dentro de nuestro juego para poder asociarle el sprite de la tuberia y sus propiedades.

Seguimos los pasos de antes:

- Botón derecho en el panel de **Jerarquía** > ***Create empty***
- Le ponemos un nombre, por ejemplo 👉 ***Pipe***
- Crea otro **GameObject** que se llame ***Top Pipe*** que esté dentro de **Pipe**
- Vamos a situarlo justo en la misma posición que el pájaro
- Asigna el sprite de la tubería a tu nuevo objeto de juego que acabas de crear
- Establece el tamaño idóneo, para que conservar ciertas proporciones
- Añade un componente de colisión **Box Collider 2D** y estable el tamaño que consideres
- Ahora duplica este objeto que hemos creado, el de **Top Pipe**
- Cámbiale el nombre al objeto duplicado, por ejemplo 👉 **Bottom Pipe**
- En las propiedades del objeto, en el apartado ***scale*** pon el valor en negativo
- Establece la posición que quieras para dicha tubería, ten en cuenta el tamaño del protagonista

<video controls style="margin: 20px auto;">
  <source src="../assets/pipes.mp4" type="video/mp4">
  Tu navegador no soporta el video.
</video>