FROM bitnami/airflow:2.3.3

USER root
# hadolint ignore=DL3013,DL3042,SC1091
RUN . /opt/bitnami/airflow/venv/bin/activate && pip install --no-cache-dir authlib apache-airflow-providers-google==8.2.0 apache-airflow-providers-dbt-cloud==2.0.1 airflow-dbt-python==0.14.5

USER 1001
