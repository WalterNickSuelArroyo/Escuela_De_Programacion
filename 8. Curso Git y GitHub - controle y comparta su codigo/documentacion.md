# COMANDOS MAS IMPORTANTES EN GIT
- **git init**: Este comando es utilizado para iniciar un nuevo repositorio de Git en un directorio local. Es el primer paso para comenzar a utilizar Git.

- **git add**: Este comando se utiliza para agregar cambios al área de preparación (staging area) antes de hacer un commit. Puedes usar git add . para agregar todos los cambios en el directorio actual.

- **git commit**: Este comando se utiliza para guardar los cambios en el repositorio. Se debe proporcionar un mensaje descriptivo para cada commit.

- **git status**: Este comando te muestra el estado actual del repositorio, incluyendo los archivos modificados, eliminados o agregados.

- **git branch**: Este comando se utiliza para listar, crear o eliminar ramas. Puedes utilizar git branch nombre_de_la_rama para crear una nueva rama.

- **git checkout**: Este comando se utiliza para cambiar entre ramas o para restaurar archivos a una versión anterior.

- **git merge**: Este comando se utiliza para combinar una rama con otra. Por ejemplo, puedes usar git merge nombre_de_la_rama para combinar la rama "nombre_de_la_rama" con la rama actual.

- **git clone**: Este comando se utiliza para crear una copia local de un repositorio remoto. Puedes utilizar git clone url_del_repositorio para clonar el repositorio.

- **git pull**: Este comando se utiliza para actualizar un repositorio local con los cambios del repositorio remoto. Puedes usar git pull para actualizar el repositorio actual.

- **git push**: Este comando se utiliza para enviar cambios locales al repositorio remoto. Puedes utilizar git push para enviar los cambios del repositorio actual al repositorio remoto.

- **git config**: El comando git config se utiliza para configurar las opciones específicas de Git. Estas opciones pueden ser específicas de usuario, de repositorio o globales.

- **git log**: Comando de Git que muestra un registro detallado de los commits realizados en un repositorio Git. El registro se muestra en orden cronológico inverso, es decir, los commits más recientes aparecen primero.

# Presentacion
# ¿Para que sirve Git?

- Git nos permite almacenar los cambios realizados en cada archivo en un servidor propio para eso. Toda la gestión de cambios la realiza Git y solo debemos preocuparnos por crear un código que funcione, y no por quién lo cambió antes.
- Cada cambio que realices se registra en un historial y se puede ver y restaurar en cualquier momento.

# Instalando Git
# Repositorios

- Git administra repositorios y cada persona del equipo puede tener su propio repositorio.
- git init inicializa un repositorio en el directorio donde se ejecuta el comando. Desde este comando, Git podrá administrar los cambios realizados en los archivos.

# Guardando las modificaciones

```git
git status
```

```git
git add <nombre_del_archivo>
```

```git
git add .
```

```git
git commit -m "Mensaje del commit"
```

```git
git config --global user.name "Tu nombre"
git config --global user.email "tu_correo@ejemplo.com"
```

# Viendo el historico

Ver todos los commits
```git
git log
```

Muestra cada commit en una sola línea, con un resumen del mensaje del commit y su hash abreviado.
```git
git log --oneline
```

Muestra una representación gráfica de la estructura del árbol de commits.
```git
git log --graph
```

Muestra solo los commits realizados por el autor "John Doe"
```git
git log --author="John Doe"
```

Muestra solo los commits realizados en los últimos 7 días.
```git
git log --since=7.days
```

La configuración global se aplica a todos los repositorios de Git en tu sistema
```git
git config --global user.name "Tu nombre"
git config --global user.email "tu@email.com"

```

La configuración local se aplica solo al repositorio de Git actual.
```git
git config --local user.name "Tu nombre"
git config --local user.email "tu@email.com"
```

Observar correo y email
```git
git config user.name
git config user.email
```

Limpiar comandos
```git
git clear
```

Pagina que me puede interesar sobre git log

https://devhints.io/git-log

# Ignorando archivos

# Repositorios remotos
# Sincronizando los datos
# Github

Si quieres clonar el repositorio de Git de la biblioteca React en GitHub a un directorio llamado react-app

```git
git clone https://github.com/facebook/react.git react-app
```

Si estás en la rama main y quieres obtener los cambios más recientes de la rama main del repositorio remoto origin

```git
git pull origin master
```

# Branches
# Uniendo el trabajo
# Actualizando la branch
# Resolviendo conflictos


