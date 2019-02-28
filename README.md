# DjangoNote
## 1.安装Django:<br>
    pip install django==<version><br>
## 2.创建工程：<br>
    django-admin.py startporject <porject_name> <dir_path>
   或<br>
    django-admin startporject <porject_name> <dir_path>
## 3.创建应用：<br>
    python manage.py <app_name>
## 4.运行工程：<br>
    python manage.py runserver <port>

### 注意:
#### django必须能连上数据库才能运行,所以必须在settings.py中进行设置数据库连接,连接信息将{DATABASES}中的 'ENGINE': 'django.db.backends.mysql'中的mysql换成需要的数据库,并配置好相应的登录信息即可<br>
(1).用数据库时需要下载驱动,由于用pip安装mysql报错<br>

        $error: Microsoft Visual C++ 10.0 is required. Get it with "Microsoft Windows SDK 7.1": www.microsoft.com/download/details.aspx?id=8279<br>
        
   所以则需要下载已经编译好的包(.mhl)使用:<br>
    
    pip install <your_download_packge>
   或者安装好所需要的编译软件后进行pip安装<br>
   
    pip install <module>
   安装.mhl需要先先安装wheel使用:
   
    pip install wheel
