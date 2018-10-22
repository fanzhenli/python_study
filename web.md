https://github.com/coco369/

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

pip list -- 查看安装过的所有软件
pip freeze -- 

cd djenv6/Scripts/activate  -- 进入虚拟环境
	deactivate --- 退出虚拟环境

pip install django==1.11  -- 安装Django










