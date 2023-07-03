1. Склонируйте репозиторий через **git clone**
2. Откройте терминал **cmd**
3. Перейдите в директорию склонированного проекта командой **cd**
4. Проверьте, что у вас установлен питон командой **python --version**, если не установлен - установите
5. Установите виртуальное окружение командой **python -m venv venv**
6. Активируйте виртуалку командой **.\venv\Scripts\activate.bat**, слева в командной строке должна появиться приписка (venv)
   ![image](https://github.com/Andrey-Savitskiy/Shoulders_of_giants_admin/assets/93083814/044e722b-6cd4-4920-8d51-76157cc1d01d)
7. Установите Django командой **pip install -r requirements.txt**
8. Проверьте версию Django командой **python -m django --version**, должно вывести 2.2
9. Командой **python .\npg\manage.py runserver** запустите сервер, если вывело ![image](https://github.com/Andrey-Savitskiy/Shoulders_of_giants_admin/assets/93083814/b28de1c4-0566-4777-9db5-088ac018479b)
,то все в порядке. остановите сервер сочетанием **ctrl + C**
10. Создайте первичные миграции командой **python .\npg\manage.py migrate**
11. Создайте суперпользователя командой **python .\npg\manage.py createsuperuser**:
    1. Введите в имя пользователя **admin**
    2. Пропустите ввод почты нажатием enter
    3. Введите пароль **admin**
    4. Повторите пароль
    5. Введите **y**, должна появиться надпись **Superuser created successfully.**
12. Повторите **пункт 9** и запустите сервер.
13. Откройте браузер, в строку поиска введите **http://127.0.0.1:8000/admin**
14. Введите данные, только что созданного пользователя. Если вы попали в административную панель - значит все сделали верно.
15. HTML/CSS исходники админки находятся по пути **venv/Lib/site-packages/django/contrib/admin**, папки **templates** и **static/css**
16. *МЕНЯТЬ ЭТИ ФАЙЛЫ НЕ НУЖНО*, нужно создавать копии этих файлов по адресу **project/templates/admin** и **project/static/css**, подробнее можно найти информацию [здесь](https://www.youtube.com/watch?v=6jyl85q6yRs)
