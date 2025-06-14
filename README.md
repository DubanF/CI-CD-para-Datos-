# CI/CD para Proyecto de Ingeniería de Datos

Este repositorio contiene scripts Python ETL, pruebas automáticas y un pipeline de integración continua.

## 🔧 ¿Qué hace el pipeline?

El pipeline se ejecuta automáticamente en cada push o pull request a la rama `main`, y realiza:

1. ✅ Instalación de dependencias (`requirements.txt`)
2. ✅ Ejecución de pruebas con `pytest`
3. ✅ Validación del código con `flake8`
4. ✅ Generación de documentación con `pdoc` en la carpeta `docs/`

## 🚀 ¿Cómo se ejecuta?

No necesitas hacer nada manualmente. El pipeline se lanza automáticamente al hacer `git push` o abrir un pull request a `main`.

Puedes revisar el estado en la pestaña **Actions** del repositorio.

## 📂 Estructura recomendada

\`\`\`
CI-CD-para-Datos-/
│
├── src/                  # Código fuente (ETL scripts)
│   └── etl.py
├── tests/                # Pruebas automatizadas
│   └── test_etl.py
├── docs/                 # Documentación generada (no editar manualmente)
├── requirements.txt
└── .github/
    └── workflows/
        └── ci.yml        # Pipeline CI/CD
\`\`\`

## 📄 Requisitos

- Python 3.10
- pytest
- flake8
- pdoc

Puedes instalar localmente con:

\`\`\`bash
pip install -r requirements.txt
\`\`\`
