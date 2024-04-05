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
