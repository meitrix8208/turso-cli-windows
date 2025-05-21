# Turso CLI para Windows (Builds no oficiales)

[![Build & Release](https://github.com/meitrix8208/turso-cli-windows/actions/workflows/main.yml/badge.svg)](https://github.com/meitrix8208/turso-cli-windows/actions/workflows/main.yml)
[![License](https://img.shields.io/badge/license-MIT-blue)](https://github.com/tursodatabase/turso-cli/blob/main/LICENSE)

Este repositorio genera automáticamente **builds no oficiales del Turso CLI para Windows (turso.exe)**, basados en los tags del repositorio original [`tursodatabase/turso-cli`](https://github.com/tursodatabase/turso-cli).

Cada domingo (o manualmente), se verifica si existe una nueva versión y, si es así, se compila un ejecutable para Windows y se publica automáticamente como un [release](https://github.com/meitrix8208/turso-cli-windows/releases).

---

## 📥 Descarga rápida

Visita la [sección de releases](https://github.com/meitrix8208/turso-cli-windows/releases) para descargar la última versión disponible de `turso.exe`.

---

## 🛠️ ¿Qué es Turso CLI?

Turso CLI es una herramienta de línea de comandos para interactuar con [Turso](https://turso.tech), una base de datos distribuida optimizada para edge computing. Puedes:

- Crear y administrar bases de datos
- Ejecutar queries SQL
- Replicar datos entre regiones
- Autenticarse con GitHub, entre otras funcionalidades

Consulta la [documentación oficial](https://docs.turso.tech/reference/turso-cli) para más detalles.

---

## ⚙️ Automatización del Build

Este repositorio usa **GitHub Actions** para:

- Verificar semanalmente si existe una nueva versión (`tag`) en el repositorio oficial
- Compilar el ejecutable `turso.exe` para Windows (`GOOS=windows`, `GOARCH=amd64`)
- Publicar el ejecutable como un nuevo release

También puedes ejecutar manualmente el workflow indicando una versión específica.

---

## 🧪 Uso básico del CLI

```bash
turso auth signup      # Registrarse
turso auth login       # Iniciar sesión con GitHub
turso db create        # Crear base de datos
turso db list          # Listar bases de datos
turso db shell <db>    # Abrir consola SQL
turso db replicate <db> <region>  # Replicar base de datos
```

---

## 📝 Nota importante

⚠️ **Este proyecto NO es una distribución oficial.**  
El binario `turso.exe` generado es una **compilación no oficial** basada en el código fuente del proyecto original.

Si necesitas soporte oficial, visita el repositorio original: [tursodatabase/turso-cli](https://github.com/tursodatabase/turso-cli).

---

## 🧑‍💻 Licencia

Este proyecto sigue la [licencia MIT](https://github.com/tursodatabase/turso-cli/blob/main/LICENSE) del repositorio original.

---
