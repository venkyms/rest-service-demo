git init

git status

git add .

git status

git commit -m "initial commit for rest service demo"

git remote add origin https://github.com/venkyms/rest-service-demo.git


git push -u origin master # did not work for the first time

git push origin main # will error out for the password, generate token at https://github.com/settings/tokens


git remote set-url origin https://<token>@github.com/venkyms/rest-service-demo

git push origin main

![image](https://github.com/venkyms/rest-service-demo/assets/482039/6b9e5e4d-c12e-4bb5-9cc0-872324ee7e89)
