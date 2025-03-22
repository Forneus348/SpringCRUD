### Если у кого-то есть предложения по проекту, то готов их обсудить😁
### Это CRUD-приложение на Java, используемые технологии:
  - Spring Boot для создания API
  - Spring Data для упрощения взаимодействия с бд
  - Hibernate как ORM-система
  - Maven для сборки приложения
  - PostgreSQL для хранения данных
  - Postman для тестирования http-запросов
  - Docker для запуска бд
  - Intellij IDEA для написания кода
### Работа с проектом:
1. Клонирование репозитория:
<pre class="language-bash"><code>git clone git@github.com:Forneus348/SpringCRUD.git</code></pre>
2. Создание Docker-образа:
<pre class="language-bash"><code>docker run --name demo-api -e POSTGRES_PASSWORD=12345678 -p 5432:5432 -d postgres</code></pre>
3. Создание бд (я использовал pgAdmin):
    - Name: demo-api
    - Host name/address: 127.0.0.1
    - Maintenance database: postgres
    - Username: postgres
5. Создание таблицы:
<pre class="language-bash"><code>CREATE TABLE IF NOT EXISTS public.users
(
    id bigint NOT NULL DEFAULT nextval('users_id_seq'::regclass),
    name character varying(255) COLLATE pg_catalog."default",
    email character varying(255) COLLATE pg_catalog."default",
    birth date,
    age integer,
    CONSTRAINT users_pkey PRIMARY KEY (id)
)</code></pre>
6. Запуск проекта
    
