# Docker中链接mongodb
## 1.docker exec -it 容器名称 image名称
## 2.use admin
## 3.db.auth('root','example') example为密码，创建用户的密码
## 4.show dbs 查看所有的mongodb用户
## 5.use testdb(数据库名)
## 6.创建角色db.createUser({user:'test1',pwd:'123456',roles:[{role:'dbOwner',db:'testdb'}]})
## 创建完用户后 use testdb
## 鉴权用户 db.auth('test1','123456') 用户名+密码