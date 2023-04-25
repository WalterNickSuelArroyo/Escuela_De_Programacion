# Presentacion
# Comenzando la pagina de contacto

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Contacto - Barbería Alura</title>
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="style.css">
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
        test
    </main>
    <footer>
        <img src="logo-blanco.png">
        <p class="copyright">&copy Copyriht Barbaria Alura - 2020</p>
    </footer>
</body>
</html>
```

# Campos basicos
# Estilos para formulario

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
main {
    width: 940px;
    margin: 0 auto;
}
form {
    margin: 40px 0;
}
form label {
    display: block;
    font-size: 20px;
    margin: 0 0 10px;
}
form input {
    display: block;
    padding: 10px 25px;
    width: 50%;
    margin: 0 0 20px 0;
}
```

# Formulario mas completo
# CSS para inputs mas complejos
# Jerarquia en el CSS
# Seleccionando opciones

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Contacto - Barbería Alura</title>
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="style.css">
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
        <form>
            <label for="nombreapellido">Nombre y Apellido</label>
            <input type="text" id="nombreapellido" class="input-padron">

            <label for="correoelectronico">Correo electronico</label>
            <input type="text" id="correoelectronico" class="input-padron">

            <label for="telefono">Telefono</label>
            <input type="text" id="telefono" class="input-padron">

            <label for="mensaje">Mensaje</label>
            <textarea name="" id="mensaje" cols="70" rows="10" class="input-padron"></textarea>

            <div>
                <p>Como le gustaria que le contactemos</p>

                <label for="radio-email"><input type="radio" id="radio-email" value="email"
                        name="contacto">Email</label>

                <label for="radio-telefono"><input type="radio" id="radio-telefono" value="telefono"
                        name="contacto">Telefono</label>


                <label for="radio-whatsapp"><input type="radio" id="radio-whatsapp" value="whatsapp"
                        name="contacto">WhatsApp</label>
            </div>

            <div>
                <p>En cual horario prediere ser atendido</p>
                <select>
                    <option>Mañana</option>
                    <option>Tarde</option>
                    <option>Noche</option>
                </select>
            </div>

            <label class="checkbox"><input type="checkbox">Le gustaria recibir novedades de la Barberia
                Alura</label>
            <input type="submit" value="Enviar formulario">

        </form>
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
main {
    width: 940px;
    margin: 0 auto;
}
form {
    margin: 40px 0;
}
form label, form p {
    display: block;
    font-size: 20px;
    margin: 0 0 10px;
}
.input-padron {
    display: block;
    padding: 10px 25px;
    width: 50%;
    margin: 0 0 20px 0;
}
.checkbox {
    margin: 20px 0;
}
```

# Inputs para celulares
# Datos importantes en los inputs
# Mejorando la semantica del formulario

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Contacto - Barbería Alura</title>
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <div class="caja">
            <h1><img src="logo.png" alt="Logo de la Barberia Alura"></h1>
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
        <form>
            <label for="nombreapellido">Nombre y Apellido</label>
            <input type="text" id="nombreapellido" class="input-padron" required>

            <label for="correoelectronico">Correo electronico</label>
            <input type="email" id="correoelectronico" class="input-padron" required placeholder="email@dominio.com">

            <label for="telefono">Telefono</label>
            <input type="tel" id="telefono" class="input-padron" required placeholder="(XX) XXXX XXXX">

            <label for="mensaje">Mensaje</label>
            <textarea name="" id="mensaje" cols="70" rows="10" class="input-padron" required></textarea>

            <fieldset>
                <legend>¿Como le gustaria que le contactemos?</legend>

                <label for="radio-email"><input type="radio" id="radio-email" value="email"
                        name="contacto">Email</label>

                <label for="radio-telefono"><input type="radio" id="radio-telefono" value="telefono"
                        name="contacto">Telefono</label>


                <label for="radio-whatsapp"><input type="radio" id="radio-whatsapp" value="whatsapp"
                        name="contacto" checked>WhatsApp</label>
            </fieldset>

            <fieldset>
                <legend>¿En cual horario prediere ser atendido?</legend>
                <select>
                    <option>Mañana</option>
                    <option>Tarde</option>
                    <option>Noche</option>
                </select>
            </fieldset>

            <label class="checkbox"><input type="checkbox" checked>¿Le gustaria recibir novedades de la Barberia Alura
            </label>
            <input type="submit" value="Enviar formulario">

        </form>
    </main>
    <footer>
        <img src="logo-blanco.png" alt="Logo de la Barberia Alura">
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
main {
    width: 940px;
    margin: 0 auto;
}
form {
    margin: 40px 0;
}
form label, form legend {
    display: block;
    font-size: 20px;
    margin: 0 0 10px;
}
.input-padron {
    display: block;
    padding: 10px 25px;
    width: 50%;
    margin: 0 0 20px 0;
}
.checkbox {
    margin: 20px 0;
}
```

# Que son las transiciones
# Entendiendo las transformaciones

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Contacto - Barbería Alura</title>
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <div class="caja">
            <h1><img src="logo.png" alt="Logo de la Barberia Alura"></h1>
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
        <form>
            <label for="nombreapellido">Nombre y Apellido</label>
            <input type="text" id="nombreapellido" class="input-padron" required>

            <label for="correoelectronico">Correo electronico</label>
            <input type="email" id="correoelectronico" class="input-padron" required placeholder="email@dominio.com">

            <label for="telefono">Telefono</label>
            <input type="tel" id="telefono" class="input-padron" required placeholder="(XX) XXXX XXXX">

            <label for="mensaje">Mensaje</label>
            <textarea name="" id="mensaje" cols="70" rows="10" class="input-padron" required></textarea>

            <fieldset>
                <legend>¿Como le gustaria que le contactemos?</legend>

                <label for="radio-email"><input type="radio" id="radio-email" value="email"
                        name="contacto">Email</label>

                <label for="radio-telefono"><input type="radio" id="radio-telefono" value="telefono"
                        name="contacto">Telefono</label>


                <label for="radio-whatsapp"><input type="radio" id="radio-whatsapp" value="whatsapp"
                        name="contacto" checked>WhatsApp</label>
            </fieldset>

            <fieldset>
                <legend>¿En cual horario prediere ser atendido?</legend>
                <select>
                    <option>Mañana</option>
                    <option>Tarde</option>
                    <option>Noche</option>
                </select>
            </fieldset>

            <label class="checkbox"><input type="checkbox" checked>¿Le gustaria recibir novedades de la Barberia Alura
            </label>
            <input type="submit" value="Enviar formulario" class="enviar">

        </form>
    </main>
    <footer>
        <img src="logo-blanco.png" alt="Logo de la Barberia Alura">
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
main {
    width: 940px;
    margin: 0 auto;
}
form {
    margin: 40px 0;
}
form label, form legend {
    display: block;
    font-size: 20px;
    margin: 0 0 10px;
}
.input-padron {
    display: block;
    padding: 10px 25px;
    width: 50%;
    margin: 0 0 20px 0;
}
.checkbox {
    margin: 20px 0;
}
.enviar {
    width: 40%;
    padding: 15px 0;
    font-size: 18px;
    font-weight: bold;
    color: white;
    background: orange;
    border: none;
    border-radius: 5px;
    transition: 1s all;
    cursor: pointer;
}
.enviar:hover {
    background: darkorange;
    transform: scale(1.1);
}
```

# Tabla basica
# Etiquetas semanticas para tablas
# Estilos en las tablas
# Conclusion

```html

```

```css

```