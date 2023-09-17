# Airflow-docker
This repo will guide you way to setup airflow in your local machine using docker img. Here we go ....

prerequisite: Docker and (docker-compose or docker compose, both will be cherry on the cake😉) version should be installed in your system. you can check by following command 

**docker --version**


**docker-compose --version **


**docker compkse version **

Here are the steps in laymens term :

1. create one directory airflow
2. place this yaml file https://airflow.apache.org/docs/apache-airflow/2.7.1/docker-compose.yaml (go with latest one) inside root directory airflow
3. create four more directorys in parent one (airflow), dags, logs, plugins, config
4. create .env file and with AIRFLOW_UID=50000
5. Initialize yaml file, **docker compose up airflow-init** or docker-compose up airflow-init
6. finally spin up your continer, **docker compose up** or **docker-compose up**
7. open http://localhost:8080/ (by default user is airflow and password is also airflow mentioned in the yaml file docker-compose.yaml, you can change it before step 5)

Directory structure :






![image](https://github.com/mvv-git-eng/Airflow-docker/assets/84799610/4b8ce8df-e6b1-4501-ba0d-c0a7072d1e35)





**NOTE** : make sure yor are in airflow directory before executing steps 5 and 6 

Refrence document : https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html
