# 4 Secundaria

¡Bienvenido! Aquí encontraras los temas a desarrollar cada semana y las actividades que permitiran que tu aprendizaje sea óptimo.

## Programas a instalar

?> Las versiones a instalar pueden ser CS5, **CS6** o CC.

- III Bimestre: Unidad 5: Adobe Flash Professional
- III Bimestre: Unidad 6: Adobe Dreamweaver - Visual Studio Code
- IV Bimestre: Unidad 7: Adobe Dreamweaver
- IV Bimestre: Unidad 8: Adobe Dreamweaver

## Presentación de tareas

?> Cuando envies tu tarea en línea, debes tomar en cuenta que el nombre del archivo debe contener el bimestre, la unidad, la sesión , tu primer nombre y tu primer apellido, por ejemplo si deseas enviar un archivo de word el nombre sería: `IIIBimestre-Unidad5-Sesion17-PepitoPeriquito.docx`

La presentación de tus tareas es importante. Es la única manera que repases lo que has aprendido en clase. Para hacerlo puedes usar algunas de estas 2 formas:

- **Presencial:** Puedes presentar tu tarea de forma presencial (En clases). Impreso, Disco o USB.
- **En linea:** Puedes presentar tu tarea via correo eletrónico: israel@israelcueva.com o subirlo a través de este [enlace](https://www.dropbox.com/request/pbjxzSv16nzWqFHeSokd "Tareas")

## Recursos

En este apartado se encuentra lo necesario para estar al tanto de todo respecto al curso.

- **Examen de preparación:** [Enlace](https://forms.gle/dSrMgbeK2XZk1Vtw6 "Examen")
- **Carpeta de Recursos:** [Enlace](https://1drv.ms/u/s!AqqTiyJZHGaLgcZfyZqdKO6YsPGABA?e=N5UJQ0 "Recursos")

## Tareas

### Unidad 5 - Adobe Flash

- Realizar la animación de la página 55 del libro de actividades.

## Clases

### Clase 01 - Introducción al lenguaje html

- **Video:** https://www.youtube.com/watch?v=i5Ha_uhyQic
- **Lista de etiquetas html:** En la carpeta de recursos.

En esta sesión veremos lo que es html, para ello debes seguir los pasos siguientes:

#### En dreamweaver

- Crear una carpeta en la ubicación deseada, ponerle tu nombre a esa carpeta
- Abrir Dreamwaver, aceptar si sale un mensaje.
- Ir al menú sitio -> Nuevo Sitio.
- Colocar un nombre al sitio.
- En carpeta del sitio local, darle clic al icono y escoger la carpeta que se habia creado.
- Y por último Guarda el sitio.

#### En VS Code.

- Crear una carpeta en la ubicación deseada, ponerle tu nombre a esa carpeta.
- Clic derecho en esa carpeta y escoger la opción "Open with Code".
- Si no aparece la opción anterior abrir VS code y en el menú file colocar open folder y escoger dicha carpeta.

Una vez creado el sitio o abriendo la carpeta., a la izquierda clic derecho y dependiendo del idioma clic en crear archivo o create file y colocarle de nombre **index.html**. Escribir lo siguiente en ese archivo.

```html
<!DOCTYPE html>
<html lang="es">

<head>
    // Aquí van las características de tu página
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Pon tu título a la página</title>
</head>

<body>
    // Aquí va el contenido de tu página
</body>

</html>
```
 Lo anterior sería la estructura básica o inicial de una página web y el nombre **index.html** siempre será para la página principal de un sitio web. HTML solo se encargaria del contenido o esqueleto del sitio, en la próxima clase veremos como añadirle estilos CSS. 

### Clase 02 - Uso de CSS

- **Video:** https://www.youtube.com/watch?v=XnFd5cBcC54
- **Lista de atributos CSS:** En la carpeta de recursos

La clase anterior vimos como agregar algunas etiquetas html, ahora veremos como añadir estilos CSS. para ello debes hacer lo siguiente:

- Crea una carpeta (create folder) y ponle de nombre CSS.
- En esa carpeta crea un archivo nuevo (New file) y ponle de nombre `estilos.css` (El nombre puede ser distinto, pero la extensión siempre será css).
- Linkamos el css al html añadiendo la etiqueta link al `index.html`

```html
<!DOCTYPE html>
<html lang="es">

<head>
    // Aquí van las características de tu página
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Pon tu título a la página</title>

    <link rel="stylesheet" href="css/estilos.css">

</head>

<body>
    // Aquí va el contenido de tu página
</body>

</html>
```

Al código que ya teniamos le hemos añadido solo `<link rel="stylesheet" href="css/estilos.css">` ,el atributo href hace referencia a la carpeta css y entra a esa carpeta con el `/` y busca un archivo llamado `estilos.css` si le pusiste otro nombre esto sería distinto.

En css hay tres tipos de selectores, para explicarlo en el body de mi página web tengo lo siguiente:

```html
<body>

    <h1>Tipos de animales</h1>

    <h2>Animales vertebrados</h2>

    <h3>Mamíferos</h3>
    <h3>Peces</h3>
    <h3>Aves</h3>
    <h3>Reptiles</h3>
    <h3>Anfibios</h3>

    <h2>Animales invertebrados</h2>

    <h3>Moluscos</h3>
    <h3>Artrópodos</h3>
    <h3>Cnidarios</h3>
    <h3>Equinodermos</h3>
    <h3>Anélidos</h3>
    <h3>Asponjas</h3>

</body>
```
Ahora le agregare estilos en el archivo `estilos.css`.

#### **Selector por etiqueta:** 
Solo coloca el nombre de la etiqueta html, para este caso el h1 y le ponemos a la propiedad color (color de texto) el valor red. 

```css
h1{
    color:red
}
```
#### **Selector por clase:** 
Supongamos de todos esos `h3` que tengo solo quiero colocarle el color verde a algunos, la haria con el selector de etiquetas `.` seguido por el nombre de la clase, en este caso `verde`, es decir que todos los h3 con la clase (class) verde se pintarian de verde.

```html
    <h3 class="verde">Mamíferos</h3>
    <h3>Peces</h3>
    <h3 class="verde">Aves</h3>
    <h3>Reptiles</h3>
    <h3>Anfibios</h3>
```

```css
.verde{
    color:verde
}
```
#### **Selector por id:** 
Si queremos que haya un elemento único le colocamos un id y mediante el `#` le agregamos estilos. **Importante:** El id solo puede ser colocado una sola vez, por ejemplo, el id favorito ya no puedo colocarle de id a ninguna otra etiqueta html. 

```html
    <h3 class="verde">Mamíferos</h3>
    <h3>Peces</h3>
    <h3 class="verde">Aves</h3>
    <h3 id="favorito">Reptiles</h3>
    <h3>Anfibios</h3>
```
```css
#favorito{
    color:orange
}
```

> Si dese colocar mas propiedades css, solo sepáralos con un puto y coma `;`

### Clase 03 - Estructura del proyecto

- **Video:** https://www.youtube.com/watch?v=DxumDNXRtpI
- **Recursos:** En la carpeta de recursos

En HTML 5 se han introducido etiquetas para la estructura de un sitio web como: `header`, `aside`, `article`, `section` y `footer`. Para que entiendas, siempre cuando veas una página web vela como cuadros de texto en Word quehan sido colocados en todo el espacio disponible.

