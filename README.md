```text
https://github.com/{user}/{name_repo}
├─ README.md
├─ .gitignore
├─ .editorconfig
├─ .env.example
│
├─ docs/
│  ├─ 00-overview/
│  ├─ 01-requirements/
│  ├─ 02-api/
│  ├─ 03-user-manual/
│  ├─ 04-dev-guide/
│  └─ assets/                # imágenes, diagramas, capturas
│
├─ architecture/
│  ├─ model-database/
│  ├─ diagrams/
│  ├─ uml/
│  ├─ decisions/
│  └─ contracts/
│
├─ app/
│  └─ README.md
│
├─ api/
│  └─ README.md
│
├─ deploy/
│  ├─ docker/
│  ├─ kubernetes/            # si aplica
│  └─ compose.yaml
│
├─ scripts/
│  ├─ dev/
│  ├─ db/
│  └─ jenkins/               # scripts auxiliares del pipeline (opcional)
│
└─ cicd/
   └─ jenkins/
      ├─ Jenkinsfile          # pipeline principal
      ├─ Jenkinsfile.app      # opcional
      └─ Jenkinsfile.api      # opcional
```

### Tipos de Commit

| Figura | Name      | Description                                                   | Ejemplo |
|--------|----------|---------------------------------------------------------------|----------|
| ✨ | `feat`     | Nueva funcionalidad para el usuario o el negocio.              | `feat(app): add inventory scan screen` |
| 🐛 | `fix`      | Corrección de un bug.                                          | `fix(api): prevent negative stock values` |
| 📝 | `docs`     | Cambios solo de documentación.                                 | `docs(readme): add repo structure and commit guide` |
| 🎨 | `style`    | Cambios de formato/estilo sin afectar la lógica.               | `style(api): run gofmt on handlers` |
| ♻️ | `refactor` | Refactorización sin cambiar comportamiento.                    | `refactor(api): split inventory service layer` |
| ⚡ | `perf`     | Mejora de rendimiento.                                         | `perf(api): optimize stock listing query` |
| ✅ | `test`     | Agregar o modificar pruebas.                                   | `test(api): add inventory service unit tests` |
| 🔧 | `chore`    | Tareas de mantenimiento o configuración.                       | `chore(deploy): update docker base image` |
| 🏗️ | `build`    | Cambios en dependencias o sistema de compilación.              | `build(api): update go modules` |
| 🚀 | `ci`       | Cambios en integración continua (Jenkins, pipelines).          | `ci(cicd): add multibranch Jenkins stages` |
| ⏪ | `revert`   | Reversión de un commit anterior.                               | `revert: undo feat(app): add offline mode` |
