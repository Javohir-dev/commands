# Commands

Bu yerda Back-end uchun kerakli buyruqlarni topishingiz mumkin.

# Django==4.0
Djangoni o'rnatish va ishga tushirish

### Vertuval muhidni yaratish va Djangoni o'rnatish

- pipenv
Agar siz [pipenv](https://pipenv.pypa.io/en/latest/)dan foydalanmoqchi bo'lsangiz quyidagi buyruqni ishlatasiz.

1.
```cmd
pip install pipenv
```
1. Agar xatolik chiqsa
```cmd
py -m pip install pipenv
```
2.
```cmd
pipenv shell
```
2. Agar xatolik chiqsa
```cmd
py -m pipenv shell
```
3.
```cmd
pipenv install django==4.0
```
3. Agar xatolik chiqsa
```cmd
py -m pipenv install django==4.0
```
- Vertuval muhitdan chiqish
```cmd
exit
```
- pip
Agar siz [venv](https://docs.python.org/3/library/venv.html)dan foydalanmoqchi bo'lsangiz quyidagi buyruqni ishlatasiz.

1.
```cmd
python3 -m venv project_name
```
2.
```cmd
course project_name/bin/activate
```
3.
```cmd
pip install django==4.0
```
- Vertuval muhitdan chiqish
```cmd
deactivate
```

### Djangoni ishga tushirish

1. Kerakli file va papkalarni yaratish
```cmd
django-admin startproject project_name .
```
2. Dastlabki migratsiyalarni ishga tushirish
```cmd
python manage.py migrate
```
- Va siz yangi "dbsqlite3" faylini ko'rishingiz mumkin, bu fayl ma'lumotlar bazasi vazifasini bajaradi
3. Endi siz loyihani yurgazishingiz mumkin
```cmd
python manage.py runserver
```
- Siga shunga o'xshash textlar chiqadi bu loyihangiz ishlayotganini bildiradi
```
$ python manage.py runserver
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
August 25, 2023 - 23:02:24
Django version 4.0, using settings 'your-project.settings'
Starting development server at http://localhost:8000/
Quit the server with CTRL-BREAK.

```
4. Shuni copy qiling va o'z browseringizda oching



## Run CELERY

```cmd
celery -A project_name worker --loglevel=info
```
