# DjangoNote
## 1.安装Django:<br>
    pip install django==<version>
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

        $error: Microsoft Visual C++ 10.0 is required. Get it with "Microsoft Windows SDK 7.1": www.microsoft.com/download/details.aspx?id=8279
        
   所以则需要下载已经编译好的包(.mhl)使用:<br>
    
    pip install <your_download_packge>
   或者安装好所需要的编译软件后进行pip安装<br>
   
    pip install <module>
   安装.mhl需要先先安装wheel使用:
   
    pip install wheel
    
   安装.mhl时会出现安装不了的情况,是由于python的每个不同版本只支持自己版本的.mhl文件,所以需要将文件中的版本类型改为自己python相同的版本例如:
            
    mysqlclient-1.4.2-cp35-cp35m-win32.whl
   改为:
   
    mysqlclient-1.4.2-cp33-cp33m-win32.whl
   即可.
