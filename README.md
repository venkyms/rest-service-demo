git init

git status

git add .

git status

git commit -m "initial commit for rest service demo"

git remote add origin https://github.com/venkyms/rest-service-demo.git


git push -u origin master #----> did not work for the first time

git push origin main #----> will error out for the password, generate token at https://github.com/settings/tokens


git remote set-url origin https://\<token\>@github.com/venkyms/rest-service-demo

git push origin main

git pull orgin main # ---> to pull latest


#to clone

git clone https://github.com/venkyms/rest-service-demo.git



http://localhost:8085/greeting?name=User


Set your username: git config --global user.name "FIRST_NAME LAST_NAME"
Set your email address: git config --global user.email "MY_NAME@example.com"