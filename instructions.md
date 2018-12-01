Что делать, чтобы залить существующий проект на существующий репозиторий на github? 


  cd existing-project
  
  
  git init
  
  
  git add --all
  
  
  git commit -m "Initial Commit"
  
  
      git remote add origin ssh://git@github.com:alenaprideina/c02-mobile_app_automator.git
      
      
    или 
    
    
      git remote set-url origin https://github.com/alenaprideina/c02-mobile_app_automator.git
      
      
  git push origin master


Посмотреть связанные удаленные репозитории:
  remote -v


--


Как отменить rebase


https://ru.stackoverflow.com/questions/590814/git-%D0%BE%D1%82%D0%BA%D0%B0%D1%82%D0%B8%D1%82%D1%8C-rebase
