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
