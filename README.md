# Repo-de-prueba-grupal
Repositorio creado para para practicar el flujo de trabajo GITFLOW con 6 colaboradores

## Ramas en GitFlow
- `main`: Contiene la versión estable del proyecto.
- `develop`: Rama de desarrollo donde se integran los cambios.
- `feature/nombre`: Ramas para nuevas funcionalidades.
- `release/nombre`: Ramas para preparar versiones.
- `hotfix/nombre`: Ramas para corregir errores críticos en producción.

## ¿Cómo contribuir?
1. Clonar el repositorio:  
   ```bash
   git clone URL_DEL_REPO

---------------------------------------------------------------------------------
¿Como mantener el CÓDIGO ACTUALIZADO?
---------------------------------------------------------------------------------
***PARA ACTUALIZAR LA RAMA-TAREA CON LOS CAMBIOS DE MAIN***
-----------------
¿Por qué se hace?
Si otras personas han hecho cambios en main, necesitas traerlos a tu rama (auth-feature) para evitar conflictos más adelante
-----------------
git checkout main	        // Entro a la RAMA PRINCIPAL
git pull origin main      // SE TRAEN los últimos cambios de main
git checkout feature/auth	// Me cambio a la RAMA-TAREA (ej: feature/auth)
git merge main            // Traigo los cambios de la RAMA PRINCIPAL a la RAMA-TAREA

---------------------------------------------------------------------------------

***PARA INTEGRAR LA RAMA-TAREA, UNA VEZ FINALIZDA, A MAIN***
-----------------
¿Por qué se hace?
Cuando finalizas una tarea en auth-feature, necesitas integrar esos cambios en main para que formen parte del código principal.
-----------------
git checkout main         // Me cambio a la RAMA PRINCIPAL
git pull origin main      // Me aseguro de que main está actualizado
git merge feature/auth    // Fusiono los cambios de feature/auth en main
git push origin main      // Subo los cambios a GitHub
