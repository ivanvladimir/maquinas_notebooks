# maquinas notebooks

```
  ███╗   ███╗ █████╗  ██████╗ ██╗   ██╗██╗███╗   ██╗ █████╗ ███████╗
  ████╗ ████║██╔══██╗██╔═══██╗██║   ██║██║████╗  ██║██╔══██╗██╔════╝
  ██╔████╔██║███████║██║   ██║██║   ██║██║██╔██╗ ██║███████║███████╗
  ██║╚██╔╝██║██╔══██║██║▄▄ ██║██║   ██║██║██║╚██╗██║██╔══██║╚════██║
  ██║ ╚═╝ ██║██║  ██║╚██████╔╝╚██████╔╝██║██║ ╚████║██║  ██║███████║
  ╚═╝     ╚═╝╚═╝  ╚═╝ ╚══▀▀═╝  ╚═════╝ ╚═╝╚═╝  ╚═══╝╚═╝  ╚═╝╚══════╝

                a            b
   ──▶ ( q0 ) ────▶ ( q1 ) ────▶ (( q2 )) ──┐
                                    ▲       │
                                    └───────┘ a,b
          notebooks · lenguajes formales y autómatas
```

[![Python](https://img.shields.io/badge/python-3.12%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![uv](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/uv/main/assets/badge/v0.json)](https://github.com/astral-sh/uv)
[![JupyterLab](https://img.shields.io/badge/JupyterLab-4.x-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![maquinas](https://img.shields.io/badge/maquinas-GitLab-FC6D26?logo=gitlab&logoColor=white)](https://gitlab.com/ivanvladimir/maquinas)
[![Último commit](https://img.shields.io/github/last-commit/ivanvladimir/maquinas_notebooks)](https://github.com/ivanvladimir/maquinas_notebooks/commits/main)
[![Curso LFyA](https://img.shields.io/badge/curso-LFyA%20·%20UNAM-003D79)](https://turing.iimas.unam.mx/~ivanvladimir/page/curso_lfya/)

Estas notebooks ilustran el uso de la librería
[**maquinas**](https://gitlab.com/ivanvladimir/maquinas) para el curso
[Lenguajes Formales y Autómatas](https://turing.iimas.unam.mx/~ivanvladimir/page/curso_lfya/):
autómatas finitos, autómatas de pila, gramáticas, máquinas de Turing y la
jerarquía de Chomsky, con visualizaciones y animaciones.

## Instalación y uso

El proyecto usa [**uv**](https://docs.astral.sh/uv/) para manejar Python y
las dependencias. Si aún no lo tienes:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Clona el repositorio, instala las dependencias y abre JupyterLab:

```bash
git clone https://github.com/ivanvladimir/maquinas_notebooks.git
cd maquinas_notebooks
uv sync
uv run jupyter lab
```

`uv sync` crea el entorno virtual (`.venv`) con la versión de Python
indicada en `.python-version` e instala exactamente las versiones fijadas en
`uv.lock`, incluyendo `maquinas` directamente desde su
[repositorio en GitLab](https://gitlab.com/ivanvladimir/maquinas). Después ve al navegador y explora las notebooks.

> **Tip:** para actualizar las dependencias usa `uv lock --upgrade && uv sync`.

## Notebooks disponibles

| Carpeta          | Contenido                                                                                                          |
|------------------|--------------------------------------------------------------------------------------------------------------------|
| `lfya/`          | Sesiones del curso [Lenguajes Formales y Autómatas](https://turing.iimas.unam.mx/~ivanvladimir/page/curso_lfya/), de lenguajes y palabras hasta máquinas con cinta |
| `basic/`         | Interfaz común de máquinas y gramáticas en `maquinas`                                                               |
| `advanced/`      | Ejemplos avanzados: minimización de AFD, gramáticas ambiguas, parsing tipo Earley/SPPF, lenguajes no libres de contexto |
| `visualization/` | Temas y emojis para visualizar máquinas                                                                             |
| `seccion4/`      | Material de revisión de la sección cuatro                                                                           |
