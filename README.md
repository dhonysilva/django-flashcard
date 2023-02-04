# django-flashcard
Flashcard em Django desenvolvido durante o tutorial da realpython.com

## Conteiners services
On your terminal, execute the command to run the docker-compose locally:

`docker-compose -f docker-compose-local.yml up --build`


Two conteiners will be up and running. These conteiners are descibed on docker-compose.yml.
- web
- db

## Other Commands

After setting up the conteiners, execute the following commands:

`docker-compose -f docker-compose-local.yml exec web python manage.py makemigrations` 

`docker-compose -f docker-compose-local.yml exec web python manage.py migrate`

`docker-compose -f docker-compose-local.yml exec web python manage.py createsuperuser`

At this point, riacho application will be running and with your superuser.
