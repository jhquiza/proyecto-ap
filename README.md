# Repositorio base para los proyectos de aula de Análisis Predictivo de Datos, 2026-2

Este repositorio constituye un laboratorio educativo y profesional destinado al desarrollo, implementación y evaluación de modelos de Machine Learning. La arquitectura del proyecto está diseñada bajo principios de reproducibilidad y eficiencia técnica.

## Arquitectura Tecnológica
Para garantizar un entorno de ejecución estable y de alto rendimiento, el proyecto utiliza:
- Lenguaje: Python >=3.12
- Gestor de Entorno: `uv` para una resolución de dependencias determinista y acelerada.
- Motor de Construcción: Hatchling
- Control de Versiones: Git con integración en GitHub.

## Estructura del Repositorio
La organización del código sigue una taxonomía lógica para facilitar la escalabilidad:

- data/: Almacenamiento de datasets (locales y externos).
- notebooks/: Documentación interactiva, Análisis Exploratorio de Datos (EDA), prototipado y experimentación.
- src/: Scripts de producción, utilidades de limpieza y definiciones de modelos.
- tests/: Protocolos de prueba para asegurar la integridad del código mediante pytest.
- models/: Modelos entrenados.

## Prerrequisitos para clonar este repositorio y configurar el entorno de desarrollo localmente
Tener:
- Git instalado
- Python 3.12
- [uv](https://github.com/astral-sh/uv)
- Un IDE (recomendado VSCode)

## Instalación
#### Clonar el repositorio
```bash
git clone https://github.com/jhquiza/proyecto-ap.git
cd proyecto-ap
```
### Configurar el entorno con uv (Recomendado)
```bash
# Instalar uv si no lo tiene (en Windows)
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"

# Configuración del entorno virtual
uv sync

### Verificar la instalación
```bash
# Listar paquetes instalados
uv pip list