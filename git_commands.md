# Comandos GIT

```ruby
echo "# git" >> README.md
git init
git add README.md
git commit -m `"first commit"`
git branch -M main
git remote add origin `enlace del repositorio`
git push -u origin main
```

```ruby
git remote add origin `enlace del repositorio`
git branch -M main
git push -u origin main
```

# GIT Cheat Sheet
## 01 Configuración en GIT
- Configurar el nombre que se adjuntará con los commits y tags.
```ruby
git config --global user.name *your name*
```
- Configurar el correo electrónico que se usará con los commits y tags.
```ruby
git config --global user.email *your email*
```
- Habilitar algo de color en la apariencia de salida en GIT.
```ruby
git config --global color.ui auto
```

## 02 Iniciando un proyecto
- Crear un nuevo repositorio localmente. Si el *project name* es dado, GIT creará un nuevo nombre de directorio *project name* y lo inicializará con un repositorio dentro de sí. Si *project name* no es dado, entonces un nuevo repositorio se inicializará en el directorio actual.
```ruby
git init *project name*
```

- Descargar un proyecto con el historial entero de un repositorio remoto.
```ruby
git clone *project url*
```

## 03 Trabajo de Día-a-Día
- Muestra todo el estado del directorio. 
```ruby
git status
```
- Agrega los archivos nuevos o editados. Se puede agregar todos los cambios con agregar espacio y punto al final * .*
```ruby
git add *file name* 
```

- Muestra cambios entre el directorio que se está trabajando y el área de ensayo.
```ruby
git diff *file*
```

- Muestra cualquier cambio entre el área de ensayo y el repositorio.
```ruby
git diff --staged *file*
```

- Descarta cambios en la rama de trabajo. 
```ruby
git checkout -- *file*
```

> [!WARNING]
> Esta acción es irrecuperable.

- Revertir el repositorio al estado conocido anterior.
```ruby
git reset *file*
```

- Crear un nuevo commit de los cambios que se agregaron al área de ensayo. 
```ruby
git commit -m "*your message*"
```
> [!WARNING]
> Los commits siempre deben tener mensaje.

- Remover un directorio desde el directorio de trabajo y del área de ensayo.
```ruby
git rm *file*
```

- Guarde los cambios actuales en su directorio de trabajo para su uso posterior.
```ruby
git stash
```

- Aplique el contenido almacenado en el directorio de trabajo y borre el contenido.
```ruby
git stash pop
```

- Elimina un cambio específico de todos los cambios anteriores.
```ruby
git stash drop
```

## 04 Modelo de Ramas GIT

- Enlistar todas las ramas locales. Con *-a* se muestran todas las ramas remoto. 
```ruby
git branch -a
```

- Crear una nueva rama, haciendo referencia al Head actual.
```ruby
git branch *branch_name*
```

- Cambiar el directorio de trabajo a la rama especificada. Con *-b* y luego crear la rama especificada si no existe.
```ruby
git branch -b *branch_name*
```




```ruby
```