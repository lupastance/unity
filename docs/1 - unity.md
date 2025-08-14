# 📦 Unity

![Unity Logo](assets/logo-unity.png){align=right}

En este primer tema vamos a conocer la herramienta principal sobre la que construiremos todo nuestro proyecto 👉 **Unity**.

Antes de ponernos a crear niveles, `scripts` o físicas, es importante entender qué es exactamente Unity, cómo se instala, por qué es una buena opción para aprender desarrollo de videojuegos y qué nos ofrece en comparación con otras alternativas.

---

## Qué es Unity

**Unity** es un motor de desarrollo de videojuegos **multiplataforma** que permite crear juegos en 2D, 3D e incluso experiencias interactivas como simuladores, aplicaciones de realidad virtual (VR), realidad aumentada (AR) o visualizaciones arquitectónicas.

Lo que hace a Unity tan poderoso es que combina varias herramientas clave en un solo entorno:

* Un editor visual para montar escenas con objetos, luces, cámaras y físicas.
* Un sistema de scripting basado en **C#**, que te permite programar el comportamiento de los objetos.
* Herramientas para importar recursos (imágenes, sonidos, animaciones, modelos 3D).
* Opciones de exportación a casi cualquier plataforma: PC, web, móviles, consolas, etc.

En resumen, Unity es un ecosistema completo que te permite pasar de una idea a un juego funcional sin necesidad de reinventar la rueda.

---

## ❓ Por qué usar Unity

Unity es uno de los motores más populares del mundo, y no es por casualidad. Aquí algunas razones por las que es una excelente opción para este y otros proyectos:

✅ Gratuito para aprender

    Unity tiene un plan llamado **Unity Personal**, completamente gratuito para estudiantes, desarrolladores indie y personas con ingresos anuales menores a 100.000 USD. Puedes usarlo sin ninguna limitación en cuanto a funcionalidades.

✅ Multiplataforma

    Con Unity puedes desarrollar para Windows, macOS, Linux, Android, iOS, WebGL, consolas y más… sin tener que reescribir el código para cada plataforma.

✅ Visual + Programación

    Ofrece un entorno visual (Editor de Unity) en el que puedes arrastrar objetos, ajustar parámetros y ver resultados en tiempo real, pero también te permite controlar todo con código, usando C#. Ideal para artistas que están aprendiendo a programar y para programadores que quieren visualizar su trabajo.

✅ Comunidad inmensa

    Al ser tan extendido, encontrarás miles de recursos: tutoriales, plugins, documentación, foros, canales de YouTube, y paquetes ya hechos que puedes integrar fácilmente en tus proyectos.

✅ Usado profesionalmente

    Unity se utiliza tanto en proyectos independientes como en desarrollos profesionales, desde juegos móviles famosos hasta prototipos de empresas como NASA o estudios de animación.

## 🔧 Instalación

Para instalar Unity necesitamos descargar la herramienta de gestión de los productos de Unity, llamada `Unity Hub` donde podremos seleccionar, además de Unity, otras herramientas de diseño y desarrollo.

Además, necesitaremos un editor de código fuente como **Visual Studio Code** o **Visual Studio**.

Por norma general, Visual Studio es más fácil de instalar, pero es verdad que consume muchos recursos y necesitaremos más memoria RAM a la hora de tener abiertos tanto Unity como Visual Studio para desarrollar nuestro juego.

Os recomiendo usar `Visual Studio Code` ya que es más liviano, consume menos recursos y funciona de la misma manera. La única ❌ desventaja es que hay que configurar tanto VSCode como Unity para que funcione correctamente, pero solo tardamos un par de minutos en hacerlo.

### Unity Hub

Unity Hub es una aplicación oficial de Unity que sirve como centro de control para gestionar todos tus proyectos, versiones del motor Unity, módulos adicionales y configuraciones relacionadas con el desarrollo.

Tenemos varias maneras de descargar Unity Hub:

=== "🌍 A través de la web de Unity"
    [🏃‍♂️ Ve a la web oficial de Unity](https://unity.com/es/download){target=blank}

=== "🌐 Usando Winget"
    ```bash
        winget install Unity.UnityHub
    ```

=== "👇 Desde Aquí"
    [1️⃣ Parte 1 de 2](assets/UnityHubSetup.zip.001)<br>
    [2️⃣ Parte 2 de 2](assets/UnityHubSetup.zip.002)

---

#### Instalando Unity

Una vez descargado e instalado, nos preguntará si queremos instalar el 👉 Editor de Unity 👈, seleccionaremos la ubicación donde se copiarán los archivos e instalaremos el software.

![Instalando Unity](assets/unityhub-instalar-1.png)
/// caption
`Instalando el editor de Unity`
///

---

![Instalando Unity 2](assets/unityhub-instalar-2.png){align=left width=300}

Una vez seleccionada la ubicación de instalación, el programa empezará a descargar el `Editor de Unity` y se instalará automáticamente junto con ciertas herramientas necesarias que deben instalarse para poder ejecutar Unity en el ordenador.

---

### 👀 OPCIONAL 👀 Instalando Visual Studio
![Visual Studio](assets/visual-studio-logo.png){ align=right width=150 class="png"}

Aunque lo normal es hacer uso de `Visual Studio` también puedes utilizar **Visual Studio** para programar tus `scripts` que vayas a utilizar en Unity.

Con Visual Studio tendrás más compatibilidad con Unity a la hora de hacer uso del *Intellisense*(1) desde que instalas el software, aunque con Visual Studio Code podrás lograr el mismo resultado pero requiere que se instalen ciertas extensiones adicionales que veremos a continuación.
{ .annotate }

1.  **IntelliSense** es una característica de los editores de código y entornos de desarrollo integrado (*IDE*) que facilita la codificación al ofrecer ayuda para la finalización de código, información sobre parámetros y miembros, y más.<br><br>ℹ️ Es una herramienta útil para la productividad y la reducción de errores al escribir código.
   
La única ❌desventaja❌ de usar `Visual Studio` es que requiere bastante más memoria RAM y puede que a la hora de guardar nuestros `scripts` y sincronizarse con Unity, tarde un poco más de la cuenta.

## ➕ Creando un proyecto

Crear un nuevo proyecto en Unity es el primer paso para dar vida a tus ideas. Desde Unity Hub, podemos definir el tipo de proyecto, su nombre, ubicación y versión del editor que utilizaremos. Una buena configuración inicial nos asegura trabajar con la plantilla y herramientas adecuadas desde el principio, evitando problemas más adelante.

---

![Creando el proyecto](assets/crear-proyecto-1.png)

### 1️⃣ Empezamos

- En el panel lateral izquierdo, selecciona "Projects".
- Ahí verás todos tus proyectos recientes (si es la primera vez, estará vacío).
- Pulsa el botón "New Project" o "Nuevo Proyecto" (según idioma).
- Aparecerá una ventana con varias opciones.

---

![Carpeta, Nombre y Plantilla](assets/crear-proyecto-2.png)

### 2️⃣ Asignando una carpeta, poniéndole nombre y eligiendo una plantilla

- 2D 👉 para juegos y aplicaciones en dos dimensiones, ***este es nuestro caso***
- `Project Name` 👉 Escribe el nombre del proyecto
- `Location` 👉 Elige una carpeta donde Unity guardará todos los archivos del proyecto
- Haz clic en **"Create project"**

!!!bug "Ahora toca esperar un poco..."
    🙃 `Unity Hub` descargará y creará todos los archivos base y abrirá el Editor de Unity<br>
    ⌛ El tiempo de carga inicial puede tardar varios minutos especialmente en ordenadores lentos o con HDD