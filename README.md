#Practica Git Urko

**- ¿Qué comando utilizaste en el paso 11? ¿Por qué?**

git reset --hard HEAD~1

Había dos formas de hacerlo. Una con un reset --hard y otra con un reset + un checkout.

He optado por la primera opción porque estaba seguro de que quería deshacer el commit y perder los cambios en mi working copy.

**- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

reflog para listar los commits realizados
git reset <identificador_commit> para volver al commit deshecho y mover styled.
git checkout -- git-nuestro.md para recuperar la información del archivo del repo.

**- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

No causó ningún conflicto. Sale el mensaje de Already up-to-date

**- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

Si se ha producido un conflicto al haber modificado mismas líneas en el mismo archivo.

**- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

No ha producido ningún conflicto. Ha sido un merge Fast-forward.

**- ¿Qué comando o comandos utilizaste en el paso 25?**

git log --graph --decorate

**- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Si se podría haber hecho un merge Fast-forward porque no se perdería ningún commit de title al avanzar master.

**- ¿Qué comando o comandos utilizaste en el paso 27?**

git reset HEAD~1

**- ¿Qué comando o comandos utilizaste en el paso 28?**

git checkout -- git-nuestro.md

**- ¿Qué comando o comandos utilizaste en el paso 29?**

git brancg -D title

**- ¿Qué comando o comandos utilizaste en el paso 30?**

git checkout <identificador_commit> # para volver al commit del merge no flash-forward

**- ¿Qué comando o comandos usaste en el paso 32?**

git reflog # buscar el identificador del commit inicial (también su podría usar git log e ir al primero)
git checkout <identificador_commit>

**- ¿Qué comando o comandos usaste en el punto 33?**

git reflog # buscar el identificador del commit del merge
git checkout <identificador_commit>
