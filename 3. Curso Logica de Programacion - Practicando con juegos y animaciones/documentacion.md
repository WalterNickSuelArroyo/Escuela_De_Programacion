# Canvas sera nuestra pantalla

```html
<canvas width="600" height="400"></canvas>
<script>
    var pantalla = document.querySelector("canvas");
    var pincel = pantalla.getContext("2d");
</script>
```

# Diseñando una bandera con un pincel

```html
<canvas width="600" height="400"></canvas>
<script>
    var pantalla = document.querySelector("canvas");
    var pincel = pantalla.getContext("2d");

    pincel.fillStyle = "lightgrey"
    pincel.fillRect(0,0,600,400);

    pincel.fillStyle = "green"
    pincel.fillRect(0,0,200,400);

    pincel.fillStyle = "red"
    pincel.fillRect(400,0,200,400);
</script>
```

# Siendo creativos con la bandera

```html
<canvas width="600" height="400"></canvas>

<script>
    var pantalla = document.querySelector("canvas");
    var pincel = pantalla.getContext("2d");

    pincel.fillStyle = "lightgrey";
    pincel.fillRect(0,0,600,400);

    pincel.fillStyle = "green";
    pincel.fillRect(0,0,200,400);

    pincel.fillStyle = "red";
    pincel.fillRect(400,0,200,400);

    pincel.fillStyle = "yellow";
    pincel.beginPath();
    pincel.moveTo(300,200);
    pincel.lineTo(200,400);
    pincel.lineTo(400,400);
    pincel.fill();

    pincel.fillStyle = "blue";
    pincel.beginPath();
    pincel.arc(300,200,50,0,2*Math.PI);
    pincel.fill();
</script>
```

# Repetir código no es de buenos programadores

```html
<canvas width="600" height="400"></canvas>

<script>
    function dibujarCuadradoVerde() {
        var pantalla = document.querySelector("canvas");
        var pincel = pantalla.getContext("2d");
        pincel.fillStyle = "green";
        pincel.fillRect(0, 0, 50, 50);
        pincel.strokeStyle = "black";
        pincel.strokeRect(0, 0, 50, 50)
    }
</script>
```

# Una funcion mas generica

```html
<canvas width="600" height="400"></canvas>

<script>
    function dibujarCuadrado(x, y, color) {
        var pantalla = document.querySelector("canvas");
        var pincel = pantalla.getContext("2d");
        pincel.fillStyle = color;
        pincel.fillRect(x, y, 50, 50);
        pincel.strokeStyle = "black";
        pincel.strokeRect(x, y, 50, 50)
    }
    dibujarCuadrado(0, 0, "green");
    dibujarCuadrado(50, 0, "green");
    dibujarCuadrado(100, 0, "green");
</script>
```

# Las iteraciones son fantasticas

```html
<canvas width="600" height="400"></canvas>

<script>
    function dibujarCuadrado(x, y, color) {
        var pantalla = document.querySelector("canvas");
        var pincel = pantalla.getContext("2d");
        pincel.fillStyle = color;
        pincel.fillRect(x, y, 50, 50);
        pincel.strokeStyle = "black";
        pincel.strokeRect(x, y, 50, 50)
    }
    /*
    var x = 0;
    while (x < 600) {
        dibujarCuadrado(x, 0, "red");
        dibujarCuadrado(x, 50, "yellow");
        dibujarCuadrado(x, 100, "green");
        x = x + 50;
    }
    */
    for (let x = 0; x < 600; x += 50) {
        dibujarCuadrado(x, 0, "red");
        dibujarCuadrado(x, 50, "yellow");
        dibujarCuadrado(x, 100, "green");
    }
</script>
```

# Nuestra pantalla tiene vida, responde sola

```html
 <canvas width="600" height="400"></canvas>
<script>
    var pantalla = document.querySelector("canvas");
    var pincel = pantalla.getContext("2d");

    pincel.fillStyle = "grey";
    pincel.fillRect(0, 0, 600, 400);

    function exhibirAlerta(){
        alert("Usted hizo un clic");
    }
    pantalla.onclick = exhibirAlerta;
</script>
```

# Mouse, en cual posicion estas

```html
<canvas width="600" height="400"></canvas>

<script>
    var pantalla = document.querySelector("canvas");
    var pincel = pantalla.getContext("2d");
    pincel.fillStyle = "grey";
    pincel.fillRect(0, 0, 600, 400);

    function exhibirAlerta(evento){
        var x = evento.pageX - pantalla.offsetLeft;
        var y = evento.pageY - pantalla.offsetTop;
        alert(x + "," + y);
    }

    function dibujarCirculo(evento){
        var x = evento.pageX - pantalla.offsetLeft;
        var y = evento.pageY - pantalla.offsetTop;

        pincel.fillStyle = "blue";
        pincel.beginPath();
        pincel.arc(x,y,10,0,2*Math.PI);
        pincel.fill();
    }

    pantalla.onclick = dibujarCirculo;
</script>
```

# Ya diseñamos un circulo, ahora a darle vida.

```html
<canvas width="600" height="400"></canvas>

<script>
    var pantalla = document.querySelector("canvas");
    var pincel = pantalla.getContext("2d");
    pincel.fillStyle = "lightgrey";
    pincel.fillRect(0, 0, 600, 400);

    function disenharCircunferencia(x,y,radio){
        pincel.fillStyle = "blue";
        pincel.beginPath();
        pincel.arc(x,y,radio,0,2*Math.PI);
        pincel.fill();
    }
    disenharCircunferencia(20,20,20);
</script>
```

# Diseñando 
# Animaciones simples

```html
<canvas width="600" height="400"></canvas>

<script>
    var pantalla = document.querySelector("canvas");
    var pincel = pantalla.getContext("2d");
    pincel.fillStyle = "lightgrey";
    pincel.fillRect(0, 0, 600, 400);

    function disenharCircunferencia(x, y, radio) {
        pincel.fillStyle = "blue";
        pincel.beginPath();
        pincel.arc(x, y, radio, 0, 2 * Math.PI);
        pincel.fill();
    }

    function limpiarPantalla() {
        pincel.clearRect(0, 0, 600, 400);
    }

    var x = 0;
    function actualizarPantalla() {
        limpiarPantalla();
        disenharCircunferencia(x,20,10);
        x++
        if (x >= 600) {
            x=0;
        }
    }
    setInterval(actualizarPantalla,10);
</script>
```

# Creando objetivo aleatorio

```html
<canvas width="600" height="400"></canvas>
<script>
    var pantalla = document.querySelector("canvas");
    var pincel = pantalla.getContext("2d");
    pincel.fillStyle = "lightgrey";
    pincel.fillRect(0, 0, 600, 400);

    radio = 10;
    var xAleatorio;
    var yAleatorio;

    function disenharCircunferencia(x, y, radio, color) {
        pincel.fillStyle = color;
        pincel.beginPath();
        pincel.arc(x, y, radio, 0, 2 * Math.PI);
        pincel.fill();
    }
    function limpiarPantalla() {
        pincel.clearRect(0, 0, 600, 400);
    }
    function actualizarPantalla() {
        limpiarPantalla();
        xAleatorio = sortearPosicion(600);
        yAleatorio = sortearPosicion(400);
        disenharObjetivo(xAleatorio, yAleatorio);
    }
    function disenharObjetivo(x, y) {
        disenharCircunferencia(x, y, radio + 20, "red");
        disenharCircunferencia(x, y, radio + 10, "white");
        disenharCircunferencia(x, y, radio, "red")
    }
    function sortearPosicion(maximo) {
        return Math.floor(Math.random() * maximo)
    }
    function disparar(evento) {
        var x = evento.pageX - pantalla.offsetLeft;
        var y = evento.pageY - pantalla.offsetTop;
        if ((x < xAleatorio + radio) &&
            (x > xAleatorio - radio) &&
            (y < yAleatorio + radio) &&
            (y > yAleatorio - radio)) {
            alert("Tiro Certero");
        }
    }
    setInterval(actualizarPantalla, 1000);
    pantalla.onclick = disparar;
</script>
```


