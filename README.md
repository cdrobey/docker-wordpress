<<<<<<< HEAD
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
   28  exit
   29  ls
   30  mkdir projects
   31  cd projects/
   32  ls
   33  git clone https://github.com/cdrobey/docker-wordpress
   34  ls
   35  cd docker-wordpress/
   36  ls
   37  ls -a
   38  git pull
   39  ls
   40  cd conf
   41  ls
   42  cd traefikdynamic/
   43  ls
   44  vi services.yml
   45  vi routers.yml
=======
# docker-compose Traefik & Wordpress

> Docker stack to have a WordPress site behind a Traefik reverse-proxy with Nginx, a SQL database and Redis objects cache.

This is a prod ready stack, but it needs some customization to be powerful.

## :factory: Requirements

* linux host (tested successfully on Ubuntu 20.04, Debian 10 & 11)
* docker >= 18.x
* docker-compose >= 1.26

## :rocket: How to use

Clone this repo where you want with this line :

```bash
git clone https://github.com/Mettmett/docker-compose.git:traefik-nginx-wordpress-sql-redis
```

You need to edit the file `.env` at the source folder to modify the values of some vars.

**Important !!** You have to "sudo chmod 600" the file "acme.json", otherwise you won't be able to pull Let's Encrypt certificates.

After that when you're all set, press the red button to initiate :fire: !

```bash
docker-compose pull; docker-compose up -d; docker-compose logs -f
```

## :star: Author

Made by Julien HOMMET :fr: for [ComputerZ Solutions](https://computerz.solutions/)

* Twitter: [@_ComputerZ](https://twitter.com/_ComputerZ)
* GitHub: [Mettmett](https://github.com/Mettmett)

## :wrench: Support & Contribution

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## :moneybag: Licence

[CC BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0)

## :anchor: Misc

More info at [https://computerz.solutions/docker-compose-wordpress-nginx-et-traefik/](https://computerz.solutions/docker-compose-wordpress-nginx-et-traefik/)
>>>>>>> f119b97 (First Commit.)
