# Learn_Git

## Introduccion a los comandos de git
### git commit;

## Creando ramas en Git
### git branch bugfix;
### git checkout bugfix;

## Haciendo merge en Git
### git checkout -b bugFix;
### git commit;
### git checkout main;
### git commit;
### git merge bugFix;

## Introduccion a rebase
### git branch bugfix;
### git checkout bugfix;
### git commit;
### git checkout main;
### git commit;
### git checkout bugfix;
### git rebase main;

## Desatachea tu head
### git checkout C4;

## Referencias relativas 
### git checkout C4^;

## El operador "~"
### git branch -f main C6;
### git branch -f bugfix C0;
### git checkout C1;

## Revirtiendo cambios en Git
### git reset local~1;
### git checkout pushed;
### git revert pushed;

## Introduccion a cherry-pick
### git cherry-pick C3 C4 C7;

## Introduccion al rebase interactivo
### git rebase -i main~4 --aboveAll;

## Tomando un unico commit
### git checkout main;
### git cherry-pick C4;

## Haciendo malabares con los commits
### git rebase -i HEAD~2; 
### git commit --amend;
### git rebase -i HEAD~2;
### git rebase caption main;

## Haciendo malabares con los commits II
### git checkout main;
### git cherry-pick C2;
### git commit --amend;
### git cherry-pick C3;

## Tags en Git
### git tag v0 C1;
### git tag v1 C2;
### git checkout C2;

## Git describe
### git commit;

## Rebaseando mas de 9000 veces
### git rebase main bugFix;
### git rebase bugFix side;
### git rebase side another;
### git rebase another main;

## Multiples padres
### git branch bugWork main~^2~;

## Ensalada de ramas
### git checkout one;
### git cherry-pick C4 C3 C2;
### git checkout two;
### git cherry-pick C5 C4 C3 C2;
### git branch -f three C2;