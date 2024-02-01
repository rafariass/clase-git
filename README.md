
# GIT

Git es un sistema de control de versiones distribuido (DVCS, por sus siglas en inglés) que se utiliza para el seguimiento de cambios en el código fuente durante el desarrollo de software. Fue creado por Linus Torvalds en 2005 para gestionar el desarrollo del kernel de Linux, pero desde entonces se ha convertido en una herramienta ampliamente utilizada en la industria del software para el control de versiones y la colaboración en proyectos de programación.



## Instalación

[Web Oficial](https://git-scm.com/)


## Configuración

Primero que todo, debemos configurar un nombre y una dirección de correo electrónico asociados a Git. Esto se hace con el objetivo de identificar, dentro del proyecto, **quién** modificó qué y cómo poder ubicarlo.


```bash
git config —global user.name '<name>'
```

```bash
git config —global user.email '<email>'
```

Reemplazar <name> y <email> por tus datos.


### Verificacion de la configuracion

Podemos revisar si la configuracion quedo correcta en nuestro sistema de 2 formas.

1- **Forma Global**:

```bash
git config --list
```

2- **Forma particular**:

```bash
git config --get user.email
git config --get user.name
```


## Comandos Basicos


| Comando                       | Descripcion                                                       |
| :---------------------------- | :---------------------------------------------------------------- |
| `git init`                    | Inicialoza un proyecto git                                        |
| `git add <file>`              | Agrga al Staged el `<file>` especificado                          |
| `git add --all`               | Agrga al Staged todos los archivos modificados                    |
| `git add .`                   | Agrga al Staged todos los archivos modificados                    |
| `git commit -m '<message>'`   | Registra los cambios del repositorio con el mensaje `<message>`   |
| `git log`                     | Muestra el historial de commits                                   |
| `git status`                  | Muestra el estado del seguimiento del proyecto                    |
| `git push origin <branch>`    | Empuja los cambios de la rama actual a la rama remota `<branch>`  |
| `git pull origin <branch>`    | Trae los cambios de la rama remota `<branch>` a la rama actual    |
| `git switch -c <new_name>`    | Crea una rama nueva por nombre `<new_name>` y entra a la misma    |
| `git switch <new_name>`       | Entra a la rama `<new_name>`                                      |
| `git branch -M <new_name>`    | Renombe la rama actual por `<new_name>`                           |
| `git clone <url>`             | Clona localmente un proyecto unicado en la web con la url `<url>` |
| `git remote -v`               | Revisa las url's remotas del proyecto local                       |
| `git remote add origin <url>` | Agrega una url remota a un proyecto local                         |


## Authors

- [@rafariass](https://www.github.com/rafariass)


## License

[MIT](./LICENSE)
