# Commands

Bu yerda Back-end uchun kerakli buyruqlarni topishingiz mumkin.
<br/><br/>
## Django==4.0
Djangoni o'rnatish va ishga tushirish

### Vertuval muhidni yaratish va Djangoni o'rnatish

<hr/>

### pipenv
Agar siz [pipenv](https://pipenv.pypa.io/en/latest/)dan foydalanmoqchi bo'lsangiz quyidagi buyruqni ishlatasiz.

```cmd
pip install pipenv
```
- Agar xatolik chiqsa
```cmd
py -m pip install pipenv
```
- Keyin esa
```cmd
pipenv shell
```
- Agar xatolik chiqsa
```cmd
py -m pipenv shell
```
- Keyin esa
```cmd
pipenv install django==4.0
```
- Agar xatolik chiqsa
```cmd
py -m pipenv install django==4.0
```
- Vertuval muhitdan chiqish
```cmd
exit
```
<hr/>

### pip
Agar siz [venv](https://docs.python.org/3/library/venv.html)dan foydalanmoqchi bo'lsangiz quyidagi buyruqni ishlatasiz.

```cmd
python3 -m venv project_name
```
- Keyin esa
```cmd
course project_name/bin/activate
```
- Keyin esa
```cmd
pip install django==4.0
```
- Vertuval muhitdan chiqish
```cmd
deactivate
```
<hr/>

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
- Sizda quyidagi ranimdek natija chiqishi kerak 
<img width="820" alt="1-26" src="https://github.com/Javohir-dev/commands/assets/97449821/973e4ebb-5730-4186-81db-eed3ad086973">

<br/><br/><br/><br/><br/><br/><br/>
# Celery
## Run CELERY

```cmd
celery -A project_name worker --loglevel=info
```
