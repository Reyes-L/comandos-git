# comandos útiles git

1. ```git init``` // Inicia git
2. ```git add .``` o ```git add <archivo>``` // Toma la fotografia a todos los archivos y los agrega al escenario
3. ```git reset .``` // Elimina la fotografia y quita los archivos del escenario
4. ```git commit -m "mensaje de commit"``` // Crea el commit
5. ```git checkout -- .``` // restaura los cambios al ultimo commit
6. ```git log``` o ```git log --oneline``` // muestra el historial de commits
7. ```git commit --amend``` // modificar commit 
8. ```git checkout -b nueva-rama``` // Crea una nueva rama y entra en ella
9. ```git checkout main``` o ```git checkout nombre-de-rama``` // Moverme a la rama main u otra rama
10. ```git branch -d nueva-rama``` // Elimina la rama creada
11. ```git push``` // Subir el commit de git a github
12. ```git commit -am "mensaje de commit"``` // Crear fotografia y commit con un solo comando
13. ```git pull -u origin main``` // Descargar el proyecto con los ultimos cambios
14. ```git push -u origin main o otra rama``` // Subir cambios de la rama main a github
15. ```git clone remote url-de-git``` // Clona un proyecto de github
16. ```git merge nueva-rama``` // Fusiona la nueva rama a la rama main (asegurate de estar en la rama main)
17. ```git branch``` // Ver todas las ramas del repositorio
18. ```git branch -m main nuevo-nombre-de-rama``` // Cambia el nombre de la rama main a nuevo-nombre-de-rama

## Ejemplos del  merge

- Crear nueva rama: ```git checkout -b nueva-rama```
- Editar algunos archivos: ```git add <archivo>```
- Crear commit: ```git commit -m "Rama agragada"```
- Editar algunos archivos: ```git add <archivo>```
- Crear commit: ```git commit -m "Funcionalidad agregada"```
- Movernos a la rama principal: ```git checkout main```
- Fusionar nueva rama: ```git merge nueva-rama```
- Eliminar la nueva rama creada: ```git branch -d nueva-rama```

## Release
- ```git tag``` // Ver todos los tags
- ```git tag -a v1.0.0 -m "nombre de tag"``` // Crear tag
- ```git push --tags``` // Subir tags a github

## Viajes en el tiempo
- ```git reset --soft HEAD^ o Hash``` // Reestablece el historial de confirmaciones (HEAD: Confirma el objetivo)
- ```git reset --mixed codigo-de-hash``` // (no elimina cambios) Permite volver a donde estaba trabajando justo antes de su ultima confirmacion
- ```git reset --hard codigo-de-hash``` // Descarta todos los cambios no confirmados incluso si los haya agregado al stage
- ```git reflog``` // Examina un registro de donde han estado todas las cabezas de las ramas
- ```git mv destruir-mundo.md salvar-mundo.md``` // Se usa para mover un archivo o cambiarle el nombre
- ```git rm salvar-mundo.md``` // Elimina un archivo pero lo deja en el stage
