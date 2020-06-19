### Что делать, чтобы залить существующий проект на существующий репозиторий на github? 

```
cd existing-project
git init
git add --all
git commit -m "Initial Commit"

git remote add origin ssh://git@github.com:alenaprideina/c02-mobile_app_automator.git
# или 
git remote set-url origin https://github.com/alenaprideina/c02-mobile_app_automator.git
```
И затем `git push origin master`


Если в удаленном репозитории уже есть коммиты и при push'е возникает ошибка вида 
```
error: failed to push some refs to 'https://github.com/alenaprideina/helpful-instructions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```
то нужно подтянуть изменения из удаленного репозитория с помощью `git pull`. 


Если что-то пошло не так:
```
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
``` 
То следуя инструкциям, нужно связать локальную и удаленную ветки `git branch --set-upstream-to=origin/master master` и повторить попытку `git pull`.

В случае ошибки со следующим сообщением:
```
fatal: refusing to merge unrelated histories
```

Можно воспользоваться командой с ключом `git pull --allow-unrelated-histories` и затем все должно получиться :) 

https://help.github.com/en/articles/adding-an-existing-project-to-github-using-the-command-line
https://github.community/t5/How-to-use-Git-and-GitHub/How-to-deal-with-quot-refusing-to-merge-unrelated-histories-quot/td-p/12619

---

### Посмотреть связанные удаленные репозитории: 
`git remote -v`

---

### Как отменить rebase

https://ru.stackoverflow.com/questions/590814/git-%D0%BE%D1%82%D0%BA%D0%B0%D1%82%D0%B8%D1%82%D1%8C-rebase

---

### Синхронизация fork-a на github с основным репозиторием

https://medium.com/@shanhaichik/%D1%81%D0%B8%D0%BD%D1%85%D1%80%D0%BE%D0%BD%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F-fork-a-%D0%BD%D0%B0-github-%D1%81-%D0%BE%D1%81%D0%BD%D0%BE%D0%B2%D0%BD%D1%8B%D0%BC-%D1%80%D0%B5%D0%BF%D0%BE%D0%B7%D0%B8%D1%82%D0%BE%D1%80%D0%B8%D0%B5%D0%BC-47565bd37385

---

### Как создать ветку с конкретного коммита из другой ветки

https://ru.stackoverflow.com/questions/431520/%D0%9A%D0%B0%D0%BA-%D0%B2%D0%B5%D1%80%D0%BD%D1%83%D1%82%D1%8C%D1%81%D1%8F-%D0%BE%D1%82%D0%BA%D0%B0%D1%82%D0%B8%D1%82%D1%8C%D1%81%D1%8F-%D0%BA-%D0%B1%D0%BE%D0%BB%D0%B5%D0%B5-%D1%80%D0%B0%D0%BD%D0%BD%D0%B5%D0%BC%D1%83-%D0%BA%D0%BE%D0%BC%D0%BC%D0%B8%D1%82%D1%83
