# Attaa_workshop
# The Steps
### 1- Create Python Virtual Environment (Make sure that you have python or download it  https://www.python.org/downloads )
```
python -m venv attaa   
source attaa/bin/activate       
```
### 2- Install libraries that you need for example
```
pip install flask gunicorn   
```

### 3- Create your foders and files then write the code for example this file (app.py)

```
from flask import Flask             
app = Flask(__name__)               

@app.route("/")                   
def hello():                     
   return "Hello World!"          
 
if __name__ == "__main__":          
   app.run(debug=True)               
 ```  

### 4- run local 
python app.py   

### 5- install heroku CLI based your system for example Mac
```
 brew tap heroku/brew && brew install heroku  
```


### 6- Create requirements.txt 
```
pip freeze > requirements.txt   
```
### 7- Create Procfile file then write in it 
```
web: gunicorn app:app   
```

### 8- heroku login
```
heroku login   
```
### 9- inti and add remote
```
git init  
heroku git:remote -a app-attaa   
```
### 10- commit and push
```
git add .   
git commit -am "make it better"   
git push heroku master    
```
---------------------------
### for deactivate Python Virtual Environment
```
conda deactivate
```
### Or 

```
deactivate
```





