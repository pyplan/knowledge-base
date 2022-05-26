# ![Pyplan](./docs/_static/logo.png)

Repositorio para la Base de conocimientos de Pyplan

## Pasos para contribuir con la base de conocimientos

### Requerimientos

* [python 3](https://www.python.org/downloads/)

### Clonar el repositorio

``` bash
cd  [path-de-proyectos]
git clone https://github.com/pyplan/pyplan-kb.git
```

### Configuración del entorno

``` bash
# Crear entorno virtual
cd [path-de-proyectos]/
python3 -m venv venv
. venv/bin/activate # in linux/mac os
venv\Scripts\activate.bat # in windows
pip install --upgrade pip
pip install -r requirements.txt
```

### Servidor de documentación en vivo

El siguiente comando corre un servidor local que permite visualizar la documentación. Al crear/guardar un nuevo archivo de documentación, el servidor aplicará los cambios y se podrá visualizar en el navegador.

``` bash
cd [path-de-proyectos]/pyplan-kb
sphinx-autobuild -a docs docs/_build/html --port 5500 --open-browser
```

### ¿Cómo contribuir?

1. Hacer checkout (seleccionar y actualizar) la rama **main**
2. Crear una nueva rama con un nombre descriptivo (ejemplo: interfaces-personalizadas) desde la rama **main**.
3. Crear/modificar archivos .rst dentro de la carpeta **/docs**. Tener en cuenta la estructura que se muestra en el punto siguiente.
4. Al terminar, realizar un **Pull Request** desde la rama actual a la rama **main**.
5. Un administrador revisará los cambios y aceptará el Pull Request.


### Estructura de archivos

La documentación se puede escribir en archivos de formato .rst (reStructuredText) o .md (markdown). Preferentemente se utilizará el formato rst. ([rst cheat sheet](https://docs.typo3.org/m/typo3/docs-how-to-document/main/en-us/WritingReST/CheatSheet.html))
Todos los archivos de documentación se ubican dentro de la carpeta /docs.
Para agregar imágenes, crear una carpeta images en el mismo path donde se encuentra el archivo .rst que están creando.

