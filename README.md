# Learn_Git

## Introduccion a los comandos de git
### git commit;
+ ![imagen1](/img/01.png)

## Creando ramas en Git
### git branch bugfix;
### git checkout bugfix;
+ ![imagen1](/img/02.png)

## Haciendo merge en Git
###### git checkout -b bugFix;
### git commit;
### git checkout main;
### git commit;
### git merge bugFix;
+ ![imagen1](/img/03.png)

## Introduccion a rebase
### git branch bugfix;
### git checkout bugfix;
### git commit;
### git checkout main;
### git commit;
### git checkout bugfix;
### git rebase main;
+ ![imagen1](/img/04.png)

## Desatachea tu head
### git checkout C4;
+ ![imagen1](/img/05.png)

## Referencias relativas 
### git checkout C4^;
+ ![imagen1](/img/06.png)

## El operador "~"
### git branch -f main C6;
### git branch -f bugfix C0;
### git checkout C1;
+ ![imagen1](/img/07.png)

## Revirtiendo cambios en Git
### git reset local~1;
### git checkout pushed;
### git revert pushed;
+ ![imagen1](/img/08.png)

## Introduccion a cherry-pick
### git cherry-pick C3 C4 C7;
+ ![imagen1](/img/09.png)

## Introduccion al rebase interactivo
### git rebase -i main~4 --aboveAll;
+ ![imagen1](/img/010.png)

## Tomando un unico commit
### git checkout main;
### git cherry-pick C4;
+ ![imagen1](/img/011.png)

## Haciendo malabares con los commits
### git rebase -i HEAD~2; 
### git commit --amend;
### git rebase -i HEAD~2;
### git rebase caption main;
+ ![imagen1](/img/012.png)

## Haciendo malabares con los commits II
### git checkout main;
### git cherry-pick C2;
### git commit --amend;
### git cherry-pick C3;
+ ![imagen1](/img/013.png)

## Tags en Git
### git tag v0 C1;
### git tag v1 C2;
### git checkout C2;
+ ![imagen1](/img/014.png)

## Git describe
### git commit;
+ ![imagen1](/img/015.png)

## Rebaseando mas de 9000 veces
### git rebase main bugFix;
### git rebase bugFix side;
### git rebase side another;
### git rebase another main;
+ ![imagen1](/img/016.png)

## Multiples padres
### git branch bugWork main~^2~;
+ ![imagen1](/img/017.png)

## Ensalada de ramas
### git checkout one;
### git cherry-pick C4 C3 C2;
### git checkout two;
### git cherry-pick C5 C4 C3 C2;
### git branch -f three C2;
+ ![imagen1](/img/019.png)