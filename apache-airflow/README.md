# Apache Airflow quickstart

## Create .env file with user UID

`echo -e "AIRFLOW_UID=$(id -u)\nAIRFLOW_GID=0" > .env`

## Run airflow-init

`docker compose up airflow-init`

## Run other services

`docker compose up`

## Navigate

Open [http://localhost:8080] and use credentials airflow / airflow to access the dashboard.
