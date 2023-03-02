# ML_Orchestration_Airflow
## airflow needs a home, ~/airflow is the default, but you can lay the foundation somewhere else if you prefer
```
export AIRFLOW_HOME=~/airflow
```
## ensure to install python and pip package
```
pip install apache-airflow
```
## initialize the database
```
airflow db init
```
## start the web server, default port is 8080
```
airflow webserver -p 8080
```
## start the scheduler
```
airflow scheduler
```
## create an admin user
```
airflow users  create --role Admin --username admin --email admin \
 --firstname admin --lastname admin --password admin
```
## visit localhost:8080 in the browser and use the above credentials to login
