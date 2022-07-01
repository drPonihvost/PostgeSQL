Создать .env.db файл с переменными:
- POSTGRES_DB = Имя базы данных
- POSTGRES_USER = Юзер
- POSTGRES_PASSWORD = Пароль
- PGDATA = Физическое размещение БД (/var/lib/postgresql/data/pgdata)

Создать .env.pgadmin файл с переменными:
PGADMIN_DEFAULT_EMAIL= email
PGADMIN_DEFAULT_PASSWORD= password
PGADMIN_CONFIG_SERVER_MODE= Режим сервера (False)


Start
docker-compose --project-name="myproject-pg" up -d

Stop
docker-compose --project-name="myproject-pg" down

Access to PgAdmin
Open in browser http://localhost:5050