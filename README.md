# Doks-based template

Proyecto basado en [Doks](https://getdoks.org/) y [doks-gh-pages](https://github.com/h-enk/doks-gh-pages)

### 💻 Ambiente de desarrollo

#### Configuración de herramientas

Puede utilizarse con las herramientas instaladas o utilizando un contenedor de 🐳, como por ejemplo [este.](https://hub.docker.com/r/bitlogicos/redoc)

Para comenzar a editar, se debe clonar o forkear el repositorio (recordando que si se clona será necesario [cambiar el link al repositorio remoto](https://docs.github.com/en/github/getting-started-with-github/managing-remote-repositories#changing-a-remote-repositorys-url), ya que esto se trata de una plantilla y no debe ser modificada)

#### Instalación de dependencias

Una vez descargado el proyecto, se debe ejecutar el siguiente comando para contar con los paquetes necesarios para compilar el código:
```
  npm install
```

Luego, para probar el funcionamiento, se puede ejecutar:

```
  npm run start
```

lo cual iniciará el servidor de desarrollo en el puerto **1313** por defecto.

### 📦 Directorios relevantes

Para modificar según sea necesario, las carpetas más importantes a tener en cuenta son:

* [`content`](https://github.com/bitlogic/doks-template/tree/master/content): Como su nombre lo indica, allí se encuentran los archivos que hacen al contenido del documento. 

* [`layouts`](https://github.com/bitlogic/doks-template/tree/master/layout): Contiene la estructura html del template, además de ciertas configuraciones como headers y redirecciones

* [`config`](https://github.com/bitlogic/doks-template/tree/master/config): Archivos de configuración varios. `_default` contiene la configuración en sí de la estructura de la página, mientras que `production` es exclusiva para ambientes productivos (en este caso sólo contiene la url de producción en `config.toml`)

Para mayor detalle de la estructura de directorios y su contenido, visitar [aquí.](https://getdoks.org/docs/prologue/directory-structure/)

### 🧰 Despliegue en ambientes productivos

En este caso se desplegó en Github Pages, utilizando Github Actions. Sin embargo si se observa el [.yml de ci](https://github.com/bitlogic/doks-template/blob/master/.github/workflows/deploy-github.yml), se notará que utiliza simplemente una imagen de node para generar el documento estático. 

En la documentación oficial de [Doks](https://getdoks.org/docs/recipes/deployment/) se encuentran ejemplos de otros servicios como AWS o Gitlab pages.
