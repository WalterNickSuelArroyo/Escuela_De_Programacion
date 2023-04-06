# ¿QUE ES LA LOGICA DE PROGRAMACION Y COMO APLICARLA?

Las empresas estan empezando a digitalizarse. Se necesita mas mano de obra en tecnologia.

**La logica de programación**

Es un conjuntode habilidades y conocimientos que son esenciales para crear programas de computadora eficientes y confiables.

**Algoritmo**

Es un conjunto de pasos o instrucciones logicas y ordenadas que se diseñan para resolver un problema especifico. En programacion de computadores, un algoritmo se utiliza para describir la secuencia de acciones que deben seguirse para llevar a cabo una tarea determinada. 

**Aplicación de la logica de programación**

Se aplica en la creacion de programas de computadoras para resolver problemas especificos. Para aplicar la logica de programacion, es necesario seguir los siguientes pasos.
1. Definir el problema
2. Identificar las entradas y salidas.
3. Diseñar el algoritmo
4. Traducir el algoritmo a un lenguaje de programacion
5. Codificar y probar el programa
6. Mantener el programa

**Consejo**

Comenzar con JavaScript, es facil, versatil, es el mas utilizado en todo el mundo. Por su simpliciad no requiere un programa especial en el computador.

# APRENDE TODO SOBRE EL IDE - ENTORNO DE DESARROLLO INTEGRADO
**IDE**
El entorno de desarrollo integrado (IDE- Integrated Development Environment) es una herramienta de desarrollo para editar codigo, acceder a una termina, ejecutar un script, depurar y compilar utilizando un unico entorno.

**Diferencia entre un editor de codigo y un IDE**

Un editor de código se utiliza para escribir, editar y dar formato al código fuente. Los editores de código suelen ofrecer características como resaltado de sintaxis, plegado de código, autocompletado, búsqueda y reemplazo, entre otros. Sin embargo, un editor de código no proporciona herramientas específicas para el desarrollo de software, como la compilación, la depuración o la integración de control de versiones.

Por otro lado, un IDE proporciona todas las características de un editor de código y, además, proporciona una variedad de herramientas y características para el desarrollo de software. Los IDEs suelen ofrecer características como la integración de control de versiones, el depurador, el perfilador, la gestión de proyectos y la compilación, entre otros. 

**Editores de codigo fuente:**
- Visual Studio Code
- Sublime Text
- Atom
- Notepad++
- Vim

**IDEs**
- Eclipse
- Visual Studio
- IntelliJ IDEA
- Android Studio
- Xcode

# CURSO DE LOGICA DE PROGRAMACION: PRIMEROS PASOS

## COMIENCE A PROGRAMAR HOY

### PRESENTACION

Se utilizara el navegador Google Chrome para el curso. Como editor de codigo utilizaremos Sublime Text o VSC

### CREANDO TU PROPIO CODIGO HTML

```html
<h1>mi primer programa HTML!!!</h1>
<br>
<br>
sera esto realmente un programa?
```

### ESTO SI ES PROGRAMACION

```html
<h1>mi primer programa HTML!!!</h1>
<br>
<br>
sera esto realmente un programa?, descubrelo <a href="https://es.wikipedia.org/wiki/HTML">aqui</a>
<br>
Ingresa <a href="https://es.wikipedia.org/wiki/JavaScript">aqui</a> para ver un verdadero lenguaje de programacion


<script>
    alert("Esto si es un lenguaje de programacion");
</script>
```

## COMUNIQUESE CON EL USUARIO

### Convenio de codificacion:

Existe una convención que establece el uso de etiquetas en letras minúsculas en HTML, sin embargo, si usamos letras mayúsculas, para el navegador no habrá diferencia alguna.

### Concatenando caracteres

```html
<meta charset="UTF-8">



<script>
    document.write("La edad de cristian es...<br>");
    document.write("25");
</script>

<!--Para concatenar cadenas de texto o caracteres usamos el signo  +   -->
```

### Operaciones con textos y numeros

```html
<meta charset="UTF-8">

<script>
    document.write("La suma de las edades de Juan, Pedro y Carlos es...");
    document.write("<br>");
    document.write(20+25+15);
    document.write("<br>");
    document.write("<br>");
    document.write("Juan nacio en el año...");
    document.write("<br>");
    document.write(2020-20);
    document.write("<br>");
    document.write("<br>");
    document.write("Pedro nacio en el año...");
    document.write("<br>");
    document.write(2020-25);
    document.write("<br>");
    document.write("<br>");
    document.write("Carlos nacio en el año...");
    document.write("<br>");
    document.write(2020-15);
</script>
```

## DEJE SU PROGRAMA DINAMICO USANDO VARIABLES

### Reduciendo alteraciones
```html
<meta charset="UTF-8">

<script>
    var anho = 2025;
    document.write("Juan tiene: "+(anho - 2000)+" años");
    document.write("<br>");
    document.write("<br>");
    document.write("Pedro tiene: "+(anho - 1995)+" años");

    anho = 2030

    document.write("<br>");
    document.write("<br>");
    document.write("Carlos tiene: "+(anho - 2005)+" años");
    </script>
```

### Variables

```html
<meta charset="UTF-8">

<script>
    var anho = 2025;
    document.write("Juan tiene: "+(anho - 2000)+" años");
    document.write("<br>");
    document.write("<br>");
    document.write("Pedro tiene: "+(anho - 1995)+" años");
    document.write("<br>");
    document.write("<br>");
    document.write("Carlos tiene: "+(anho - 2005)+" años");

    anho = 2020

    document.write("<br>");
    document.write("<br>");
    document.write("<br>");
    document.write("<br>");

    document.write("Jimena tiene: "+(anho - 2010)+" años");
    document.write("<br>");
    document.write("<br>");
    document.write("Paola tiene: "+(anho - 1995)+" años");
    document.write("<br>");
    document.write("<br>");
    document.write("Laura tiene: "+(anho - 2005)+" años");
    document.write("<br>");
    document.write("<br>");

    var edadJimena = 10;
    var edadPaola = 25;
    var edadLaura = 15;

    var nombre1 = "Jimena";
    var nombre2 = "Paola";
    var nombre3 = "Laura";

    promedio = (edadJimena + edadPaola + edadLaura)/3;

    document.write("El promedio de las edades de " + nombre1 + ", " + nombre2 + " y " + nombre3 + " es: " + Math.round(promedio));
    </script>
```


## CREE SUS PROPIAS FUNCIONALIDADES

### Mejorando el mantenimiento de codigo

```html
<meta charset="UTF-8">
<script>
    var anho = 2025;
    var saltoLinea = "<br><br><br>"; 

    document.write("Juan tiene: "+(anho - 2000)+" años");

    document.write(saltoLinea);

    document.write("Pedro tiene: "+(anho - 1995)+" años");

    document.write(saltoLinea);

    document.write("Carlos tiene: "+(anho - 2005)+" años");
    </script>
```

### Funciones

```html
<meta charset="UTF-8">
<script>
    function saltarLinea(){
        document.write("<br>");
        document.write("<br>");
        document.write("<br>");
    }

    var anho = 2025;
    var saltoLinea = "<br><br><br>"; 

    document.write("Juan tiene: "+(anho - 2000)+" años");

    saltarLinea();

    document.write("Pedro tiene: "+(anho - 1995)+" años");

   saltarLinea();

    document.write("Carlos tiene: "+(anho - 2005)+" años");
</script>
```

## PRACTIQUE RESOLVIENDO PROBLEMAS DEL DIA A DIA

### Calculo del IMC, aplicacion

```html
<meta charset="UTF-8">
<h1>PROGRAMA CALCULAR IMC</h1>
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
    function calcularImc(peso,altura,nombre){
        imc = peso/ (altura*altura);
        imprimir("El imc calculado de " + nombre + " es: "  + imc);
    }
    calcularImc(71,1.72,"Christian");
    calcularImc(75,1.73,"Felipe");
</script>
```

### Explorando a fondo el retorno de funciones

```html
<meta charset="UTF-8">
<h1>PROGRAMA CALCULAR IMC</h1>
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
    imprimir("El promedio del imc calculado de Christian y Bruno es: "  + (calcularImc(71,1.72)+calcularImc(75,1.73))/2);
    imprimir("El promedio del imc calculado de Gabriela y Luisa es: "  + (calcularImc(65,1.68)+calcularImc(55,1.60))/2);
</script>
```

### Interactuando con el usuario

```html
<meta charset="UTF-8">
<h1>PROGRAMA CALCULAR IMC</h1>
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
    var nombre = prompt("Informe su nombre")
    var pesoInformado = prompt(nombre + ", Informe su peso");
    var alturaInformado = prompt(nombre + ", Informe su altura");



    imprimir("El imc calculado de " + nombre + " es " + calcularImc(pesoInformado,alturaInformado));
</script>
```