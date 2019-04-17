### Что делать, чтобы залить существующий проект на существующий репозиторий на github? 

```
cd existing-project
git init
git add --all
git commit -m "Initial Commit"
git remote add origin ssh://git@github.com:alenaprideina/c02-mobile_app_automator.git
```      
или 
```
git remote set-url origin https://github.com/alenaprideina/c02-mobile_app_automator.git
git push origin master
```

---

### Посмотреть связанные удаленные репозитории: 
`git remote -v`

---

### Как отменить rebase

https://ru.stackoverflow.com/questions/590814/git-%D0%BE%D1%82%D0%BA%D0%B0%D1%82%D0%B8%D1%82%D1%8C-rebase

---

### Синхронизация fork-a на github с основным репозиторием

https://medium.com/@shanhaichik/%D1%81%D0%B8%D0%BD%D1%85%D1%80%D0%BE%D0%BD%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F-fork-a-%D0%BD%D0%B0-github-%D1%81-%D0%BE%D1%81%D0%BD%D0%BE%D0%B2%D0%BD%D1%8B%D0%BC-%D1%80%D0%B5%D0%BF%D0%BE%D0%B7%D0%B8%D1%82%D0%BE%D1%80%D0%B8%D0%B5%D0%BC-47565bd37385
