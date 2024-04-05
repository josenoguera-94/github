# GITHUB

- [GitHub Actions](https://docs.github.com/es/actions)
- [Quickstart](https://docs.github.com/es/actions/quickstart)
- [Default variables](https://docs.github.com/es/actions/learn-github-actions/variables)

## **SECRETS AND VARIABLES**

para crear secretos y variables de entorno en github actions se debe seguir la siguiente ruta:

- `Settings` > `Secrets and variables` > `Actions` > `Secrets` o `Variables`

para obtener el valor de un secreto o variable se debe utilizar la siguiente sintaxis:

```yaml
${{ secrets.SECRET_NAME }}
${{ vars.VARIABLE_NAME }}

# esta ultima se declara en el archivo de configuración del workflow
${{ env.VARIABLE_NAME }}
```

- **Secrets**: son variables de entorno que se almacenan encriptadas y se pueden utilizar en un job.
  - **repository secrets**: se pueden utilizar en cualquier job de un repositorioespecífico.
  - **environment secrets**: se pueden utilizar en un job de un ambiente específico.
  - **organization secrets**: se pueden utilizar en cualquier job de una organización.
- **Environment**: son variables de entorno que se pueden utilizar en un job. no son encriptadas.

## ACTIONS

github actions es una herramienta que permite automatizar tareas del lado del servidor en un repositorio de github. Se pueden ejecutar acciones predefinidas o personalizadas en respuesta a eventos específicos.

sus principales componentes son:

- **Workflows**: se definen en un archivo de configuración en la ruta `.github/workflows/` y se encargan de definir las acciones a ejecutar.
- **Actions**: son las tareas que se ejecutan en respuesta a un evento específico.
- **Events**: son los eventos que pueden desencadenar una acción.
- **Runners**: son las máquinas virtuales que ejecutan las acciones.
- **Workflow file**: es el archivo de configuración que define el flujo de trabajo.
- **Job**: es una colección de tareas que se ejecutan en un runner.
- **Step**: es una tarea individual que se ejecuta en un job.
- **Action**: es una tarea reutilizable que se puede utilizar en un job.
- **Service**: es un contenedor que se puede ejecutar en un job.
- **Environment**: son las variables de entorno que se pueden utilizar en un job.
- **Secrets**: son las credenciales que se pueden utilizar en un job.
- **Artifacts**: son los archivos que se pueden almacenar y compartir entre jobs.
- **Cache**: es el almacenamiento en caché que se puede utilizar en un job.

run shell uses with working-directory
