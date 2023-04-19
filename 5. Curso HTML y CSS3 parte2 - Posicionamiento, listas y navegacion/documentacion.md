# Revision

# Nueva Página

# Encabezado

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Productos - Barbería Alura</title>
    <link rel="stylesheet" href="productos.css">
</head>

<body>
    <header>
        <h1><img src="logo.png" alt=""></h1>
        <ul>
            <li>Home</li>
            <li>Productos</li>
            <li>Contacto</li>
        </ul>
    </header>

</body>

</html>
```

# Estructurando la navegación

# Ajustando la lista

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Productos - Barbería Alura</title>
    <link rel="stylesheet" href="productos.css">
</head>
<body>
    <header>
        <h1><img src="logo.png" alt=""></h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="productos.html">Productos</a></li>
                <li><a href="contacto.html">Contacto</a></li>
            </ul>
        </nav>

    </header>
</body>
</html>
```

```css
header {
    background: #BBB;
}
nav li {
    display: inline;
    margin: 0 0 0 15px;
}
nav a {
    text-transform: uppercase;
    color: #000;
    font-weight: bold;
    font-size: 22px;
    text-decoration: none;
}
```

# Limpiando el CSS
# Como funciona el posicionamiento
# Posicionando el encabezado

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Productos - Barbería Alura</title>
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="productos.css">
</head>
<body>
    <header>
        <div class="caja">
            <h1><img src="logo.png"></h1>
            <nav>
                <ul>
                    <li><a href="index.html">Home</a></li>
                    <li><a href="productos.html">Productos</a></li>
                    <li><a href="contacto.html">Contacto</a></li>
                </ul>
            </nav>
        </div>

    </header>
</body>
</html>
```

```css
header {
    background: #BBB;
    padding: 20px 0;
}
.caja {
    width: 940px;
    position: relative;
    margin: 0 auto;
}
nav {
    position: absolute;
    top: 115px;
    right: 0px;
}
nav li {
    display: inline;
    margin: 0 0 0 15px;
}
nav a {
    text-transform: uppercase;
    color: #000;
    font-weight: bold;
    font-size: 22px;
    text-decoration: none;
}
```

# Divisiones semanticas
# Creando Listas complejas
# Reforzando el inline-block
# Ajustando el tamano de los elementos

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Productos - Barbería Alura</title>
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="productos.css">
</head>
<body>
    <header>
        <div class="caja">
            <h1><img src="logo.png"></h1>
            <nav>
                <ul>
                    <li><a href="index.html">Home</a></li>
                    <li><a href="productos.html">Productos</a></li>
                    <li><a href="contacto.html">Contacto</a></li>
                </ul>
            </nav>
        </div>

    </header>
    <main>
        <ul class="productos">
            <li>
                <h2>Cabello</h2>
                <img src="cabello.jpg" alt="">
                <p class="producto-descripcion">Con tijera o maquina, a gusto del cliente</p>
                <p class="producto-precio">$ 10.00</p>
                
            </li>
            <li>
                <h2>Barba</h2>
                <img src="barba.jpg" alt="">
                <p class="producto-descripcion">Corte y diseño profesional de barba</p>
                <p class="producto-precio">$ 8.00</p>
                
            </li>
            <li>
                <h2>Cabello + Barba</h2>
                <img src="cabello+barba.jpg" alt="">
                <p class="producto-descripcion">Paquete completo de cabello y barba</p>
                <p class="producto-precio">$ 15.00</p>
                
            </li>
        </ul>
    </main>
</body>
</html>
```

```css
header {
    background: #BBB;
    padding: 20px 0;
}
.caja {
    width: 940px;
    position: relative;
    margin: 0 auto;
}
nav {
    position: absolute;
    top: 115px;
    right: 0px;
}
nav li {
    display: inline;
    margin: 0 0 0 15px;
}
nav a {
    text-transform: uppercase;
    color: #000;
    font-weight: bold;
    font-size: 22px;
    text-decoration: none;
}
.productos {
    width: 940px;
    margin: 0 auto;
    padding: 50px;
}
.productos li {
    display: inline-block;
    text-align: center;
    width: 30%;
    vertical-align: top;
    margin: 0 1.5%;
    padding: 30px 20px;
    box-sizing: border-box;
}
.productos h2 {
    font-size: 30px;
    font-weight: bold;
}
.producto-descripcion {
    font-size: 18px;
}
.producto-precio {
    font-size: 20px;
    font-weight: bold;
    margin-top: 10px;
}
```

# Aplicando bordes
# Bordes redondeados

```css
header {
    background: #BBB;
    padding: 20px 0;
}
.caja {
    width: 940px;
    position: relative;
    margin: 0 auto;
}
nav {
    position: absolute;
    top: 115px;
    right: 0px;
}
nav li {
    display: inline;
    margin: 0 0 0 15px;
}
nav a {
    text-transform: uppercase;
    color: #000;
    font-weight: bold;
    font-size: 22px;
    text-decoration: none;
}
.productos {
    width: 940px;
    margin: 0 auto;
    padding: 50px;
}
.productos li {
    display: inline-block;
    text-align: center;
    width: 30%;
    vertical-align: top;
    margin: 0 1.5%;
    padding: 30px 20px;
    box-sizing: border-box;
    border: 2px solid #000;
    border-radius: 10px;
}
.productos h2 {
    font-size: 30px;
    font-weight: bold;
}
.producto-descripcion {
    font-size: 18px;
}
.producto-precio {
    font-size: 20px;
    font-weight: bold;
    margin-top: 10px;
}
```

# Capturando el movimiento del mouse
# Capturando el clic del mouse

```css
header {
    background: #BBB;
    padding: 20px 0;
}
.caja {
    width: 940px;
    position: relative;
    margin: 0 auto;
}
nav {
    position: absolute;
    top: 115px;
    right: 0px;
}
nav li {
    display: inline;
    margin: 0 0 0 15px;
}
nav a {
    text-transform: uppercase;
    color: #000;
    font-weight: bold;
    font-size: 22px;
    text-decoration: none;
}
nav a:hover{
    color: #c78c19;
    text-decoration: underline;
}

.productos {
    width: 940px;
    margin: 0 auto;
    padding: 50px;
}
.productos li {
    display: inline-block;
    text-align: center;
    width: 30%;
    vertical-align: top;
    margin: 0 1.5%;
    padding: 30px 20px;
    box-sizing: border-box;
    border: 2px solid #000;
    border-radius: 10px;
}
.productos li:hover {
    border-color: #c78c19;

} 
.productos li:active {
    border-color: #088c19;
}
.productos h2 {
    font-size: 30px;
    font-weight: bold;
}
.productos li:hover h2{
    font-size: 33px;
}
.producto-descripcion {
    font-size: 18px;
}
.producto-precio {
    font-size: 20px;
    font-weight: bold;
    margin-top: 10px;
}
```

# Pie de pagina
# Caracteres especiales

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Productos - Barbería Alura</title>
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="productos.css">
</head>
<body>
    <header>
        <div class="caja">
            <h1><img src="logo.png"></h1>
            <nav>
                <ul>
                    <li><a href="index.html">Home</a></li>
                    <li><a href="productos.html">Productos</a></li>
                    <li><a href="contacto.html">Contacto</a></li>
                </ul>
            </nav>
        </div>

    </header>
    <main>
        <ul class="productos">
            <li>
                <h2>Cabello</h2>
                <img src="cabello.jpg" alt="">
                <p class="producto-descripcion">Con tijera o maquina, a gusto del cliente</p>
                <p class="producto-precio">$ 10.00</p>
                
            </li>
            <li>
                <h2>Barba</h2>
                <img src="barba.jpg" alt="">
                <p class="producto-descripcion">Corte y diseño profesional de barba</p>
                <p class="producto-precio">$ 8.00</p>
                
            </li>
            <li>
                <h2>Cabello + Barba</h2>
                <img src="cabello+barba.jpg" alt="">
                <p class="producto-descripcion">Paquete completo de cabello y barba</p>
                <p class="producto-precio">$ 15.00</p>
                
            </li>
        </ul>
    </main>
    <footer>
        <img src="logo-blanco.png">
        <p class="copyright">&copy Copyriht Barbaria Alura - 2020</p>
    </footer>
</body>
</html>
```

```css
header {
    background: #BBB;
    padding: 20px 0;
}
.caja {
    width: 940px;
    position: relative;
    margin: 0 auto;
}
nav {
    position: absolute;
    top: 115px;
    right: 0px;
}
nav li {
    display: inline;
    margin: 0 0 0 15px;
}
nav a {
    text-transform: uppercase;
    color: #000;
    font-weight: bold;
    font-size: 22px;
    text-decoration: none;
}
nav a:hover{
    color: #c78c19;
    text-decoration: underline;
}

.productos {
    width: 940px;
    margin: 0 auto;
    padding: 50px;
}
.productos li {
    display: inline-block;
    text-align: center;
    width: 30%;
    vertical-align: top;
    margin: 0 1.5%;
    padding: 30px 20px;
    box-sizing: border-box;
    border: 2px solid #000;
    border-radius: 10px;
}
.productos li:hover {
    border-color: #c78c19;

} 
.productos li:active {
    border-color: #088c19;
}
.productos h2 {
    font-size: 30px;
    font-weight: bold;
}
.productos li:hover h2{
    font-size: 33px;
}
.producto-descripcion {
    font-size: 18px;
}
.producto-precio {
    font-size: 20px;
    font-weight: bold;
    margin-top: 10px;
}
footer {
    text-align: center;
    background: url(bg.jpg);   
    padding: 40px;
}
.copyright {
    color: #fff;
    font-size: 13px;
    margin: 20px;
}
```
