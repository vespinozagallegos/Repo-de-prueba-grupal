# Repo-de-prueba-grupal
Repositorio creado para para practicar el flujo de trabajo GITFLOW con 6 colaboradores

## Ramas en GitFlow
- `main`: Contiene la versión estable del proyecto.
- `develop`: Rama de desarrollo donde se integran los cambios.
- `feature/nombre`: Ramas para nuevas funcionalidades.
- `release/nombre`: Ramas para preparar versiones.
- `hotfix/nombre`: Ramas para corregir errores críticos en producción.

## ¿Cómo crear ramas?
Cada integrante deberá trabajar en una rama determinada según la tarea. Por ejemplo, para autenticación se creará la rama feature/auth con el siguiente comando:

- `git checkout -b feature/auth`:   feature/auth es el nombre de la rama-tarea

## ¿Cómo contribuir?
1. Clonar el repositorio:  
   ```bash
   git clone URL_DEL_REPO


# ¿Como mantener el código actualizado?

## *Pasos para actualizar la rama-tarea con los cambios de main*

¿Por qué se hace?
Si otras personas han hecho cambios en main, necesitas traerlos a tu rama-tarea (ej: feature/auth) para evitar conflictos más adelante

- `git checkout main`   :   Entro a la RAMA PRINCIPAL
- `git pull origin main`:   SE TRAEN los últimos cambios de main
- `git checkout feature/auth`:   Me cambio a la RAMA-TAREA (ej: feature/auth)
- `git merge main`:   Traigo los cambios de la RAMA PRINCIPAL a la RAMA-TAREA
- `git push origin feature/auth`:   Subo los cambios a la rama-tarea


## *Pasos para integrar la rama-tarea, una vez finalizada, a main con PULL REQUEST*
¿Por qué se hace?
Cuando finalizas tu rama-tarea (ej: feature/auth) necesitas integrar esos cambios en main para que formen parte del código principal. Con pull request integramos estos cambios desde github.

- `IR a PULL REQUESTS` --> "New Pull Request"
- `SELECCIONAR la rama-tarea (feature/auth) y comparar con la rama principal`
- `EXPLICAR los cambios y SOLICITAR REVISIÓN de otro COLABORADOR`
-	`SI TODO ESTÁ OK`
- `MERGE` --> Se fusionan las ramas