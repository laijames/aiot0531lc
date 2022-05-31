# AIoT Github

## Lecture 15: IoT Flask Web (deploy to heroku)
### 前置作業:註冊 Heroku, github 請下載 HeidiSQL, VS code 

### step 1 : Clone this github
 ctrl+shift+p 輸入 git:clone https://github.com/huanchen1107/aiot0530-start-no-token
 選擇自己要的folder存放
 原本是要把local folder裡的.git刪掉(以便產生自己的管理員)並建立自己的repository
 但我的電腦沒有.git 所以我自己新增了一個空資料夾再將必要資料放進去，這樣就可以建立自己的管理員了
### step 2 : install some package

* ctrl+` 開啟終端並輸入以下文字以安裝相關模組
```python
pip insall gunicorn   
Flask==2.0.1 
Jinja2==3.0.1 
psycopg2 
sklearn 
pandas  
numpy 
```

### step 3: add an heroku postgredb

* register heroku account
* go to dashboard
* new an app
* go to resource and add-on an Heroku postgredb
![](image%5C5.jpg)
### step 4: login to heroku pstgredb using HeidiSQL
* 透過HeidiSQL登入STEP3建立的 heroku pstgredb 


```sql
myserver ="<fill-in-Heroku-Postgredb-DB-sever>"
myuser="<fill-in-Heroku-Postgredb-DB-user>"
mypassword="<fill-in-Heroku-Postgredb-DB-pwd>"
mydb="<fill-in-Heroku-Postgredb-DB-db>"

```
### step 5: import postgredb (in db/postgre.db)


### step 6: setting db in app.py


```sql
myserver ="<fill-in-Heroku-Postgredb-DB-sever>"
myuser="<fill-in-Heroku-Postgredb-DB-user>"
mypassword="<fill-in-Heroku-Postgredb-DB-pwd>"
mydb="<fill-in-Heroku-Postgredb-DB-db>"

```
### step 7: testing locally by running python app.py

### step 8: deploy to github (new private github repositoy)

delete .git and git remote add origin master github.com/xxxxx


### step 9: Heroku deploy from github

### step 10: Complete

my link:
https://aiot0531lc.herokuapp.com/





