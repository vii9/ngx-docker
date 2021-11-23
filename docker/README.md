# Using Docker for Laravel App
`Nginx & debian linux & php7.4-fpm & nodejs & composer & supervisord & mysql5.7`

## How to work
```
1 - clone from github 
  cd in current folder project
    $ mkdir docker && cd docker
    $ git clone ...
2 - config
  .env file
    - change (a) => name folder working directory
    - (b) => mysql config database name and pass root
  
  docker-compose.yml file
    - change (c) => folder working directory where contains all code your project

  ngxfpm/default.conf file
    - (d) => change to where contains index.php file
    - (e) => change it and add in file hosts
3 - start
  $ cd docker
  $ ./up.sh
4 - end
  $ cd docker
  $ ./down.sh
5 - mysql tools connection
  open port _:33066  
```