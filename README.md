## php7 + nginx + percona + symfony3 docker image

Just clone the repo and run ```docker-compose up```, your symfony aplication should be placed in symfony directory. All nginx logs will be placed in `logs` directory.

After running the container, page will be available at ```http://symfony.dev/```. 

DB credentials:
* db name: symfony
* user: root
* password: root
* host: db