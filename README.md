# Face_Recognition
## 任务：基于facenet+flask部署一个web解决方案，用户注册上传个人照片，然后通过人脸登录平台
### flask-facenet配置和使用
1. 根据requirements.txt配置好环境（执行pip install -r  requirements.txt）
2. 创建数据库，导入database.sql文件
3. 下载facenet预训练模型(https://github.com/davidsandberg/facenet)，按models\facenet\20180408-102900的方式存放
4. 修改文件face_recognition_api.py中的模型路径modelpath和文件face_mysql.py中的数据库密码等设置
5. 运行face_recognition_api.py文件（python face_recognition_api.py），用浏览器打开显示的地址
6. 使用如图。使用照片和用户则和用户名注册，注册成功返回id和state。注册后使用包含同样人脸的照片（计划改成调用摄像头拍摄人脸来代替上传照片）和用户组登录，成功则返回用户名。
![image](https://github.com/wcszzdzxj/Face_Recognition/blob/master/pic/creat.png)
![image](https://github.com/wcszzdzxj/Face_Recognition/blob/master/pic/failogin.png)
![image](https://github.com/wcszzdzxj/Face_Recognition/blob/master/pic/succreate.png)
![image](https://github.com/wcszzdzxj/Face_Recognition/blob/master/pic/suclogin.png)
