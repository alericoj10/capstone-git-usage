# Uso de Git para proyecto Capstone
**Importante! Leer documento agregado en el repo: `git-curso.pdf`**
## Formato commits
Usaremos **mensajes en inglés** del formato:
`tipo(contexto): descripción`

- Tipos:
  - `feat`: Un nuevo feature
  - `fix`: La corrección de un bug
  - `style`: Cambios que no afectan el significado del código (espacios, indentación, etc.)
  - `refactor`: Un cambio en el código que no agrega una funcionalidad ni corrige un bug
  - `test`:  Agrega, corrige o mejora tests
  - `chore`: Cambios al proceso de build y herramientas auxiliares
- Contexto:
  - Una palabra que hace referencia al lugar del código o funcionalidad que afecta el commit. Puede ser el nombre del archivo, componente, etc.
- Descripicón:
  - Mensaje que describe lo realizado. Comienza siempre con un verbo imperativo
-Ejemplo:
  - `fix(ui/SignUpForm): validate username availability`

## Formato branches
Vamos a tener 2 branches principales: `main` y `development`.
Cada feature tiene su propia branch sacada desde la rama `development` con el comando `git checkout -b nombre-nueva-rama` y se realizará una Pull request hacia `development` donde tendremos nuestro ambiente de Staging.

## Formato Pull Requests
- Usar el siguiente template de markdown para la descripción de sus pull request
```
# [Commit Type]: [Title]

## Description

[Description of the pull request]

## Requirements

[Additional actions that have to be done for the pull request to work (such as adding a secret key to the repository)]


## Additional changes

[Changes done in this pull request that are additional to the purpose of the branch (such as formatting code or deleting files)]
```
- TODAS LAS PULL REQUEST DEBEN PASAR POR REVISION DE CODIGO POR OTRO INTEGRANTE DEL EQUIPO!
- Quien revisa el codigo es la persona responsable de aprobar y mergear la pull request. No quien la crea
