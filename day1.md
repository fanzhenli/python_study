https://github.com/coco369/

- MVC
M：模型层
V：视图层
C：业务层

- Django
M：模型层
V：视图：处理业务逻辑
T：模板：html



Django,系统采用了MVC的框架模式，也称为MTV模式
MVC -- model（模型）view（视图）controller（控制器）

#python虚拟环境的安装
通过virtualenv安装虚拟环境

- 1 pip install virtualenv 安装virtualenv包
- 2 cd python_three/ENV 创建保存虚拟环境的文件夹（ENV）在控制台进入
- 3 virtualenv --no-site-packages -p C:\Users\Administrator\AppData\Local\Programs\Python\Python36-32\python.exe djenv6
      -- no-site-packages --创建空环境
      -- -p C:\Users\Administrator\AppData\Local\Programs\Python\Python36-32\python.exe -- 指定python版本路径
      -- djenv6 -- 虚拟环境名

pip list -- 查看虚拟环境中安装过的所有包
pip freeze -- 查看虚拟环境中通过pip安装过的所有包

cd djenv6/Scripts/activate  -- 进入虚拟环境
	deactivate --- 退出虚拟环境

pip install django==1.11  -- 安装Django

(djenv6) D:\python_three\wordspace\day1>django-admin startproject day01  -- 在wordspace\day1文件下创建名为day01的项目

创建项目时自动创建的几个文件
__init__.py
__settings.py -- 存放配置信息
urls.py -- 定义路由地址
wsgi.py -- 

python manage.py -- 
python manage.py runserver （8080）-- 运行项目（改端口） 

pip install pymysql -- 安装数据库驱动
 __init__.py import pymysql
---  修改数据库配置
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'dj6',
        'USER':'root',
        'PASSWORD':'123456',
        'HOST':'127.0.0.1',
        'PORT':3306
    }
}

python manage.py migrate -- 自动添加表
python manage.py createsuperuser -- 创建超级用户

数据库中的表
auth_group/auth_group_permissions/auth_permissions/auth_user/auth_user_groups/auth_user_user_permissions -- 设置用户权限









