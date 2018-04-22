ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

eval "$(ssh-agent -s)"

ssh-add ~/.ssh/id_rsa

cat ~/.ssh/id_rsa.pub

#copy this to the github setting/ssh key webpage




touch README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:alexpchin/<reponame>.git
git push -u origin master

