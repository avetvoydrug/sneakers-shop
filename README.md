# Магазин кросовок
# Телеграм бот на aiogram3 + Postgresql
### Как запустить проект:

- Установить Postgresql на Ваш пк;
- Клонировать репозиторий и перейти в него в командной строке:
    ```
    git clone https://github.com/avetvoydrug/sneakers-shop.git
    ```
    ```
    cd sneakers-shop
    ```
- Cоздать и активировать виртуальное окружение:
    ```
    python -m venv env
    ```
    ```
    .\venv\Scripts\activate
    ```

- Установить зависимости из файла requirements.txt:
    ```
    pip install -r requirements.txt
    ```
- Создать базу данных в pgAdmin
- Создать тг-бота через @BotFather в тг
- Создать в директории sneakers-shop файл .env:
    - в нём cоздать константу TOKEN=токен_вашего_бота
    - на следующей строке создать константу SQLALCHEMY_URL=postgresql+asyncpg://user:password@host:port/dbname...
    - внести свои данные в user, password, host, dbname
- Запустить бота
    ```
    python main.py
    ```