FROM bitnami/airflow:2.2.5

USER root
RUN . /opt/bitnami/airflow/venv/bin/activate && pip install authlib apache-airflow-providers-dbt-cloud==1.0.2

USER 1001
