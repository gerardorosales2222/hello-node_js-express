#Deploy Automático
Esto sirve para hacer un deploy automático


#GIT

INSTALAR Y CONFIGURAR GIT

sudo add-apt-repository ppa:git-core/ppa
sudo apt-get update
sudo apt-get install git
git --version

git config --global user.name "Your Name Here"
git config --global user.email "your_email@example.com"
git config --global credential.helper cache
git config --global color.ui true
git config --list


#Heroku
cd carpeta-proyecto
git init
heroku login
heroku create
heroku apps:rename nombre-proyecto
git remote add heroku https://git.heroku.com/murmuring-meadow-25196.git
git status
git add .
git commit 'el commit que hiciste'
git push heroku master
heroku rake db:migrate
heroku open



#Video Útil para Deploy Automático
https://www.youtube.com/watch?v=QUvxrzINj5Q


#Para hacer que funque el responsive: 

<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0">

[![Deploy on Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)
