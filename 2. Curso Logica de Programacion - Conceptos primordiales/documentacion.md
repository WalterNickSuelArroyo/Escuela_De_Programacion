# Presentacion
**Contenido de este curso:**
- Condicionales
- Iteraciones(ciclo while y ciclo for)
- Interaccion con el usuario
    - Conectando HTML con JavaScript
    - Botones y Cajas de Texto
- Arrays o Listas
- Chrome será nuestro compilador
- Sublime nuestro editor de texto

# Convirtiendo texto a numero
```html
<meta charset="UTF-8">
<h1>PROGRAMA - CALCULAR PUNTOS DE UN EQUIPO DE FUTBOL</h1>
<script>
    function saltarLinea(){
        document.write("<br>");
        document.write("<br>");
        document.write("<br>");
    }
    function imprimir(frase){
        document.write(frase);
        saltarLinea();
    }
    var victorias = parseInt(prompt("Informe la cantidad de victorias"));
    var empates = parseInt(prompt("Informe la cantidad de empates"));
    puntosTotal = victorias * 3 + empates;
    imprimir("El total de puntos del equipo es: " + puntosTotal);
</script>
```

# Trabajando con condiciones
```html
<meta charset="UTF-8">
<h1>PROGRAMA - CALCULAR PUNTOS DE UN EQUIPO DE FUTBOL</h1>
<script>
    function saltarLinea(){
        document.write("<br>");
        document.write("<br>");
        document.write("<br>");
    }
    function imprimir(frase){
        document.write(frase);
        saltarLinea();
    }
    var victorias = parseInt(prompt("Informe la cantidad de victorias"));
    var empates = parseInt(prompt("Informe la cantidad de empates"));
    puntosTotal = victorias * 3 + empates;
    imprimir("El total de puntos del equipo es: " + puntosTotal);

    if (puntosTotal > 28) {
        imprimir("El equipo esta mejor que el año pasado");
    }
    if (puntosTotal < 28) {
        imprimir("El equipo esta peor que el año pasado");
    }
    if (puntosTotal == 28) {
        imprimir("El equipo esta igual que el año pasado");
    }
</script>
```

# Mejorando el programa de IMC
```html
<meta charset="UTF-8">
<h1>PROGRAMA - CALCULAR IMC</h1>
<script>
    function saltarLinea(){
        document.write("<br>");
        document.write("<br>");
        document.write("<br>");
    }
    function imprimir(frase){
        document.write(frase);
        saltarLinea();
    }
    function calcularImc(peso,altura){
        return (peso / (altura*altura));
    }
    nombre = prompt("Informe su nombre");
    pesoInformado = prompt(nombre + ", informe su peso");
    alturaInformado = prompt(nombre + ", informe su altura");
    imcCalcualdo = calcularImc(pesoInformado,alturaInformado);
    imprimir(nombre + ", su imc calculado es: " + imcCalcualdo);

    if (imcCalcualdo < 18.5) {
        imprimir("IMC abajo de lo recomendado");
    }
    if (imcCalcualdo >= 18.5) {
        if (imcCalcualdo < 25) {
            imprimir("IMC esta dentro del intervalo normal");
        }
    }
    if (imcCalcualdo >= 25) {
        if (imcCalcualdo < 30) {
            imprimir("IMC considerado como sobrepeso");
        }
    }
    if (imcCalcualdo >= 30) {
        imprimir("IMC considerado como obesidad");
    }
</script>
```

# Juego de Adivinación
```html
<meta charset="UTF-8">
<h1>PROGRAMA - CALCULAR IMC</h1>
<script>
    function saltarLinea(){
        document.write("<br>");
        document.write("<br>");
        document.write("<br>");
    }
    function imprimir(frase){
        document.write(frase);
        saltarLinea();
    }
    var numeroPensado = Math.round(Math.random()*10);
    var numeroLanzado = parseInt(prompt("Ingrese un numero entre 0-10"));

    if(numeroPensado == numeroLanzado){
        imprimir("Usted aserto");
    }
    if(numeroPensado != numeroLanzado){
        imprimir("Usted error, el numero pensado era " + numeroPensado);
    }
</script>
```

# Mientras que

```html
<meta charset="UTF-8">
<h1>PROGRAMA - AÑO MUNDIAL DE LA FIFA</h1>
<script>
    function saltarLinea() {
        document.write("<br>");
        document.write("<br>");
        document.write("<br>");
    }
    function imprimir(frase) {
        document.write(frase);
        saltarLinea();
    }
    var anhoMundial = 1930;
    var limite = parseInt(prompt("Ingrese el año limite para calcular"));
    while (anhoMundial <= limite ) {
        imprimir("Hubo Mundial de la FIFA en el año: " + anhoMundial);
        anhoMundial = anhoMundial + 4;
    }
</script>
```

# Otra forma de repetir
```html
<meta charset="UTF-8">
<h1>PROGRAMA - CALCULAR LA TABLA DE MULTIPLICAR</h1>
<script>
    function saltarLinea() {
        document.write("<br>");
        document.write("<br>");
        document.write("<br>");
    }
    function imprimir(frase) {
        document.write(frase);
        saltarLinea();
    }
    var max = 10
    for (let i = 1; i <= max; i++) {
        imprimir("5 por " + i + " = " + (5*i));       
    }
</script>
```

# Acumulando Variables
```html
<meta charset="UTF-8">
<h1>PROGRAMA - CALCULAR LA MEDIA DE LAS EDADES DE UNA FAMILIA</h1>
<script>
    function saltarLinea() {
        document.write("<br>");
        document.write("<br>");
        document.write("<br>");
    }
    function imprimir(frase) {
        document.write(frase);
        saltarLinea();
    }

    var cantidad = parseInt(prompt("Digite cuantos miembros son en su familia: "));
    
    var i = 1;
    var sumaEdades = 0;
    while (i <= cantidad) {
        var edades = parseInt(prompt("Digite la edad de miembro" + i));
        sumaEdades = sumaEdades + edades;
        i++;
    }
    var promedio = sumaEdades / cantidad;
    imprimir("El promedio de las edades de los miembros es: " + promedio);
</script>
```

# Interrumpiendo una Repeticion

```html
<meta charset="UTF-8">
<h1>PROGRAMA - CALCULAR IMC</h1>
<script>
    function saltarLinea() {
        document.write("<br>");
        document.write("<br>");
        document.write("<br>");
    }
    function imprimir(frase) {
        document.write(frase);
        saltarLinea();
    }
    var numeroPensado = Math.round(Math.random() * 10);
    var intentos = 3;
    i = 1;
    while (i <= intentos) {
        var numeroLanzado = parseInt(prompt("Ingrese un numero entre 0-10"));
        if (numeroPensado == numeroLanzado) {
            alert("Usted aserto en el intento " + i + " el numero pensado era " + numeroPensado);
            break;
        }
        if (numeroPensado != numeroLanzado) {
            alert("Usted erró, vuelva a intentarlo ");
        }
        i++;
    }
</script>
```

# Repeticiones anidadas

```html
<meta charset="UTF-8">
<h1>PROGRAMA - ASTERISCOS</h1>
<script>
    function saltarLinea() {
        document.write("<br>");
    }
    function imprimir(frase) {
        document.write(frase);
        saltarLinea();
    }
    for (let i = 1; i <= 3; i++) {
        for (let j = 0; j < 10; j++) {
            document.write("*");         
        }
        saltarLinea(); 
    }
</script>
```

# Campo de Texto y Boton

```html
<meta charset="UTF-8">

<input type="text">
<button>Verificar si acerto con el secreto</button>

<script>
    var secreto = 5;
    var inp = document.querySelector("input");
    function verificar() {
        if (secreto == parseInt(inp.value)) {
            alert("Usted acerto");
        } else {
            alert("Usted erró");
        }
    }

    var but = document.querySelector("button");
    but.onclick = verificar;
</script>
```

# Mejorando la usabilidad

```html
<meta charset="UTF-8">

<input type="text">
<button>Verificar si acerto con el secreto</button>

<script>
    var secreto = Math.round(Math.random() * 10);
    var inp = document.querySelector("input");
    inp.focus();
    function verificar() {
        if (secreto == parseInt(inp.value)) {
            alert("Usted acerto");
        } else {
            alert("Usted erró");
        }
        inp.value = "";
        inp.focus();
    }
    var but = document.querySelector("button");
    but.onclick = verificar;
</script>
```

# Almacenando muchos datos
# Usando Loop para carga de datos
# Tamaño del Array

```html
<meta charset="UTF-8">

<input type="text">
<button>Verificar si acerto con el secreto</button>

<script>
    var secretos = [3, 5, 7, 9];
    var inp = document.querySelector("input");
    inp.focus();
    function verificar() {
        var encontrado = false;
        for (let i = 0; i < secretos.length; i++) {
            if (secretos[i] == parseInt(inp.value)) {
                encontrado = true;
                alert("Usted acerto");
                break;               
            }
        }
        if (encontrado == false) {
            alert("Usted erro");
        }
        inp.value = ""
        inp.focus();        
    }
    var but = document.querySelector("button");
    but.onclick = verificar;
</script>
```

# Manipulando Array
# Validando duplicados
# Refinando nuestro codigo

```html
<meta charset="UTF-8">
<input type="text">
<button>Verificar si acerto con el secreto</button>
<script>
    function aleatorio() {
        return Math.round(Math.random() * 10);
    }
    function sortearNumeros(cantidad) {
        var secretos = [];
        var contador = 1;
        while (contador <= cantidad) {
            var numeroAleatorio = aleatorio();
            var encontrado = false
            if (numeroAleatorio != 0) {
                for (let index = 0; index < secretos.length; index++) {
                    if (numeroAleatorio == secretos[index]) {
                        encontrado = true;
                    }
                }
                if (encontrado = false) {
                    secretos.push(numeroAleatorio);
                    contador++;
                }
            }
        }
        return secretos;
    }
    var secretos = sortearNumeros(4);

    console.log(secretos);


    var inp = document.querySelector("input");
    inp.focus();
    function verificar() {
        var encontrado = false;
        for (let i = 0; i < secretos.length; i++) {
            if (secretos[i] == parseInt(inp.value)) {
                encontrado = true;
                alert("Usted acerto");
                break;
            }
        }
        if (encontrado == false) {
            alert("Usted erro");
        }
        inp.value = ""
        inp.focus();
    }
    var but = document.querySelector("button");
    but.onclick = verificar;
</script>
```
