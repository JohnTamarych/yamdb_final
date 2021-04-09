# yamdb_final
yamdb_final

# workflow status
![example workflow](https://github.com/johntamarych/yamdb_final/actions/workflows/yamdb_workflow.yaml/badge.svg)


# о чём проект:
Проект **YaMDb** собирает отзывы пользователей на произведения. 
Произведения делятся на категории: «Книги», «Фильмы», «Музыка».

# что нужно иметь, чтобы его запустить:
Docker: https://docs.docker.com/engine/install/ubuntu/- automatic! 
Docker-compose: https://docs.docker.com/compose/install/- automatic!

# установка окружения:
1) необходимо скопировать локально репозиторий проекта
2) создать в рабочей директории файл `.env`(в случае развертывания через workflow прописать переменные в GH secrets)
3) заполнить файл `.env`, пользуясь шаблоном из файла `.env.example`

# как запустить и как увидеть, что проект работает:
`docker-compose up`
Миграции: `docker-compose run web python manage.py migrate`
Сборка статики: `docker-compose run web python manage.py dumpdata > fixtures.json`
Создание админа: `docker-compose run web python manage.py createsuperuser`

# Технологии:
Postgresql 10.6: https://www.postgresql.org/download/- automatic!
Guinicorn 20.0.4: https://docs.gunicorn.org/en/stable/install.html- automatic!
Ngnix 1.19.8: https://www.nginx.com/resources/wiki/start/topics/tutorials/install/- automatic!

# коротко об авторе
My GitHub: https://github.com/JohnTamarych- automatic!