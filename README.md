# Learn_Git

## Introduccion a los comandos de git
#### git commit;
+ ![imagen1](/img/a.png)

## Creando ramas en Git
#### git branch bugfix;
#### git checkout bugfix;
+ ![imagen1](/img/b.png)

## Haciendo merge en Git
#### git checkout -b bugFix;
#### git commit;
#### git checkout main;
#### git commit;
#### git merge bugFix;
+ ![imagen1](/img/c.png)

## Introduccion a rebase
#### git branch bugfix;
#### git checkout bugfix;
#### git commit;
#### git checkout main;
#### git commit;
#### git checkout bugfix;
#### git rebase main;
+ ![imagen1](/img/d.png)

## Desatachea tu head
#### git checkout C4;
+ ![imagen1](/img/e.png)

## Referencias relativas 
#### git checkout C4^;
+ ![imagen1](/img/f.png)

## El operador "~"
#### git branch -f main C6;
#### git branch -f bugfix C0;
#### git checkout C1;
+ ![imagen1](/img/g.png)

## Revirtiendo cambios en Git
#### git reset local~1;
#### git checkout pushed;
#### git revert pushed;
+ ![imagen1](/img/h.png)

## Introduccion a cherry-pick
#### git cherry-pick C3 C4 C7;
+ ![imagen1](/img/i.png)

## Introduccion al rebase interactivo
#### git rebase -i main~4 --aboveAll;
+ ![imagen1](/img/j.png)

## Tomando un unico commit
#### git checkout main;
#### git cherry-pick C4;
+ ![imagen1](/img/k.png)

## Haciendo malabares con los commits
#### git rebase -i HEAD~2; 
#### git commit --amend;
#### git rebase -i HEAD~2;
#### git rebase caption main;
+ ![imagen1](/img/l.png)

## Haciendo malabares con los commits II
#### git checkout main;
#### git cherry-pick C2;
#### git commit --amend;
#### git cherry-pick C3;
+ ![imagen1](/img/ll.png)

## Tags en Git
#### git tag v0 C1;
#### git tag v1 C2;
#### git checkout C2;
+ ![imagen1](/img/m.png)

## Git describe
#### git commit;
+ ![imagen1](/img/n.png)

## Rebaseando mas de 9000 veces
#### git rebase main bugFix;
#### git rebase bugFix side;
#### git rebase side another;
#### git rebase another main;
+ ![imagen1](/img/o.png)

## Multiples padres
#### git branch bugWork main~^2~;
+ ![imagen1](/img/p.png)

## Ensalada de ramas
#### git checkout one;
#### git cherry-pick C4 C3 C2;
#### git checkout two;
#### git cherry-pick C5 C4 C3 C2;
#### git branch -f three C2;
+ ![imagen1](/img/q.png)