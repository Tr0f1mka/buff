# Благотворительная платформа "Все вместе"
## Короткое описание
Веб-сайт, помогающий людям найти волонтёрские точки в своем и других городах. Удобен благодаря интерактивной карте с фильтрами.

---
# Локальный запуск

Терминал 1, Backend
```bash
source venv/bin/activate
python manage.py runserver
```

Терминал 2, Frontend
```bash
cd src
python3 -m http.server 3000
```

---
# Функционал сайта
- Авторизация / регистрация фонда, физ. лица
- Возможность оставить заявку на интерактивной карте для физ. лица
- Актуальная информация о фондах, зарегистрированных на сайте

---
# Стек
- Python, Django, Django frameworks
- YandexMapAPI
- HTML, CSS, JS
- SQLite3

---
# Структура проекта
<pre>
    .
    ├── vse_vmeste
    │   ├── api/                              # Реализатор API
    │       ├── pycache/                  
    │       ├── migrations/   
    │       ├── admin.py       
    │       ├── apps.py
    │       ├── models.py
    │       ├── serializers.py
    │       ├── tests.py
    │       ├── urls.py
    │       ├── views.py 
    │   ├── charity_platform/  
    │       ├── pycache/
    │       ├── asgi.py 
    │       ├── settings.py       
    │       ├── urls.py      
    │       ├── wsgi.py       
    │   ├── src/                               # Папка с кодом
    │       ├── images/                        # Папка с картинками(пока только логотип)
    |           ├── favicon.png                # Логотип      
    │       ├── .DS_Store
    │       ├── api.js
    │       ├── app.js
    │       ├── auth.js
    │       ├── index.html
    │       ├── map.js
    │       ├── styles.css
    │       ├── ui.js
    │   ├── venv/                              # Виртуальное окружение
    |   ├── README.md                          # Документация
    |   ├── manage.py                          # Запуск сервера на Django
    |   ├── requirements.txt  
    |   ├── start_server.sh                    # Запуск сервера
</pre>