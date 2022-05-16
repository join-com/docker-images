FROM bitnami/airflow:2.2.5

USER root
# hadolint ignore=DL3013,DL3042,SC1091
RUN . /opt/bitnami/airflow/venv/bin/activate && pip install --no-cache-dir authlib apache-airflow-providers-dbt-cloud==1.0.2

USER 1001
