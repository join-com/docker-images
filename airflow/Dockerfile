FROM bitnami/airflow:2.3.3

USER root
# hadolint ignore=DL3013,DL3042,SC1091
RUN . /opt/bitnami/airflow/venv/bin/activate && pip install --no-cache-dir authlib apache-airflow-providers-dbt-cloud==2.0.0

USER 1001
