-------Docker----------
docker pull hello-world
docker run hello-world
------Docker/SQL-SERVER-----------
docker pull mcr.microsoft.com/mssql/server
docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=Passw0rD" -p 14033:1433 --name sql1 -h sql1 -d -v C:\Users\a875714\Documents\campus-git-docker\data:\var\opt\mssql\data mcr.microsoft.com/mssql/server
------GIT-------------------------
git remote add campus-git-docker https://github.com/Diego-Valdiviezo-S/campus-git-docker.git
git push --set-upstream campus-git-docker master
git status
git commit -m "mensaje"
git push
