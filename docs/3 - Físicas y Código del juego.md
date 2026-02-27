# 🏋️ Físicas y Código del juego

En **Unity**, las *físicas* son el sistema que simula cómo se comportan los objetos en el mundo del juego siguiendo leyes similares a las del mundo real: **gravedad, fuerzas, colisiones, rebotes, fricción, etc.**

En otras palabras, permiten que los objetos **caigan, choquen, se deslicen o empujen** de manera realista (o configurable).

## Componentes principales de las físicas en Unity

### 1️⃣ Rigidbody

Es el componente que permite que un objeto sea afectado por la física (gravedad, fuerzas, impulso).

Si un objeto tiene **Rigidbody**:

* Puede caer por gravedad.
* Puede recibir fuerzas (`AddForce`).
* Reacciona a colisiones.

Sin Rigidbody, el objeto es estático y no se mueve por física.

### 2️⃣ Colliders

Definen la forma física del objeto para detectar colisiones.

Tipos comunes:

* **Box Collider**
* **Sphere Collider**
* **Capsule Collider**
* **Mesh Collider**

💡 Importante:
Un objeto puede tener Collider sin Rigidbody (será un objeto fijo como el suelo).



### 3️⃣ Física 2D vs 3D

Unity tiene dos sistemas separados:

* **Física 3D** → usa `Rigidbody` y `Collider`
* **Física 2D** → usa `Rigidbody2D` y `Collider2D`

No se mezclan entre sí.



## 🔹 Qué puedes hacer con las físicas

* Crear gravedad
* Detectar colisiones (`OnCollisionEnter`)
* Detectar triggers (`OnTriggerEnter`)
* Aplicar fuerzas
* Simular explosiones
* Crear plataformas móviles
* Hacer juegos de disparos, carreras o puzzles