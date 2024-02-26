# 2024-dj5-ecommerce
Membuat aplikasi ecommerce menggunakan Django versi 5.0.2


## 1. SETUP


#### 1. Inisial setup

        modified:   README.md


#### 2. Membuat virtual environment

        modified:   .gitignore
        modified:   README.md
        new file:   venv312502/Scripts/Activate.ps1
        new file:   venv312502/Scripts/activate
        new file:   venv312502/Scripts/activate.bat
        new file:   venv312502/Scripts/deactivate.bat
        new file:   venv312502/Scripts/pip.exe
        new file:   venv312502/Scripts/pip3.12.exe
        new file:   venv312502/Scripts/pip3.exe
        new file:   venv312502/Scripts/python.exe
        new file:   venv312502/Scripts/pythonw.exe
        new file:   venv312502/pyvenv.cfg


#### 3. Mengaktifkan lingkungan virtual atau venv312502

        λ REM: Mengaktifkan venv312502
        λ venv312502\Scripts\activate.bat
        C:\Users\ING\Desktop\2024-DEVSPACE\2024-dj5-ecommerce(main -> origin)
        (dj5ecom) λ


#### 4. Membuat root direktori dan memindahkan file .gitignore dan README.md ke dalamnya

        modified:   README.md


#### 5. Menginstal django versi 5.0.2

        C:\Users\ING\Desktop\2024-DEVSPACE\2024-dj5-ecommerce\root(main -> origin)
        (dj5ecom) λ pip install django==5.0.2
        ...
        Successfully installed asgiref-3.7.2 django-5.0.2 sqlparse-0.4.4 tzdata-2024.1

        [notice] A new release of pip is available: 23.2.1 -> 24.0
        [notice] To update, run: python.exe -m pip install --upgrade pip

        C:\Users\ING\Desktop\2024-DEVSPACE\2024-dj5-ecommerce\root(main -> origin)
        (dj5ecom) λ pip freeze
        asgiref==3.7.2
        Django==5.0.2
        sqlparse==0.4.4
        tzdata==2024.1


#### 6. Meng-upgrade pip

        (dj5ecom) λ python.exe -m pip install --upgrade pip
        ...
        Successfully installed pip-24.0


## 2. PROYEK DJANGO


#### 1. Memembuat proyek django

        C:\Users\ING\Desktop\2024-DEVSPACE\2024-dj5-ecommerce\root(main -> origin)
        (dj5ecom) λ django-admin

        ...
            startapp
            startproject
            test
            testserver

        (dj5ecom) λ django-admin startproject config .

        C:\Users\ING\Desktop\2024-DEVSPACE\2024-dj5-ecommerce\root(main -> origin)
        (dj5ecom) λ ls
        config/  manage.py*  README.md

        C:\Users\ING\Desktop\2024-DEVSPACE\2024-dj5-ecommerce\root(main -> origin)
        (dj5ecom) λ tree /f
        Folder PATH listing
        Volume serial number is C0000100 1A60:D2FA
        C:.
        │   .gitignore
        │   manage.py
        │   README.md
        │
        └───config
                asgi.py
                settings.py
                urls.py
                wsgi.py
                __init__.py

        modified:   README.md
        new file:   config/__init__.py
        new file:   config/asgi.py
        new file:   config/settings.py
        new file:   config/urls.py
        new file:   config/wsgi.py
        new file:   manage.py


#### 2. Menjalankan sever django atau lokal server

        C:\Users\ING\Desktop\2024-DEVSPACE\2024-dj5-ecommerce\root(main -> origin)
        (dj5ecom) λ python manage.py

        ...
            runserver

        C:\Users\ING\Desktop\2024-DEVSPACE\2024-dj5-ecommerce\root(main -> origin)
        (dj5ecom) λ python manage.py runserver
        Watching for file changes with StatReloader
        Performing system checks...

        System check identified no issues (0 silenced).

        You have 18 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
        Run 'python manage.py migrate' to apply them.
        February 26, 2024 - 15:59:12
        Django version 5.0.2, using settings 'config.settings'
        Starting development server at http://127.0.0.1:8000/
        Quit the server with CTRL-BREAK.
