# AIoT Github
<br>  

##### author: "YJCHEN"

## Lecture 15: IoT Flask Web (deploy to heroku)

### step0: Setup Environment
*github,heroku account setup

### step 1 : Clone this github     

* clone  
* delete .git  
* 推送至gitHub




### step 2 : install some package


```python
pip install gunicorn   Flask==2.0.1 Jinja2==3.0.1 psycopg2 sklearn pandas  numpy 
```

### step 3: add an heroku postgredb

* register heroku account
* go to dashboard
* new an app
* go to resource and add-on an Heroku postgredb

### step 4: login to heroku pstgredb using HeidiSQL  

![image](/img/1.PNG) 


```sql
myserver ="ec2-52-72-99-110.compute-1.amazonaws.com"  
myuser="iqmjrjfmvekuwe"  
mypassword="896a432e316c729c6a591a6cc7a0d46a3f0be657b2cc01501e6118f75e365cc2"  
mydb="d7ujfaokgqld81"  

```
### step 5: import postgredb (in db/postgre.db)   

![image](/img/4.PNG)
   

### step 6: setting db in app.py  

![image](/img/5.PNG)   

```sql
myserver ="<fill-in-Heroku-Postgredb-DB-sever>"
myuser="<fill-in-Heroku-Postgredb-DB-user>"
mypassword="<fill-in-Heroku-Postgredb-DB-pwd>"
mydb="<fill-in-Heroku-Postgredb-DB-db>"

```
### step 7: testing locally by running python app.py   

![image](/img/2.PNG) 
![image](/img/3.PNG)   

### step 8: deploy to github (new private github repositoy)

delete .git and git remote add origin master github.com/xxxxx


### step 9: Heroku deploy from github
![image](/img/6.PNG)  

### step 10: Complete

   

Sample link 1:
https://aiot0601-yjchen.herokuapp.com/

Sample link 2: 
https://aiot0529.herokuapp.com/


### Result :(remote random sensor points)
![image](/img/8.PNG)



### Result :(remote after AI prediction)   


![image](/img/7.PNG)

 
