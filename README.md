# docker-wordpress

ls
    2  cd /etc/sudoers.d/
    3  ls
    4  cp 90-cloud-init-users 110-app-users
    5  vi 110-app-users
    6  sudo su app
    7  man useradd
    8  grep docker /etc/passwd
    9  useradd -m docker
   10  grep /etc/passwd
   11  grep docker /etc/passwd
   12  useradd -m app
   13  usermod -aG sudo app
   14  cd
   15  cd /etc/sudoers.d/
   16  ls
   17  rm 110-app-users
   18  sudo su app
   19  echo "app  ALL=(ALL) NOPASSWD:ALL" | sudo tee /etc/sudoers.d/app
   20  ls
   21  more app
   22  ls
   23  mv app 110-user-app
   24  ls -l
   25  chmod 440 110-user-app
   26  sudo su app
   27  history
