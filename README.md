# 🚀 Curso de Git y GitHub - MoureDev

En este repositorio comparto mi progreso, apuntes y prácticas desarrolladas a lo largo del **Curso de Git y GitHub desde Cero** impartido por Brais Moure ([MoureDev](https://youtube.com/@mouredev)) en su canal de YouTube.

El objetivo de este proyecto es asimilar los conceptos fundamentales del control de versiones, aprender a gestionar repositorios de manera eficiente y aplicar buenas prácticas en el flujo de trabajo de desarrollo y ciberseguridad.

---

## 🛠️ Tecnologías y Conceptos Aprendidos

* **Control de Versiones:** Inicialización de repositorios (`git init`), gestión del ciclo de vida de los archivos (`git status`, `git add`, `git commit`).
* **Historial y Ramas:** Navegación por el historial de cambios (`git log`) y gestión de ramas (`git branch`, `git checkout/switch`).
* **Sincronización Remota:** Conexión y subida de proyectos a GitHub (`git remote`, `git push`, `git pull`).

---

## 🔐 Aprendizaje: Resolución de Problemas

Como parte del proceso de aprendizaje práctico en un entorno Linux, me enfrenté al error clásico de autenticación:
`git@github.com: Permission denied (publickey).`

### ¿Cómo se solucionó?
En lugar de utilizar la autenticación tradicional por HTTPS, opté por configurar un entorno más seguro utilizando **claves criptográficas SSH**:

1.  **Generación de credenciales:** Creé un par de llaves asimétricas.
2.  **Vinculación con GitHub:** Registré la clave pública en mi perfil de GitHub.
3.  **Enrutamiento del repositorio:** Corregí el destino remoto del repositorio local utilizando el comando:
    ```bash
    git remote set-url origin git@github.com:
    ```
4.  **Resultado:** Conexión segura, cifrada y automatizada establecida con éxito.
