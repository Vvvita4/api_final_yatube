# API для Yatube

## Описание
Этот проект представляет собой API для социальной сети Yatube, позволяющий пользователям создавать посты, комментировать их, подписываться на других пользователей и работать с группами. API разработан с использованием Django REST Framework и обеспечивает аутентификацию через JWT-токены.

## Установка
1. Клонируйте репозиторий:  

2. Перейдите в директорию проекта:  
   `cd api_final_yatube`

3. Создайте и активируйте виртуальное окружение:  
   `python -m venv venv`  
   `source venv/bin/activate` (на Unix) или `venv\Scripts\activate` (на Windows)

4. Установите зависимости:  
   `pip install -r requirements.txt`

5. Выполните миграции:  
   `python manage.py migrate`

6. Запустите сервер:  
   `python manage.py runserver`

## Примеры запросов
### Получение токена (JWT)
- **Метод:** POST  
- **URL:** `/api/v1/jwt/create/`  
- **Тело запроса:**  
  ```json  
  {  
    "username": "your_username",  
    "password": "your_password"  
  }  