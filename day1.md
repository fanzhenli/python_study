https://github.com/coco369/

**MVC**
  M��ģ�Ͳ�
  V����ͼ��
  C��ҵ���

**Django,ϵͳ������MVC�Ŀ��ģʽ��Ҳ��ΪMTVģʽ**

* M��ģ�Ͳ�
* V����ͼ������ҵ���߼�
* T��ģ�壺html



#python���⻷���İ�װ
- ͨ��virtualenv��װ���⻷��

   1- pip install virtualenv ��װvirtualenv��
   2- cd python_three/ENV �����������⻷�����ļ��У�ENV���ڿ���̨����
   3- virtualenv --no-site-packages -p C:\Users\Administrator\AppData\Local\Programs\Python\Python36-32\python.exe djenv6

   * -no-site-packages --�����ջ���

   - -p C:\Users\Administrator\AppData\Local\Programs\Python\Python36-32\python.exe -- ָ��python�汾·��
   - djenv6 -- ���⻷����

pip list  --  �鿴���⻷���а�װ�������а�
pip freeze  --  �鿴���⻷����ͨ��pip��װ�������а�

cd djenv6/Scripts/activate  -- �������⻷��
	deactivate --- �˳����⻷��

pip install django==1.11  -- ��װDjango

(djenv6) D:\python_three\wordspace\day1>django-admin startproject day01  -- ��wordspace\day1�ļ��´�����Ϊday01����Ŀ

������Ŀʱ�Զ������ļ����ļ�

**day01**

* init__.py
* settings.py -- ���������Ϣ
* urls.py -- ����·�ɵ�ַ
* wsgi.py --    

**manage.py** -- ���߼��������

python manage.py --  ӳ��ģ�͵����ݿ���

IP��0.0.0.0    port:8080

python manage.py runserver  IP port-- ������Ŀ���Ķ˿ڣ� 

pip install pymysql -- ��װ���ݿ�����

��ʼ�����ݿ������ __init__.py

```
 import pymysql

pymysql.install_as_mysqldb()

```



### �޸����ݿ�����

```
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
```
python manage.py migrate -- �Զ���ӱ�
python manage.py createsuperuser -- ���������û�

���ݿ��еı�
auth_group/auth_group_permissions/auth_permissions/auth_user/auth_user_groups/auth_user_user_permissions -- �����û�Ȩ��









