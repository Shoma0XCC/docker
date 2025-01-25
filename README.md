# Docker
<h3>Работа с docker, docker-compose</h3>
<h3>Работа с фоновыми задачами с помощью redis,celery,beat</h3>

<h4>Скачайте zip-file или используйте команду git clone</h4>

```
git clone https://github.com/Shoma0XCC/docker.git
```

<h4>Так же вам понадобиться docker-desktop</h4>

```
https://www.docker.com/products/docker-desktop/
```

# Setup

<h3>После установки создаем виртуальное окружение</h3>
#Mac

```
python3 -m venv venv
source venv/bin/activate
```

#Windows

```
python3 -m venv venv
.\venv\Scripts\activate.bat
```

<h3>Устанавливаем зависимости</h3>

```
pip install --upgrade pip
pip install -r requirements.txt
```

<h3>Делаем миграцию БД. Создаем админа</h3>

```
python manage.py migrate
python manage.py createsuperuser
```


<h3>Собираем контейнеры</h3>

```
docker compose build
```

<h3>И запускаем в автономном режиме</h3>

```
docker compose up -d 
```

# Работа приложения
<h4>После запуска контейнеров переходим на адрес</h4> 

```
http://localhost:8000/
``` 
<h4>Можно создать пользователя или войти в уже созданый акаунт</h4>
<h4>При нажатие на кнопку в логах контейнера my-celery-container вы увидите отсчет  от 1 до 10 по окончанию надпись Task completed!</h4>
<h4>Выполненые или команды которые находятся в процессе можно посмотреть в реальном по адресу</h4>

```
http://localhost:5555/
```











